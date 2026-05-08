# RudderStack (rudderstack)

RudderStack is a warehouse-native customer data platform (CDP) for developers, with open-source data plane SDKs (rudder-server) and a managed control plane.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/rudderstack/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=rudderstack-api-evangelist&utm_content=repo)

## Type

- **x-type:** company

## Tags

 - Customer Data Platform, CDP, Data Pipeline, Open Source, Event Streaming, Reverse ETL, Analytics, Identity Resolution

## Timestamps

- **Created:** 2026-05-08
- **Modified:** 2026-05-08

## APIs

| API | Description |
|---|---|
| RudderStack HTTP Tracking API | Identify / track / page / screen / group / alias / batch |
| RudderStack Config Backend API | Manage sources, destinations, connections, workspaces |
| RudderStack Transformations API | JS/Python transforms on streaming pipelines |
| RudderStack Tracking Plan API | Schema governance + event validation |
| RudderStack Data Catalog API | Cross-source schema inventory and lineage |
| RudderStack Profiles API | Warehouse-native identity resolution + Customer 360 |
| RudderStack Audiences API | Audience definition + activation via Reverse ETL |
| RudderStack Reverse ETL API | Warehouse-to-SaaS sync orchestration |
| RudderStack Event Stream API | Event-stream pipeline configuration and operation |
| RudderStack Webhook Source API | Inbound webhooks from third-party SaaS |
| RudderStack Warehouse Destination API | Configure loads to Snowflake/BigQuery/Redshift/etc |
| RudderStack Orchestration API | Airflow + Dagster integration for sync orchestration |

## Common Properties

- [Website](https://www.rudderstack.com/)
- [Documentation](https://www.rudderstack.com/docs/)
- [Pricing](https://www.rudderstack.com/pricing/)
- [GitHub Organization](https://github.com/rudderlabs)
- [Open Source Server (rudder-server)](https://github.com/rudderlabs/rudder-server)
- [Plans](plans/rudderstack-plans-pricing.yml) — API Commons Plans 0.1 (reconciled)
- [RateLimits](rate-limits/rudderstack-rate-limits.yml) — API Commons Rate Limits 0.1 (reconciled)
- [FinOps](finops/rudderstack-finops.yml) — FOCUS-aligned FinOps Framework 1.0 (reconciled)

## Plans Summary

- **Open Source (Self-Hosted)** — AGPLv3, free
- **Free** — 250K events/month, $0
- **Starter** — 1M events/month, $220/month
- **Growth** — Custom volume, custom price (adds Profiles)
- **Enterprise** — Custom volume, custom price (adds Python transforms, HIPAA, SSO)

## Rate Limits Summary

- **Free Plan:** 250K events/month
- **Starter Plan:** 1M events/month
- **Growth/Enterprise:** custom monthly events
- **Per-event payload:** keep under 32 KB
- **Batch payload:** up to 4 MB / 500 events

## Artifacts

| Artifact | Path |
|---|---|
| Plans | `plans/rudderstack-plans-pricing.yml` |
| Rate Limits | `rate-limits/rudderstack-rate-limits.yml` |
| FinOps | `finops/rudderstack-finops.yml` |

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
