# Y42 (y42)

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

Y42 is a managed DataOps platform ("Gitful data ops") that runs production-ready data pipelines on top of Snowflake and BigQuery, combining managed Airbyte ingestion, managed dbt Core for SQL models, a DAG-based orchestration scheduler, and a managed Git backend. Most workflows are driven through the Y42 web app and Git, but Y42 also exposes a documented public REST API and webhooks for programmatically managing spaces, triggering orchestration runs, and retrieving run and manifest information.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/y42/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/y42/refs/heads/main/apis.yml)

## Tags

- DataOps
- Data Pipelines
- Orchestration
- dbt
- Snowflake
- BigQuery
- GitOps

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Y42 Spaces API

Programmatically list, create, retrieve, and delete spaces (Y42 environments) within an organization, manage credentials, and configure the underlying data warehouse connection (BigQuery, Snowflake, GCS, S3) via the Git backend endpoints.

- **Human URL:** [https://y42-public-api.readme.io/](https://y42-public-api.readme.io/)
- **Base URL:** `https://api.y42.dev`

#### Tags

- Spaces
- Environments
- Provisioning

#### Properties

- [Documentation](https://docs.y42.com/reference/api_overview)
- [API Reference](https://y42-public-api.readme.io/)
- [OpenAPI](openapi/y42-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/y42.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/y42.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Y42 Orchestration API

Trigger orchestration runs for a space by command or by asset, and retrieve information about runs by id or by conditions, enabling external schedulers and CI/CD systems to drive Y42 data pipelines.

- **Human URL:** [https://y42-public-api.readme.io/](https://y42-public-api.readme.io/)
- **Base URL:** `https://api.y42.dev`

#### Tags

- Orchestration
- Pipelines
- Scheduling

#### Properties

- [Documentation](https://docs.y42.com/reference/api_overview)
- [API Reference](https://y42-public-api.readme.io/)
- [OpenAPI](openapi/y42-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/y42.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/y42.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Y42 Runs API

Retrieve orchestration run details and the latest job information for a space, supporting monitoring, alerting, and observability over pipeline executions.

- **Human URL:** [https://y42-public-api.readme.io/](https://y42-public-api.readme.io/)
- **Base URL:** `https://api.y42.dev`

#### Tags

- Runs
- Jobs
- Monitoring

#### Properties

- [Documentation](https://docs.y42.com/reference/api_overview)
- [API Reference](https://y42-public-api.readme.io/)
- [OpenAPI](openapi/y42-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/y42.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/y42.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Y42 Manifest API

Retrieve the dbt manifest content for a space, exposing the data assets, models, sources, and lineage that make up a Y42 project for downstream tooling.

- **Human URL:** [https://y42-public-api.readme.io/](https://y42-public-api.readme.io/)
- **Base URL:** `https://api.y42.dev`

#### Tags

- Manifest
- dbt
- Assets

#### Properties

- [Documentation](https://docs.y42.com/reference/api_overview)
- [API Reference](https://y42-public-api.readme.io/)
- [OpenAPI](openapi/y42-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/y42.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/y42.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Y42 Webhooks

Y42 documents webhook-based triggers as part of its fully programmable pipelines (alongside the API and CLI), allowing external events to trigger orchestration. Specific webhook payloads and registration endpoints are not fully enumerated in the public API reference and are documented here as available but not reconciled.

- **Human URL:** [https://docs.y42.com/docs/welcome](https://docs.y42.com/docs/welcome)
- **Base URL:** `https://api.y42.dev`

#### Tags

- Webhooks
- Events
- Triggers

#### Properties

- [Documentation](https://docs.y42.com/reference/api_overview)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/y42)
- [Website](https://www.y42.com)
- [Documentation](https://docs.y42.com)
- [Plans](plans/y42-plans-pricing.yml)
- [Rate Limits](rate-limits/y42-rate-limits.yml)
- [Fin Ops](finops/y42-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
