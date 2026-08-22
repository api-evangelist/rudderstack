# RudderStack (rudderstack)

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

RudderStack is a warehouse-native customer data platform (CDP) for developers, with open-source data plane SDKs (rudder-server) and a managed control plane. The platform exposes an HTTP Tracking (Event Stream) API for ingest, a Config Backend API for managing sources/destinations/connections, a Transformations API for in-flight event transforms, a Tracking Plan API for schema governance, a Profiles API for identity resolution and audiences, and a Reverse ETL API for warehouse-to-SaaS sync.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/rudderstack/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/rudderstack/refs/heads/main/apis.yml)

## Tags

- Customer Data Platform
- CDP
- Data Pipeline
- Open Source
- Event Streaming
- Reverse ETL
- Analytics
- Identity Resolution

## Timestamps

- **Created:** 2026-05-08
- **Modified:** 2026-05-30

## APIs

### RudderStack HTTP Tracking API

The RudderStack HTTP Tracking API ingests customer events server-side via the standard CDP event-spec calls — identify, track, page, screen, group, alias, and batch — using a Segment-compatible payload at /v1/{call}.

#### Tags

- Tracking
- Events
- HTTP Source
- Identify
- Track
- Page
- Screen
- Group
- Alias
- Batch

#### Properties

- [Documentation](https://www.rudderstack.com/docs/sources/event-streams/http/)
- [API Reference](https://www.rudderstack.com/docs/event-spec/standard-events/)
- [OpenAPI](openapi/rudderstack-gateway-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/rudderstack-gateway.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/rudderstack-gateway.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/rudderstack-event-streaming-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### RudderStack Config Backend API

The RudderStack Config Backend API manages workspace configuration objects — sources, destinations, connections, and workspace settings — supporting full programmatic provisioning of pipelines outside the Dashboard.

#### Tags

- Sources
- Destinations
- Connections
- Workspaces
- Management

#### Properties

- [Documentation](https://www.rudderstack.com/docs/api/)
- [Postman Collection](collections/rudderstack-gateway.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/rudderstack-gateway.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### RudderStack Transformations API

The RudderStack Transformations API manages user-defined transformation functions (JavaScript, with Python on Enterprise) attached to a destination connection to filter, mask, enrich, or reshape events in flight.

#### Tags

- Transformations
- JavaScript
- Python
- Data Quality

#### Properties

- [Documentation](https://www.rudderstack.com/docs/transformations/)
- [Postman Collection](collections/rudderstack-gateway.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/rudderstack-gateway.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### RudderStack Tracking Plan API

The RudderStack Tracking Plan API defines and enforces the canonical event schema (events, properties, traits, types, required fields) used to validate ingested events and surface violations.

#### Tags

- Tracking Plan
- Schema Governance
- Data Quality
- Validation

#### Properties

- [Documentation](https://www.rudderstack.com/docs/data-governance/tracking-plans/)
- [Postman Collection](collections/rudderstack-gateway.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/rudderstack-gateway.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### RudderStack Data Catalog API

The RudderStack Data Catalog API exposes the inventory of events and properties seen across all sources, supporting schema discovery, lineage, and governance reporting.

#### Tags

- Catalog
- Data Governance
- Schema

#### Properties

- [Documentation](https://www.rudderstack.com/docs/data-governance/data-catalog/)
- [Postman Collection](collections/rudderstack-gateway.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/rudderstack-gateway.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### RudderStack Profiles API

The RudderStack Profiles API powers warehouse-native identity resolution, customer feature engineering, and unified Customer 360 model definitions executed inside the customer's data warehouse.

#### Tags

- Profiles
- Identity Resolution
- Customer 360
- Features

#### Properties

- [Documentation](https://www.rudderstack.com/docs/profiles/)
- [Postman Collection](collections/rudderstack-gateway.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/rudderstack-gateway.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### RudderStack Audiences API

The RudderStack Audiences API builds and manages audience definitions in the warehouse and activates them across destinations via Reverse ETL.

#### Tags

- Audiences
- Segmentation
- Activation

#### Properties

- [Documentation](https://www.rudderstack.com/docs/data-pipelines/reverse-etl/features/audiences/)
- [Postman Collection](collections/rudderstack-gateway.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/rudderstack-gateway.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### RudderStack Reverse ETL API

The RudderStack Reverse ETL API manages warehouse-source-to-SaaS-destination syncs, including model definitions, sync schedules, run history, and incremental cursor management.

#### Tags

- Reverse ETL
- Warehouse
- Sync
- Models

#### Properties

- [Documentation](https://www.rudderstack.com/docs/data-pipelines/reverse-etl/)
- [Postman Collection](collections/rudderstack-gateway.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/rudderstack-gateway.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### RudderStack Event Stream API

The RudderStack Event Stream API manages real-time event-stream pipelines — sources, destinations, connections, event filters, and feature toggles — that route events from collection to downstream tools.

#### Tags

- Event Stream
- Pipelines
- Streaming

#### Properties

- [Documentation](https://www.rudderstack.com/docs/data-pipelines/event-stream/)
- [Postman Collection](collections/rudderstack-gateway.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/rudderstack-gateway.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### RudderStack Webhook Source API

The RudderStack Webhook Source API receives inbound webhooks from third-party SaaS tools and normalizes them into RudderStack events for downstream routing.

#### Tags

- Webhooks
- Sources
- Cloud Apps

#### Properties

- [Documentation](https://www.rudderstack.com/docs/sources/event-streams/cloud-apps/webhook-source/)
- [AsyncAPI](asyncapi/rudderstack-event-streaming-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/rudderstack-gateway.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/rudderstack-gateway.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### RudderStack Warehouse Destination API

The RudderStack Warehouse Destination API configures and operates loads into supported warehouses (Snowflake, BigQuery, Redshift, Postgres, Databricks, Trino, S3 Data Lake) with configurable sync interval, schema namespace, and incremental loading.

#### Tags

- Warehouse
- Snowflake
- BigQuery
- Redshift
- Databricks
- Destinations

#### Properties

- [Documentation](https://www.rudderstack.com/docs/destinations/warehouse-destinations/)
- [Postman Collection](collections/rudderstack-gateway.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/rudderstack-gateway.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### RudderStack Orchestration API

The RudderStack Orchestration API integrates with Airflow and Dagster to coordinate Reverse ETL syncs, Profiles model runs, and other RudderStack jobs from external orchestration systems.

#### Tags

- Orchestration
- Airflow
- Dagster
- Workflows

#### Properties

- [Documentation](https://www.rudderstack.com/docs/data-pipelines/orchestration/)
- [Postman Collection](collections/rudderstack-gateway.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/rudderstack-gateway.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/rudderstack)
- [Website](https://www.rudderstack.com/)
- [Documentation](https://www.rudderstack.com/docs/)
- [API Reference](https://www.rudderstack.com/docs/api/)
- [Getting Started](https://www.rudderstack.com/docs/get-started/)
- [Pricing](https://www.rudderstack.com/pricing/)
- [Sign Up](https://app.rudderstack.com/signup)
- [Login](https://app.rudderstack.com/)
- [GitHub Organization](https://github.com/rudderlabs)
- [Open  Source  Server](https://github.com/rudderlabs/rudder-server)
- [Java Script  S D K](https://github.com/rudderlabs/rudder-sdk-js)
- [Node.js  S D K](https://github.com/rudderlabs/rudder-sdk-node)
- [Python  S D K](https://github.com/rudderlabs/rudder-sdk-python)
- [Java  S D K](https://github.com/rudderlabs/rudder-sdk-java)
- [Go  S D K](https://github.com/rudderlabs/analytics-go)
- [Ruby  S D K](https://github.com/rudderlabs/rudder-sdk-ruby)
- [P H P  S D K](https://github.com/rudderlabs/rudder-sdk-php)
- [. N E T  S D K](https://github.com/rudderlabs/rudder-analytics-dotnet)
- [i O S  S D K](https://github.com/rudderlabs/rudder-sdk-ios)
- [Android  S D K](https://github.com/rudderlabs/rudder-sdk-android)
- [Status Page](https://status.rudderstack.com/)
- [Blog](https://www.rudderstack.com/blog/)
- [Changelog](https://www.rudderstack.com/docs/release-notes/)
- [License](https://github.com/rudderlabs/rudder-server/blob/master/LICENSE.md)
- [X ( Twitter)](https://x.com/RudderStack)
- [YouTube](https://www.youtube.com/c/RudderStack)
- [Slack  Community](https://www.rudderstack.com/join-rudderstack-slack-community/)
- [Plans](plans/rudderstack-plans-pricing.yml)
- [Rate Limits](rate-limits/rudderstack-rate-limits.yml)
- [Fin Ops](finops/rudderstack-finops.yml)
- [Integrations](https://www.rudderstack.com/partners/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
