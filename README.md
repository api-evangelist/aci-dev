# ACI.dev

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

ACI.dev (Aipolabs Agent-Computer Interface) is an open-source tool-calling platform that hooks AI agents into 600+ pre-built tools through direct function calling or a unified Model Context Protocol server. Maintained by Aipotheosis Labs (Aipolabs) under Apache 2.0, ACI provides multi-tenant OAuth2 and API-key authentication, per-project App Configurations, natural-language permission guardrails, OpenAI- and Anthropic-compatible function definitions, Python and TypeScript SDKs, and the unified aci-mcp server with ACI_SEARCH_FUNCTIONS and ACI_EXECUTE_FUNCTION meta-tools. The sister project Gate22 adds an open-source MCP gateway and control plane for governing which tools agents can use, what they can do, and how it is audited.

**Areas:** Agent Infrastructure · Agents · Artificial Intelligence · Function Calling · MCP · Authentication · Open Source · Tool Calling · VibeOps

## ACI.dev on APIs.io

Everything profiled for ACI.dev is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/aci-dev/](https://apis.io/providers/aci-dev/)** — or go straight to one of the APIs or properties below.

### APIs (4)

- [ACI.dev App Configurations API](https://apis.io/apis/aci-dev/aci-dev-app-configurations-api/) — The app-configurations API from ACI.dev — 2 operation(s) for app-configurations.
- [ACI.dev Apps API](https://apis.io/apis/aci-dev/aci-dev-apps-api/) — The apps API from ACI.dev — 2 operation(s) for apps.
- [ACI.dev Functions API](https://apis.io/apis/aci-dev/aci-dev-functions-api/) — The functions API from ACI.dev — 3 operation(s) for functions.
- [ACI.dev Linked Accounts API](https://apis.io/apis/aci-dev/aci-dev-linked-accounts-api/) — The linked-accounts API from ACI.dev — 4 operation(s) for linked-accounts.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Aci Dev Agentic Access](https://apis.io/agentic-access/aci-dev/aci-dev-agentic-access/)

#### JSON Schema (9)

The data models the API reads and writes.

- [AnthropicFunctionDefinition](https://apis.io/schemas/aci-dev/aci-dev-anthropic-function-definition/)
- [AppBasic](https://apis.io/schemas/aci-dev/aci-dev-app/)
- [AppConfigurationPublic](https://apis.io/schemas/aci-dev/aci-dev-app-configuration/)
- [AppBasicWithFunctions](https://apis.io/schemas/aci-dev/aci-dev-app-with-functions/)
- [FunctionBasic](https://apis.io/schemas/aci-dev/aci-dev-function/)
- [FunctionExecute](https://apis.io/schemas/aci-dev/aci-dev-function-execute/)
- [FunctionExecutionResult](https://apis.io/schemas/aci-dev/aci-dev-function-execution-result/)
- [LinkedAccountPublic](https://apis.io/schemas/aci-dev/aci-dev-linked-account/)
- [OpenAIFunctionDefinition](https://apis.io/schemas/aci-dev/aci-dev-openai-function-definition/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Aci Dev Context](https://apis.io/jsonld/aci-dev/aci-dev-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [ACI.dev Vocabulary](https://apis.io/vocabularies/aci-dev/aci-dev-vocabulary/)

#### Examples (3)

Example requests and responses.

- [Aci Dev Execute Function Example](https://apis.io/examples/aci-dev/aci-dev-execute-function-example/)
- [Aci Dev Link Oauth2 Account Example](https://apis.io/examples/aci-dev/aci-dev-link-oauth2-account-example/)
- [Aci Dev Search Functions Example](https://apis.io/examples/aci-dev/aci-dev-search-functions-example/)

#### Collections (5)

Postman and Open Collection request collections.

- [ACI.dev API](https://apis.io/collections/aci-dev/open-aci-dev/)
- [ACI.dev app-configurations API](https://apis.io/collections/aci-dev/open-aci-dev-app-configurations-api/)
- [ACI.dev app-configurations apps API](https://apis.io/collections/aci-dev/open-aci-dev-apps-api/)
- [ACI.dev app-configurations functions API](https://apis.io/collections/aci-dev/open-aci-dev-functions-api/)
- [ACI.dev app-configurations linked-accounts API](https://apis.io/collections/aci-dev/open-aci-dev-linked-accounts-api/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [ACI.dev — jsonschema rules](https://apis.io/rules/aci-dev/aci-dev-jsonschema-spectral-rules/)
- [ACI.dev API Rules](https://apis.io/rules/aci-dev/aci-dev-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Aci Dev Authentication](https://apis.io/security/aci-dev/aci-dev-authentication/)
- [Aci Dev Domain Security](https://apis.io/security/aci-dev/aci-dev-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.aci.dev/)
- [Documentation](https://aci.dev/docs)
- [Getting started](https://aci.dev/docs/introduction/quickstart.md)
- [GitHub](https://github.com/aipotheosis-labs)

## API Evangelist rating

**Kin Score 35.0** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 57.1 |
| Contract quality | 65.1 |
| Contract governance | 27.3 |
| Operational transparency | 2.6 |
| Developer ergonomics | 50.0 |
| Access clarity | 0.0 |

**Agent readiness 24.3** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | — |
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

**Regulatory alignment 15.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/aci-dev/](https://apis.io/providers/aci-dev/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for ACI.dev: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/aci-dev/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
