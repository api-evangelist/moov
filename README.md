# Moov (moov)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Moov is a financial infrastructure platform that enables developers to embed money movement capabilities directly into their applications. Their developer platform provides a RESTful API, client-side JavaScript SDK, pre-built UI components, and official backend SDKs across multiple languages for building compliant, full-featured financial products.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Banking
- Embedded Finance
- Financial Infrastructure
- Money Movement
- Payments
- Transfers

## Timestamps

- **Created:** 2026-03-21
- **Modified:** 2026-05-19

## APIs

### Moov API

The Moov API is a RESTful financial infrastructure platform that enables developers to integrate money movement capabilities into their applications. The API supports a full range of financial operations including account management, payment method onboarding, transfers, sweeps, refunds, dispute resolution, card issuing, and payment links. Authentication uses OAuth2 access tokens with permission scopes.

- **Human URL:** [https://docs.moov.io/api/](https://docs.moov.io/api/)

#### Tags

- Banking
- Financial Infrastructure
- Money Movement
- Payments
- Transfers

#### Properties

- [Documentation](https://docs.moov.io/api/)
- [OpenAPI](openapi/moov-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/moov-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/moov-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/moov-webhooks-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [JSON Schema](json-schema/moov-account-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/moov-transfer-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/moov-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Moov.js

Moov.js is a client-side JavaScript SDK designed to streamline interactions with the Moov API while keeping personally identifiable information out of developer infrastructure. All PII is transmitted directly to Moov, relieving developers of the responsibility for storing or handling sensitive user data. The SDK supports account creation, funding source integration, and transfer facilitation, along with pre-built UI components called Moov Drops.

- **Human URL:** [https://docs.moov.io/moovjs/](https://docs.moov.io/moovjs/)

#### Tags

- Client SDK
- Data Collection
- JavaScript
- Payments
- PCI Compliance

#### Properties

- [Documentation](https://docs.moov.io/moovjs/)
- [Postman Collection](collections/moov-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/moov-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Moov Drops

Moov Drops are pre-built, drop-in web UI components for complicated payment and account management flows. These components securely collect payment and account information from users without developers needing to build complex financial forms from scratch. Drops integrate with the Moov API and Moov.js to provide a cohesive front-end experience for onboarding, bank account linking, card collection, and other payment-related workflows.

- **Human URL:** [https://docs.moov.io/guides/developer-tools/](https://docs.moov.io/guides/developer-tools/)

#### Tags

- Embedded Finance
- Frontend
- Payments
- UI Components
- Web Components

#### Properties

- [Documentation](https://docs.moov.io/guides/developer-tools/)
- [Postman Collection](collections/moov-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/moov-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Moov Backend SDKs

Moov provides official server-side client libraries for interacting with the Moov API across multiple programming languages, including Go, TypeScript, Python, Java, PHP, Ruby, and C#/.NET. These SDKs abstract the HTTP layer and provide idiomatic interfaces for each language to access Moov's full range of financial operations. Each SDK is actively maintained and versioned to track the Moov API's versioning scheme.

- **Human URL:** [https://docs.moov.io/sdks/](https://docs.moov.io/sdks/)

#### Tags

- .NET
- Go
- Java
- PHP
- Python
- Ruby
- SDK
- TypeScript

#### Properties

- [Documentation](https://docs.moov.io/sdks/)
- [Postman Collection](collections/moov-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/moov-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/moovfinancial)
- [LinkedIn](https://www.linkedin.com/company/moov-io)
- [Portal](https://docs.moov.io/)
- [Documentation](https://docs.moov.io/)
- [Website](https://moov.io/)
- [Blog](https://moov.io/blog/)
- [Login](https://dashboard.moov.io/)
- [Features](undefined)
- [L L Ms Txt](https://docs.moov.io/llms.txt)

## Maintainers

**FN:** API Evangelist
**Email:** info@apievangelist.com
