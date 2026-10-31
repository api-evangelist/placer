# Placer

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

Placer.ai is a location analytics and foot-traffic intelligence platform that measures visits, trade areas, demographics, and consumer behavior for physical points of interest across retail, CPG, commercial real estate, hospitality, and the public sector. Its public developer surface, the Placer API (PAPI, base https://papi.placer.ai), lets developers and data analysts extract Placer's location analytics programmatically to enrich, filter, or combine it with other data sources for custom dashboards, internal reporting, and competitive analysis. The v1 REST API covers entity/POI search, custom POI and tag management, and a suite of report endpoints spanning visit metrics and trends, trade area (true trade area, drive-time, demographics), ranking, loyalty, and retail sales. Authentication is a static API key sent in the x-api-key header.

**Areas:** Company · Location Analytics · Foot Traffic · Geospatial · Retail Analytics · Real Estate · Consumer Insights · Data

## Placer on APIs.io

Everything profiled for Placer is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/placer/](https://apis.io/providers/placer/)** — or go straight to one of the APIs or properties below.

### APIs (8)

- [Placer Account Info API](https://apis.io/apis/placer/placer-account-info-api/) — The Account Info API from Placer — 1 operation(s) for account info.
- [Placer Loyalty Reports API](https://apis.io/apis/placer/placer-loyalty-reports-api/) — The Loyalty Reports API from Placer — 1 operation(s) for loyalty reports.
- [Placer Manage POIs API](https://apis.io/apis/placer/placer-manage-pois-api/) — The Manage POIs API from Placer — 6 operation(s) for manage pois.
- [Placer Ranking Reports API](https://apis.io/apis/placer/placer-ranking-reports-api/) — The Ranking Reports API from Placer — 4 operation(s) for ranking reports.
- [Placer Retail Sales Reports API](https://apis.io/apis/placer/placer-retail-sales-reports-api/) — The Retail Sales Reports API from Placer — 5 operation(s) for retail sales reports.
- [Placer Trade Area Reports API](https://apis.io/apis/placer/placer-trade-area-reports-api/) — The Trade Area Reports API from Placer — 3 operation(s) for trade area reports.
- [Placer Visitor Journey Reports API](https://apis.io/apis/placer/placer-visitor-journey-reports-api/) — The Visitor Journey Reports API from Placer — 2 operation(s) for visitor journey reports.
- [Placer Visits Reports API](https://apis.io/apis/placer/placer-visits-reports-api/) — The Visits Reports API from Placer — 7 operation(s) for visits reports.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [placer](https://apis.io/servers/placer/placer/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Placer Agentic Access](https://apis.io/agentic-access/placer/placer-agentic-access/)

#### Collections (8)

Postman and Open Collection request collections.

- [papi Account Info API](https://apis.io/collections/placer/open-placer-account-info-api/)
- [papi Account Info Loyalty Reports API](https://apis.io/collections/placer/open-placer-loyalty-reports-api/)
- [papi Account Info Manage POIs API](https://apis.io/collections/placer/open-placer-manage-pois-api/)
- [papi Account Info Ranking Reports API](https://apis.io/collections/placer/open-placer-ranking-reports-api/)
- [papi Account Info Retail Sales Reports API](https://apis.io/collections/placer/open-placer-retail-sales-reports-api/)
- [papi Account Info Trade Area Reports API](https://apis.io/collections/placer/open-placer-trade-area-reports-api/)
- [papi Account Info Visitor Journey Reports API](https://apis.io/collections/placer/open-placer-visitor-journey-reports-api/)
- [papi Account Info Visits Reports API](https://apis.io/collections/placer/open-placer-visits-reports-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Placer Papi Overlay](https://apis.io/overlays/placer/placer-papi-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Placer Authentication](https://apis.io/security/placer/placer-authentication/)
- [Placer Domain Security](https://apis.io/security/placer/placer-domain-security/)

#### Rate limits (1)

Published request limits.

- [Placer Rate Limits](https://apis.io/rate-limits/placer/placer-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://placer.ai)
- [Documentation](https://docs.placer.ai/docs/welcome-to-placers-feeds)
- [Getting started](https://docs.placer.ai/reference/getting-started)
- [API reference](https://docs.placer.ai/reference/welcome-to-papi)
- [Pricing](https://www.placer.ai/pricing)
- [Support](https://analytics.placer.ai/my-zone/my-requests/support-requests)
- [Changelog](https://docs.placer.ai/changelog)
- [Blog](https://www.placer.ai/blog)
- [Terms of service](https://www.placer.ai/terms-of-service)
- [Privacy policy](https://www.placer.ai/privacy-policy)

## API Evangelist rating

**Kin Score 41.3** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 49.9 |
| Contract governance | 4.5 |
| Operational transparency | 43.4 |
| Developer ergonomics | 35.1 |
| Access clarity | 38.2 |

**Agent readiness 26.7** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | partial |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 24.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/placer/](https://apis.io/providers/placer/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Placer: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/placer/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
