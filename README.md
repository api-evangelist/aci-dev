# ACI.dev (aci-dev)

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
