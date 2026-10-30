# Hathora

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

Hathora provides on-demand, globally distributed dedicated compute for multiplayer games. Hathora Cloud spins game server processes up and down across regions in response to player demand, exposing a REST API to manage applications, builds, deployments, processes, rooms, discovery/ping, logs, metrics, billing, and organization tokens, plus a player-authentication surface that issues short-lived player tokens.

**Areas:** Game Servers · Multiplayer · Compute · Hosting · Orchestration

## Hathora on APIs.io

Everything profiled for Hathora is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/hathora/](https://apis.io/providers/hathora/)** — or go straight to one of the APIs or properties below.

### APIs (11)

- [Hathora AppsV2 API](https://apis.io/apis/hathora/hathora-appsv2-api/) — Create and manage your organization's applications.
- [Hathora AuthV1 API](https://apis.io/apis/hathora/hathora-authv1-api/) — Player authentication - issue short-lived player tokens.
- [Hathora BillingV1 API](https://apis.io/apis/hathora/hathora-billingv1-api/) — Account balance, invoices, payment method, and Stripe portal.
- [Hathora BuildsV3 API](https://apis.io/apis/hathora/hathora-buildsv3-api/) — Upload and manage game server build artifacts.
- [Hathora DeploymentsV3 API](https://apis.io/apis/hathora/hathora-deploymentsv3-api/) — Versioned runtime configuration for a build.
- [Hathora DiscoveryV2 API](https://apis.io/apis/hathora/hathora-discoveryv2-api/) — Region ping endpoints for latency-based routing.
- [Hathora LogsV1 API](https://apis.io/apis/hathora/hathora-logsv1-api/) — Stream and download logs for processes.
- [Hathora ProcessesV3 API](https://apis.io/apis/hathora/hathora-processesv3-api/) — Launch, inspect, and stop running game server processes.
- [Hathora RoomsV2 API](https://apis.io/apis/hathora/hathora-roomsv2-api/) — Create, inspect, and destroy rooms and get connection info.
- [Hathora TokensV1 API](https://apis.io/apis/hathora/hathora-tokensv1-api/) — Create, list, and revoke organization API tokens.
- [Hathora Metrics V1 API](https://apis.io/apis/hathora/hathora-metrics-v1-api/) — Read CPU, memory, egress, and connection metrics for a process.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Hathora Agentic Access](https://apis.io/agentic-access/hathora/hathora-agentic-access/)

#### Collections (12)

Postman and Open Collection request collections.

- [Hathora Cloud API](https://apis.io/collections/hathora/open-hathora/)
- [Hathora Cloud AppsV2 API](https://apis.io/collections/hathora/open-hathora-appsv2-api/)
- [Hathora Cloud AppsV2 AuthV1 API](https://apis.io/collections/hathora/open-hathora-authv1-api/)
- [Hathora Cloud AppsV2 BillingV1 API](https://apis.io/collections/hathora/open-hathora-billingv1-api/)
- [Hathora Cloud AppsV2 BuildsV3 API](https://apis.io/collections/hathora/open-hathora-buildsv3-api/)
- [Hathora Cloud AppsV2 DeploymentsV3 API](https://apis.io/collections/hathora/open-hathora-deploymentsv3-api/)
- [Hathora Cloud AppsV2 DiscoveryV2 API](https://apis.io/collections/hathora/open-hathora-discoveryv2-api/)
- [Hathora Cloud AppsV2 LogsV1 API](https://apis.io/collections/hathora/open-hathora-logsv1-api/)
- [Hathora Cloud AppsV2 MetricsV1 API](https://apis.io/collections/hathora/open-hathora-metricsv1-api/)
- [Hathora Cloud AppsV2 ProcessesV3 API](https://apis.io/collections/hathora/open-hathora-processesv3-api/)
- [Hathora Cloud AppsV2 RoomsV2 API](https://apis.io/collections/hathora/open-hathora-roomsv2-api/)
- [Hathora Cloud AppsV2 TokensV1 API](https://apis.io/collections/hathora/open-hathora-tokensv1-api/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Hathora Authentication](https://apis.io/security/hathora/hathora-authentication/)
- [Hathora Domain Security](https://apis.io/security/hathora/hathora-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Hathora Plans Pricing](https://apis.io/plans/hathora/hathora-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Hathora Rate Limits](https://apis.io/rate-limits/hathora/hathora-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Hathora Finops](https://apis.io/finops/hathora/hathora-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://hathora.dev/)
- [Documentation](https://hathora.dev/docs)
- [Blog](https://gamefabric.com/blog)
- [GitHub](https://github.com/hathora)

## API Evangelist rating

**Kin Score 21.8** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 41.4 |
| Contract governance | 0.0 |
| Operational transparency | 10.5 |
| Developer ergonomics | 15.5 |
| Access clarity | 7.9 |

**Agent readiness 20.4** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | partial |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 11.8** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/hathora/](https://apis.io/providers/hathora/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Hathora: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/hathora/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
