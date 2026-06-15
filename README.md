# RudderStack (rudderstack)

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
