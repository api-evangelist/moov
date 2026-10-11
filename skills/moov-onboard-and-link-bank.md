---
name: moov-onboard-and-link-bank
description: Create a Moov account, request capabilities, link a bank account and verify it with micro-deposits.
api: openapi/moov-openapi.yml
operations: [createAccessToken, createAccount, requestCapabilities, linkBankAccount, initiateMicroDeposits, completeMicroDeposits, listPaymentMethods]
generated: '2026-10-12'
method: generated
---
# Onboard an account and link a bank account

Send `X-Moov-Version: v2026.01.00` on every call (see ../lifecycle/moov-lifecycle.yml).

1. `createAccessToken` with the scopes you need (../scopes/moov-scopes.yml), or use HTTP Basic with your API key.
2. `createAccount` for the individual or business.
3. `requestCapabilities` (e.g. transfers, send-funds, collect-funds); a 409 means requirements are unmet (../errors/moov-problem-types.yml).
4. `linkBankAccount` with account/routing numbers, a Plaid processor token, or an MX authorization code.
5. `initiateMicroDeposits`, then `completeMicroDeposits` with the amounts the user reports.
6. `listPaymentMethods` to get the payment method IDs used as transfer source/destination.

In test mode use the routing numbers and amounts in ../sandbox/moov-sandbox.yml; never use live data.
