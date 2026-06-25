# Y42 (y42)

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
