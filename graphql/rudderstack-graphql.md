# RudderStack GraphQL Schema

## Overview

This conceptual GraphQL schema models the RudderStack customer data platform (CDP) API surface. RudderStack is a warehouse-native CDP for developers that provides an open-source data plane and a managed control plane. The schema covers the full breadth of the platform: event ingestion, source and destination management, pipeline configuration, transformations, identity resolution, tracking plans, regulations, and data governance.

The schema is derived from the RudderStack public documentation and API reference at https://www.rudderstack.com/docs/api/.

## Schema Source

- API Reference: https://www.rudderstack.com/docs/api/
- Event Spec: https://www.rudderstack.com/docs/event-spec/standard-events/
- Config Backend API: https://www.rudderstack.com/docs/api/
- Transformations API: https://www.rudderstack.com/docs/transformations/
- Tracking Plan API: https://www.rudderstack.com/docs/data-governance/tracking-plans/
- Profiles API: https://www.rudderstack.com/docs/profiles/
- Reverse ETL API: https://www.rudderstack.com/docs/data-pipelines/reverse-etl/

## Type Categories

### Event Ingestion Types
Models the RudderStack HTTP Tracking API event-spec calls. Covers the six standard CDP event types (Track, Identify, Page, Screen, Group, Alias) plus batch ingestion. Each event carries a Context object with sub-contexts for App, Device, Library, Network, OS, Page, and Campaign data.

- `Event`, `EventDetails`, `EventType`
- `TrackEvent`, `IdentifyEvent`, `PageEvent`, `ScreenEvent`, `GroupEvent`, `AliasEvent`
- `Property`, `PropertyType`, `PropertyValue`
- `Context`, `ContextDetails`, `AppContext`, `DeviceContext`, `LibraryContext`, `NetworkContext`, `OSContext`, `PageContext`
- `Campaign`

### Identity and User Types
Models the user identity graph and profile resolution capabilities. RudderStack uses both a `userId` (known, authenticated) and an `anonymousId` (pre-login or anonymous) to stitch user journeys across sessions and devices.

- `UserProfile`, `UserDetails`, `UserIdentity`
- `UserId`, `AnonymousId`
- `Traits`, `TraitDetails`, `TraitType`
- `Group`, `GroupDetails`, `GroupTraits`

### Source and Destination Management
Models the Config Backend API objects for managing workspace configuration programmatically. Sources are data origins (SDKs, HTTP, cloud apps, warehouses). Destinations are downstream tools or warehouses that receive processed events.

- `Source`, `SourceDetails`, `SourceType`, `SourceStatus`
- `Destination`, `DestinationDetails`, `DestinationType`
- `Connection`, `ConnectionDetails`, `ConnectionMode`

### Pipeline and Webhook Types
Models the pipeline execution layer — the data plane configuration that routes events from sources through transformations to destinations — plus webhook ingestion sources.

- `Pipeline`, `PipelineDetails`, `PipelineStatus`
- `Webhook`

### Transformation Types
Models user-defined transformation functions (JavaScript or Python) that filter, mask, enrich, or reshape events in flight as they pass through a destination connection.

- `Transformation`, `TransformationDetails`, `TransformationCode`
- `UserTransformation`, `StreamTransformation`

### Data Governance and Regulation Types
Models the privacy and compliance layer: tracking plans that enforce schema governance, suppression lists for GDPR/CCPA opt-outs, and deletion requests.

- `Regulation`, `RegulationType`
- `DataSuppression`, `DataDeletion`

### Authentication Types
Models workspace-scoped authentication credentials.

- `APIKey`, `Token`

## Root Operations

### Query
- `source(id: ID!)` — fetch a single source by ID
- `sources` — list all sources in the workspace
- `destination(id: ID!)` — fetch a single destination by ID
- `destinations` — list all destinations
- `connection(id: ID!)` — fetch a single source-destination connection
- `connections` — list all connections
- `event(id: ID!)` — look up a stored event by ID
- `userProfile(userId: ID!)` — fetch a resolved user profile
- `transformation(id: ID!)` — fetch a transformation by ID
- `transformations` — list all transformations
- `pipeline(id: ID!)` — fetch a pipeline by ID
- `pipelines` — list all pipelines
- `regulation(id: ID!)` — fetch a regulation request by ID
- `regulations` — list all regulation requests
- `webhook(id: ID!)` — fetch a webhook source by ID
- `webhooks` — list all webhook sources
- `apiKey(id: ID!)` — fetch an API key by ID

### Mutation
- `createSource(input: SourceInput!)` — create a new source
- `updateSource(id: ID!, input: SourceInput!)` — update an existing source
- `deleteSource(id: ID!)` — remove a source
- `createDestination(input: DestinationInput!)` — create a new destination
- `updateDestination(id: ID!, input: DestinationInput!)` — update a destination
- `deleteDestination(id: ID!)` — remove a destination
- `createConnection(input: ConnectionInput!)` — connect a source to a destination
- `deleteConnection(id: ID!)` — remove a connection
- `createTransformation(input: TransformationInput!)` — create a transformation function
- `updateTransformation(id: ID!, input: TransformationInput!)` — update a transformation
- `deleteTransformation(id: ID!)` — remove a transformation
- `trackEvent(input: TrackEventInput!)` — ingest a track event
- `identifyEvent(input: IdentifyEventInput!)` — ingest an identify event
- `pageEvent(input: PageEventInput!)` — ingest a page event
- `screenEvent(input: ScreenEventInput!)` — ingest a screen event
- `groupEvent(input: GroupEventInput!)` — ingest a group event
- `aliasEvent(input: AliasEventInput!)` — ingest an alias event
- `createRegulation(input: RegulationInput!)` — submit a data regulation request (deletion/suppression)
- `createWebhook(input: WebhookInput!)` — register a webhook source
- `deleteWebhook(id: ID!)` — remove a webhook source
- `createAPIKey(input: APIKeyInput!)` — generate a new API key
- `revokeAPIKey(id: ID!)` — revoke an API key
