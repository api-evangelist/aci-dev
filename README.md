# ACI.dev (aci-dev)

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

ACI.dev (Aipolabs Agent-Computer Interface) is an open-source tool-calling platform that hooks AI agents into 600+ pre-built tools through direct function calling or a unified Model Context Protocol server. Maintained by Aipotheosis Labs (Aipolabs) under Apache 2.0, ACI provides multi-tenant OAuth2 and API-key authentication, per-project App Configurations, natural-language permission guardrails, OpenAI- and Anthropic-compatible function definitions, Python and TypeScript SDKs, and the unified aci-mcp server with ACI_SEARCH_FUNCTIONS and ACI_EXECUTE_FUNCTION meta-tools. The sister project Gate22 adds an open-source MCP gateway and control plane for governing which tools agents can use, what they can do, and how it is audited.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/aci-dev/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/aci-dev/refs/heads/main/apis.yml)

## Scope

- **Position:** Producing
- **Access:** 3rd-Party

## Tags

- Agent Infrastructure
- Agents
- AI
- Artificial Intelligence
- Function Calling
- MCP
- Model Context Protocol
- OAuth
- Open Source
- Tool Calling
- VibeOps

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### ACI.dev Apps API

Search and inspect the 600+ pre-built Apps in the ACI.dev catalog. Apps are external service integrations (Slack, Gmail, Zendesk, GitHub, etc.) that expose Functions for AI agents to call. Search supports natural-language intent for vector similarity ranking and filtering by category or configured-only.

- **Human URL:** [https://aci.dev/docs/core-concepts/app.md](https://aci.dev/docs/core-concepts/app.md)

#### Tags

- Apps
- Catalog
- Tool Calling

#### Properties

- [Documentation](https://aci.dev/docs/core-concepts/app.md)
- [Documentation](https://aci.dev/docs/api-reference/apps/search-apps.md)
- [Documentation](https://aci.dev/docs/api-reference/apps/get-app-details.md)
- [OpenAPI](openapi/aci-dev-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/aci-dev.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/aci-dev.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/aci-dev-app-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/aci-dev-app-with-functions-schema.json) — [JSON Schema](https://json-schema.org/specification)

### ACI.dev Functions API

Search, inspect, and execute the callable Functions (tools) exposed by configured Apps. Function definitions are returned in OpenAI- and Anthropic-compatible JSON Schema, and the same surface powers the unified MCP server's ACI_SEARCH_FUNCTIONS and ACI_EXECUTE_FUNCTION meta-tools.

- **Human URL:** [https://aci.dev/docs/core-concepts/function.md](https://aci.dev/docs/core-concepts/function.md)

#### Tags

- Functions
- Tool Calling
- MCP

#### Properties

- [Documentation](https://aci.dev/docs/core-concepts/function.md)
- [Documentation](https://aci.dev/docs/api-reference/functions/search-functions.md)
- [Documentation](https://aci.dev/docs/api-reference/functions/get-function-definition.md)
- [Documentation](https://aci.dev/docs/api-reference/functions/execute.md)
- [OpenAPI](openapi/aci-dev-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/aci-dev.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/aci-dev.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/aci-dev-function-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/aci-dev-function-execute-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/aci-dev-function-execution-result-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/aci-dev-openai-function-definition-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/aci-dev-anthropic-function-definition-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/aci-dev-search-functions-example.json)
- [Example](examples/aci-dev-execute-function-example.json)

### ACI.dev App Configurations API

Create and manage per-project App Configurations. An App Configuration declares which App is enabled, which security scheme it should use (OAuth2, API key, or no-auth), which functions are permitted, and any security-scheme overrides. App Configurations are the governance boundary for the ACI.dev tool catalog.

- **Human URL:** [https://aci.dev/docs/core-concepts/app-configuration.md](https://aci.dev/docs/core-concepts/app-configuration.md)

#### Tags

- App Configurations
- Governance
- Authentication

#### Properties

- [Documentation](https://aci.dev/docs/core-concepts/app-configuration.md)
- [OpenAPI](openapi/aci-dev-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/aci-dev.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/aci-dev.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/aci-dev-app-configuration-schema.json) — [JSON Schema](https://json-schema.org/specification)

### ACI.dev Linked Accounts API

Manage end-user Linked Accounts for configured Apps. Initiate an OAuth2 link flow, handle the OAuth2 callback, list and retrieve linked accounts by owner ID, and revoke a Linked Account. White-label OAuth2 is supported so production agents can present the customer's own brand during the consent screen.

- **Human URL:** [https://aci.dev/docs/core-concepts/linked-account.md](https://aci.dev/docs/core-concepts/linked-account.md)

#### Tags

- Linked Accounts
- OAuth
- Authentication

#### Properties

- [Documentation](https://aci.dev/docs/core-concepts/linked-account.md)
- [Documentation](https://aci.dev/docs/api-reference/linked-accounts/link-oauth2-account.md)
- [Documentation](https://aci.dev/docs/api-reference/linked-accounts/linked-accounts-oauth2-callback.md)
- [Documentation](https://aci.dev/docs/advanced/oauth2-whitelabel.md)
- [OpenAPI](openapi/aci-dev-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/aci-dev.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/aci-dev.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/aci-dev-linked-account-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/aci-dev-link-oauth2-account-example.json)

## Common Properties

- [Portal](https://aci.dev)
- [Documentation](https://aci.dev/docs)
- [Getting Started](https://aci.dev/docs/introduction/quickstart.md)
- [Documentation](https://aci.dev/docs/api-reference/overview.md)
- [Documentation](https://aci.dev/docs/api-reference/openapi.json)
- [Documentation](https://aci.dev/docs/sdk/intro.md)
- [Documentation](https://aci.dev/docs/sdk/custom-functions.md)
- [Documentation](https://aci.dev/docs/mcp-servers/introduction)
- [Documentation](https://aci.dev/docs/agent-playground/introduction.md)
- [Documentation](https://aci.dev/docs/advanced/oauth2-whitelabel.md)
- [Documentation](https://aci.dev/docs/llms.txt)
- [GitHub Organization](https://github.com/aipotheosis-labs)
- [Source Code](https://github.com/aipotheosis-labs/aci)
- [Source Code](https://github.com/aipotheosis-labs/aci-mcp)
- [Source Code](https://github.com/aipotheosis-labs/aci-mcp-node)
- [SDK](https://github.com/aipotheosis-labs/aci-python-sdk)
- [SDK](https://github.com/aipotheosis-labs/aci-typescript-sdk)
- [Source Code](https://github.com/aipotheosis-labs/aci-agents)
- [Source Code](https://github.com/aipotheosis-labs/aci-developer-docs)
- [Source Code](https://github.com/aipotheosis-labs/gate22)
- [Source Code](https://github.com/aipotheosis-labs/gate22-docs)
- [Documentation](https://platform.aci.dev)
- [Documentation](https://discord.gg/nnqFSzq2ne)
- [LinkedIn](https://www.linkedin.com/company/aipotheosis-labs-aipolabs)
- [Twitter](https://twitter.com/AipoLabs)
- [Documentation](https://www.youtube.com/@AipotheosisLabs)
- [License](https://www.apache.org/licenses/LICENSE-2.0)
- [Features](undefined)
- [Integrations](undefined)
- [Vocabulary](vocabulary/aci-dev-vocabulary.yml)
- [Spectral Rules](rules/aci-dev-rules.yml)
- [JSON-LD](json-ld/aci-dev-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
