# Hathora (hathora)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
