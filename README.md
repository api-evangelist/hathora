# Hathora (hathora)

Hathora provides on-demand, globally distributed dedicated compute for multiplayer games. Hathora Cloud spins game server processes up and down across regions in response to player demand, exposing a REST API to manage applications, builds, deployments, processes, rooms, discovery/ping, logs, metrics, billing, and organization tokens, plus a player-authentication surface that issues short-lived player tokens.

> **Note:** Hathora is winding down its public Hathora Cloud offering and moving to GameFabric (hathora.dev/pricing redirects to gamefabric.com). This entry documents the Hathora Cloud REST API at its last public state. See `review.yml` for details.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/apis.yml)

## Tags

- Game Servers
- Multiplayer
- Compute
- Hosting
- Orchestration

## Timestamps

- **Created:** 2026-07-01
- **Modified:** 2026-07-01

## APIs

### Hathora Auth API

Issues short-lived player tokens for game clients via anonymous, nickname, and Google OIDC login flows, used to authorize room and lobby operations.

- **Human URL:** [https://hathora.dev/docs/api-reference/auth-v1](https://hathora.dev/docs/api-reference/auth-v1)
- **Base URL:** `https://api.hathora.dev`

#### Tags

- Authentication
- Player Tokens
- JWT

#### Properties

- [Documentation](https://hathora.dev/docs)
- [API Reference](https://hathora.dev/api#tag/AuthV1)
- [OpenAPI](openapi/hathora-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/hathora.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/hathora.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Hathora Apps API

Create, list, read, update, and delete the applications that group your game server builds, deployments, and processes under an organization.

- **Human URL:** [https://hathora.dev/docs/api-reference/apps-v2](https://hathora.dev/docs/api-reference/apps-v2)
- **Base URL:** `https://api.hathora.dev`

#### Tags

- Applications
- Management

#### Properties

- [Documentation](https://hathora.dev/docs)
- [API Reference](https://hathora.dev/api#tag/AppsV2)
- [OpenAPI](openapi/hathora-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/hathora.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/hathora.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Hathora Builds API

Create a build, upload a game server tarball, run the build into a container image, and list, inspect, or delete builds for an application.

- **Human URL:** [https://hathora.dev/docs/api-reference/builds-v3](https://hathora.dev/docs/api-reference/builds-v3)
- **Base URL:** `https://api.hathora.dev`

#### Tags

- Builds
- Container Images
- Deploy

#### Properties

- [Documentation](https://hathora.dev/docs)
- [API Reference](https://hathora.dev/api#tag/BuildsV3)
- [OpenAPI](openapi/hathora-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/hathora.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/hathora.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Hathora Deployments API

Create and read deployments — the versioned runtime configuration (CPU, memory, transport, ports, env, rooms-per-process, idle timeout) that binds a build to how new processes run.

- **Human URL:** [https://hathora.dev/docs/api-reference/deployments-v3](https://hathora.dev/docs/api-reference/deployments-v3)
- **Base URL:** `https://api.hathora.dev`

#### Tags

- Deployments
- Runtime Configuration

#### Properties

- [Documentation](https://hathora.dev/docs)
- [API Reference](https://hathora.dev/api#tag/DeploymentsV3)
- [OpenAPI](openapi/hathora-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/hathora.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/hathora.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Hathora Processes API

Start game server processes in a chosen region, list latest processes, read process details (host, port, allocation, status), and stop a running process.

- **Human URL:** [https://hathora.dev/docs/api-reference/processes-v3](https://hathora.dev/docs/api-reference/processes-v3)
- **Base URL:** `https://api.hathora.dev`

#### Tags

- Processes
- Compute
- Lifecycle

#### Properties

- [Documentation](https://hathora.dev/docs)
- [API Reference](https://hathora.dev/api#tag/ProcessesV3)
- [OpenAPI](openapi/hathora-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/hathora.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/hathora.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Hathora Rooms API

Create rooms on running processes, poll for connection info (host/port), read room status, and destroy rooms — the unit game clients connect to for a match.

- **Human URL:** [https://hathora.dev/docs/api-reference/rooms-v2](https://hathora.dev/docs/api-reference/rooms-v2)
- **Base URL:** `https://api.hathora.dev`

#### Tags

- Rooms
- Matchmaking
- Connection Info

#### Properties

- [Documentation](https://hathora.dev/docs)
- [API Reference](https://hathora.dev/api#tag/RoomsV2)
- [OpenAPI](openapi/hathora-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/hathora.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/hathora.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Hathora Discovery API

Returns every region with a host and port that a game client can directly ping, enabling latency-based routing to the nearest region.

- **Human URL:** [https://hathora.dev/docs/api-reference/discovery-v2](https://hathora.dev/docs/api-reference/discovery-v2)
- **Base URL:** `https://api.hathora.dev`

#### Tags

- Discovery
- Ping
- Latency

#### Properties

- [Documentation](https://hathora.dev/docs)
- [API Reference](https://hathora.dev/api#tag/DiscoveryV2)
- [OpenAPI](openapi/hathora-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/hathora.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/hathora.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Hathora Logs API

Stream live logs for a running process and download the full log file for a stopped process, keyed by appId and processId.

- **Human URL:** [https://hathora.dev/docs/api-reference/logs-v1](https://hathora.dev/docs/api-reference/logs-v1)
- **Base URL:** `https://api.hathora.dev`

#### Tags

- Logs
- Observability
- Streaming

#### Properties

- [Documentation](https://hathora.dev/docs)
- [API Reference](https://hathora.dev/api#tag/LogsV1)
- [OpenAPI](openapi/hathora-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/hathora.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/hathora.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Hathora Metrics API

Read time-series metrics for a process — CPU, memory, egress rate, total egress, and active connections — to monitor game server health and capacity.

- **Human URL:** [https://hathora.dev/docs/api-reference/metrics-v1](https://hathora.dev/docs/api-reference/metrics-v1)
- **Base URL:** `https://api.hathora.dev`

#### Tags

- Metrics
- Monitoring
- Telemetry

#### Properties

- [Documentation](https://hathora.dev/docs)
- [API Reference](https://hathora.dev/api#tag/MetricsV1)
- [OpenAPI](openapi/hathora-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/hathora.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/hathora.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Hathora Billing API

Read account balance and invoice history, view the stored payment method, and initialize a Stripe customer portal URL for self-service billing management.

- **Human URL:** [https://hathora.dev/docs/api-reference/billing-v1](https://hathora.dev/docs/api-reference/billing-v1)
- **Base URL:** `https://api.hathora.dev`

#### Tags

- Billing
- Invoices
- Payments

#### Properties

- [Documentation](https://hathora.dev/docs)
- [API Reference](https://hathora.dev/api#tag/BillingV1)
- [OpenAPI](openapi/hathora-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/hathora.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/hathora.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Hathora Tokens API

Create, list, and revoke the organization API tokens (hathoraDevToken) used as bearer credentials for the management endpoints of the Hathora Cloud API.

- **Human URL:** [https://hathora.dev/docs/api-reference/tokens-v1](https://hathora.dev/docs/api-reference/tokens-v1)
- **Base URL:** `https://api.hathora.dev`

#### Tags

- Tokens
- Organization
- API Keys

#### Properties

- [Documentation](https://hathora.dev/docs)
- [API Reference](https://hathora.dev/api#tag/TokensV1)
- [OpenAPI](openapi/hathora-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/hathora.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/hathora.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/hathora)
- [LinkedIn](https://www.linkedin.com/company/hathora)
- [Website](https://hathora.dev/)
- [Documentation](https://hathora.dev/docs)
- [Plans](plans/hathora-plans-pricing.yml)
- [Rate Limits](rate-limits/hathora-rate-limits.yml)
- [Fin Ops](finops/hathora-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
