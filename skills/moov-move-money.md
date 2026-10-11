---
name: moov-move-money
description: Create a Moov transfer safely with an idempotency key, track it, and cancel, refund or reverse it if needed.
api: openapi/moov-openapi.yml
operations: [createTransferOptions, createTransfer, getTransfer, createCancellation, initiateRefund, createReversal]
generated: '2026-10-12'
method: generated
---
# Move money and reverse it

1. `createTransferOptions` to see which payment-method pairs and rails are available.
2. `createTransfer` with a deterministic `X-Idempotency-Key` (up to 36 chars or UUID v5; keys never expire). A repeat key returns 409 — do not retry with the same key expecting a new transfer.
3. Transfers are asynchronous: use webhooks (../asyncapi/) or the `x-wait-for` header, then `getTransfer`. A 202 means the rail response timed out; read the transfer later.
4. To undo: ACH transfers use `createCancellation` within the cancellation window; card transfers use `createReversal` (cancel or refund) or `initiateRefund`. Both refund/reversal calls take an `X-Idempotency-Key`; after a 4xx decline, retry with a NEW key.
5. Card declines carry a `failureCode` — see ../errors/moov-decline-codes.yml for the action to take.

Rate limit: 40 requests/second per account ID (10 in test mode); 429 says how long to wait.
