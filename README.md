# YouScan

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

YouScan is an AI-powered social media listening and consumer-intelligence platform that monitors mentions, conversations, and images across social networks, news, blogs, forums, and review sites. It provides sentiment analysis, trend and topic detection, visual insights via image recognition, and an AI Insights Copilot for querying data in natural language. YouScan exposes a REST API (documented with an OpenAPI 3.1 specification) to manage monitoring topics, retrieve and stream mentions, manage tags, run data imports, and query statistics, plus outbound webhooks that push new mentions to subscriber endpoints in real time.

**Areas:** Company · Social Media Listening · Social Intelligence · Consumer Insights · Sentiment Analysis · Media Monitoring · Analytics · Artificial Intelligence

## YouScan on APIs.io

Everything profiled for YouScan is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/youscan/](https://apis.io/providers/youscan/)** — or go straight to one of the APIs or properties below.

### APIs (8)

- [YouScan Data Import API](https://apis.io/apis/youscan/youscan-data-import-api/) — The Data Import API allows you to import mentions from external sources into YouScan topics. This feature enables you to bring historical data or mentions…
- [YouScan History API](https://apis.io/apis/youscan/youscan-history-api/) — Manage historical data collection for a topic. Starting a collection can return `400` if a collection is already running, if the date range is invalid, or…
- [YouScan Mentions API](https://apis.io/apis/youscan/youscan-mentions-api/) — Retrieve and update mentions collected in a topic. ### How to effectively retrieve large sets of mentions Common scenarios are: * Load all the mentions from…
- [YouScan Spaces API](https://apis.io/apis/youscan/youscan-spaces-api/) — Spaces available to the authenticated user and categories configured in them.
- [YouScan Statistics API](https://apis.io/apis/youscan/youscan-statistics-api/) — Aggregated statistics for mentions of a topic. ### Dates `from` and `to` are dates (`yyyy-MM-dd`); `to` is inclusive. Day boundaries are computed in the API…
- [YouScan Tags API](https://apis.io/apis/youscan/youscan-tags-api/) — Manage tags created in your topic.
- [YouScan Topics API](https://apis.io/apis/youscan/youscan-topics-api/) — Create and manage topics — the monitoring entities that collect mentions matching your queries. ### Topic query structure A topic query consists of a…
- [YouScan Webhook API](https://apis.io/apis/youscan/youscan-webhook-api/) — Webhooks push new mentions to your own server in real time, so you don't have to poll the API. Every time a new mention is found and saved to a topic,…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Youscan Mentions Webhooks](https://apis.io/asyncapis/youscan/youscan-mentions-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [youscan](https://apis.io/servers/youscan/youscan/)

#### Collections (8)

Postman and Open Collection request collections.

- [YouScan Data Import API](https://apis.io/collections/youscan/open-youscan-data-import-api/)
- [YouScan Data Import History API](https://apis.io/collections/youscan/open-youscan-history-api/)
- [YouScan Data Import Mentions API](https://apis.io/collections/youscan/open-youscan-mentions-api/)
- [YouScan Data Import Spaces API](https://apis.io/collections/youscan/open-youscan-spaces-api/)
- [YouScan Data Import Statistics API](https://apis.io/collections/youscan/open-youscan-statistics-api/)
- [YouScan Data Import Tags API](https://apis.io/collections/youscan/open-youscan-tags-api/)
- [YouScan Data Import Topics API](https://apis.io/collections/youscan/open-youscan-topics-api/)
- [YouScan Data Import Webhook API](https://apis.io/collections/youscan/open-youscan-webhook-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Youscan Openapi Overlay](https://apis.io/overlays/youscan/youscan-openapi-overlay/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Youscan Authentication](https://apis.io/security/youscan/youscan-authentication/)
- [Youscan Domain Security](https://apis.io/security/youscan/youscan-domain-security/)
- [Youscan Trust Center](https://apis.io/security/youscan/youscan-trust-center/)
- [Youscan Vulnerability Disclosure](https://apis.io/security/youscan/youscan-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Youscan Plans Pricing](https://apis.io/plans/youscan/youscan-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Youscan Rate Limits](https://apis.io/rate-limits/youscan/youscan-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://youscan.io)
- [Documentation](https://developers.youscan.io/)
- [Getting started](https://help.youscan.io/en/articles/2754452-how-to-use-youscan-api)
- [API reference](https://developers.youscan.io/api/)
- [Pricing](https://youscan.io/pricing/)
- [Sign up](https://app.youscan.io)
- [Support](https://help.youscan.io/en/collections/76280-integrations-and-api)
- [Blog](https://youscan.io/blog/)
- [Terms of service](https://youscan.io/terms-of-service)
- [Privacy policy](https://youscan.io/privacy-policy)
- [GitHub](https://github.com/youscan)

## API Evangelist rating

**Kin Score 57.8** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 60.4 |
| Contract governance | 18.2 |
| Operational transparency | 73.7 |
| Developer ergonomics | 39.9 |
| Access clarity | 68.4 |

**Agent readiness 35.4** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | verified |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 32.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/youscan/](https://apis.io/providers/youscan/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for YouScan: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/youscan/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
