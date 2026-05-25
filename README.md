# ACI.dev (aci-dev)

ACI.dev (Aipolabs Agent-Computer Interface) is an open-source tool-calling platform that hooks AI agents into 600+ pre-built tools through direct function calling or a unified Model Context Protocol (MCP) server. Maintained by Aipotheosis Labs (Aipolabs) under Apache 2.0. The sister project Gate22 adds an open-source MCP gateway and control plane for governed agent tool-use across Cursor and other agentic IDEs.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/aci-dev/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=opensource-api-evangelist&utm_content=repo)

## Tags

 - Agent Infrastructure, Agents, AI, Artificial Intelligence, Function Calling, MCP, Model Context Protocol, OAuth, Open Source, Tool Calling, VibeOps

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## Project

| Field | Value |
|---|---|
| Project type | Open source |
| Operator | Aipotheosis Labs (Aipolabs) |
| License | Apache 2.0 |
| Primary languages | Python, TypeScript |
| Primary repo | [aipotheosis-labs/aci](https://github.com/aipotheosis-labs/aci) |
| MCP server | [aipotheosis-labs/aci-mcp](https://github.com/aipotheosis-labs/aci-mcp) |
| Gateway / control plane | [aipotheosis-labs/gate22](https://github.com/aipotheosis-labs/gate22) |
| API base URL | `https://api.aci.dev` |
| Authentication | `X-API-KEY` header (issued from `platform.aci.dev`) |
| Authoritative OpenAPI | [aci.dev/docs/api-reference/openapi.json](https://aci.dev/docs/api-reference/openapi.json) |

## APIs

### ACI.dev Apps API
Search and inspect the 600+ pre-built Apps in the ACI.dev catalog. Apps are external service integrations (Slack, Gmail, Zendesk, GitHub, Notion, Stripe, ...) that expose Functions for AI agents to call.

**Human URL:** [https://aci.dev/docs/core-concepts/app.md](https://aci.dev/docs/core-concepts/app.md)

- [Documentation — App concept](https://aci.dev/docs/core-concepts/app.md)
- [Documentation — Search Apps](https://aci.dev/docs/api-reference/apps/search-apps.md)
- [Documentation — Get App Details](https://aci.dev/docs/api-reference/apps/get-app-details.md)
- [OpenAPI](openapi/aci-dev-openapi.yml)
- [JSON Schema — App](json-schema/aci-dev-app-schema.json)
- [JSON Schema — App With Functions](json-schema/aci-dev-app-with-functions-schema.json)
- [Naftiko Capability — Apps](capabilities/apps.yaml)

### ACI.dev Functions API
Search, inspect, and execute the callable Functions (tools) exposed by configured Apps. The same surface backs the unified MCP server's `ACI_SEARCH_FUNCTIONS` and `ACI_EXECUTE_FUNCTION` meta-tools.

**Human URL:** [https://aci.dev/docs/core-concepts/function.md](https://aci.dev/docs/core-concepts/function.md)

- [Documentation — Function concept](https://aci.dev/docs/core-concepts/function.md)
- [Documentation — Search Functions](https://aci.dev/docs/api-reference/functions/search-functions.md)
- [Documentation — Get Function Definition](https://aci.dev/docs/api-reference/functions/get-function-definition.md)
- [Documentation — Execute](https://aci.dev/docs/api-reference/functions/execute.md)
- [OpenAPI](openapi/aci-dev-openapi.yml)
- [JSON Schema — Function](json-schema/aci-dev-function-schema.json)
- [JSON Schema — Function Execute](json-schema/aci-dev-function-execute-schema.json)
- [JSON Schema — Function Execution Result](json-schema/aci-dev-function-execution-result-schema.json)
- [JSON Schema — OpenAI Function Definition](json-schema/aci-dev-openai-function-definition-schema.json)
- [JSON Schema — Anthropic Function Definition](json-schema/aci-dev-anthropic-function-definition-schema.json)
- [Example — Search Functions](examples/aci-dev-search-functions-example.json)
- [Example — Execute Function](examples/aci-dev-execute-function-example.json)
- [Naftiko Capability — Functions](capabilities/functions.yaml)

### ACI.dev App Configurations API
Create and manage per-project App Configurations. An App Configuration declares which App is enabled, which security scheme it should use (OAuth2, API key, or no-auth), which functions are permitted, and any security-scheme overrides.

**Human URL:** [https://aci.dev/docs/core-concepts/app-configuration.md](https://aci.dev/docs/core-concepts/app-configuration.md)

- [Documentation — App Configuration concept](https://aci.dev/docs/core-concepts/app-configuration.md)
- [OpenAPI](openapi/aci-dev-openapi.yml)
- [JSON Schema — App Configuration](json-schema/aci-dev-app-configuration-schema.json)
- [Naftiko Capability — App Configurations](capabilities/app-configurations.yaml)

### ACI.dev Linked Accounts API
Manage end-user Linked Accounts for configured Apps. Initiate an OAuth2 link flow, handle the OAuth2 callback, list and retrieve linked accounts by owner ID, and revoke a Linked Account. White-label OAuth2 is supported.

**Human URL:** [https://aci.dev/docs/core-concepts/linked-account.md](https://aci.dev/docs/core-concepts/linked-account.md)

- [Documentation — Linked Account concept](https://aci.dev/docs/core-concepts/linked-account.md)
- [Documentation — Link OAuth2 Account](https://aci.dev/docs/api-reference/linked-accounts/link-oauth2-account.md)
- [Documentation — OAuth2 Callback](https://aci.dev/docs/api-reference/linked-accounts/linked-accounts-oauth2-callback.md)
- [Documentation — White-label OAuth2](https://aci.dev/docs/advanced/oauth2-whitelabel.md)
- [OpenAPI](openapi/aci-dev-openapi.yml)
- [JSON Schema — Linked Account](json-schema/aci-dev-linked-account-schema.json)
- [Example — Link OAuth2 Account](examples/aci-dev-link-oauth2-account-example.json)
- [Naftiko Capability — Linked Accounts](capabilities/linked-accounts.yaml)

## Ecosystem repositories (aipotheosis-labs)

| Repo | Purpose |
|---|---|
| [aci](https://github.com/aipotheosis-labs/aci) | Open-source tool-calling platform — backend, frontend portal, SDKs |
| [aci-mcp](https://github.com/aipotheosis-labs/aci-mcp) | Python MCP server (unified + apps modes) |
| [aci-mcp-node](https://github.com/aipotheosis-labs/aci-mcp-node) | TypeScript/Node port of aci-mcp |
| [aci-python-sdk](https://github.com/aipotheosis-labs/aci-python-sdk) | Official Python SDK |
| [aci-typescript-sdk](https://github.com/aipotheosis-labs/aci-typescript-sdk) | Official TypeScript SDK |
| [aci-agents](https://github.com/aipotheosis-labs/aci-agents) | Example agents built on ACI.dev |
| [aci-developer-docs](https://github.com/aipotheosis-labs/aci-developer-docs) | Developer documentation source |
| [gate22](https://github.com/aipotheosis-labs/gate22) | Open-source MCP gateway and control plane |
| [gate22-docs](https://github.com/aipotheosis-labs/gate22-docs) | Gate22 documentation |

## Common

- [Portal — aci.dev](https://aci.dev)
- [Documentation — aci.dev/docs](https://aci.dev/docs)
- [Getting Started](https://aci.dev/docs/introduction/quickstart.md)
- [API Reference Overview](https://aci.dev/docs/api-reference/overview.md)
- [Authoritative OpenAPI](https://aci.dev/docs/api-reference/openapi.json)
- [SDK Introduction](https://aci.dev/docs/sdk/intro.md)
- [Custom Functions SDK](https://aci.dev/docs/sdk/custom-functions.md)
- [MCP Servers Introduction](https://aci.dev/docs/mcp-servers/introduction)
- [Agent Playground](https://aci.dev/docs/agent-playground/introduction.md)
- [llms.txt Documentation Index](https://aci.dev/docs/llms.txt)
- [Platform Console — platform.aci.dev](https://platform.aci.dev)
- [Aipolabs on X (@AipoLabs)](https://twitter.com/AipoLabs)
- [Aipolabs on LinkedIn](https://www.linkedin.com/company/aipotheosis-labs-aipolabs)
- [Aipolabs Discord](https://discord.gg/nnqFSzq2ne)
- [Aipotheosis Labs on YouTube](https://www.youtube.com/@AipotheosisLabs)

## Features

- 600+ pre-built App integrations (Slack, Gmail, Zendesk, GitHub, Notion, Stripe, ...)
- Unified MCP server (`aci-mcp`) exposing `ACI_SEARCH_FUNCTIONS` and `ACI_EXECUTE_FUNCTION` meta-tools
- Apps MCP mode that surfaces a specific set of Apps as named MCP tools
- Node port (`aci-mcp-node`) for TypeScript-native MCP integration
- OpenAI-compatible and Anthropic-compatible function-definition output formats
- Multi-tenant end-user OAuth2 link flow, white-label OAuth2 for production branding
- Per-project App Configurations with function-level enable/disable and security-scheme overrides
- Natural-language permission filters that guardrail tool executions
- Custom Functions SDK for registering proprietary tools alongside the catalog
- Agent Playground for prompting against the unified catalog before production wiring
- Python and TypeScript SDKs (`aci-python-sdk`, `aci-typescript-sdk`)
- Sister project `gate22` — open-source MCP gateway and control plane for governance and audit across Cursor and other agentic IDEs
- Self-hostable backend, frontend portal, and SDKs under Apache 2.0

## Integrations

- Anthropic Claude (function definitions returned in Anthropic tool-use format)
- OpenAI (function definitions returned in OpenAI tool-use format)
- Model Context Protocol — Cursor, Claude Desktop, Claude Code, and other MCP clients
- GitHub, Gmail, Slack, Zendesk, Notion, Stripe, and 600+ other apps via the ACI catalog

## Artifacts in this repository

- `apis.yml` — APIs.json 0.16 profile for ACI.dev
- `openapi/aci-dev-openapi.yml` — Mirrored authoritative OpenAPI 3.1 spec, title-cased
- `json-schema/` — Extracted JSON Schemas for App, Function, FunctionExecute, FunctionExecutionResult, App Configuration, Linked Account, OpenAI and Anthropic function-definition shapes
- `json-ld/aci-dev-context.jsonld` — JSON-LD context for ACI.dev resources
- `capabilities/` — Naftiko 1.0.0-alpha2 capabilities for Apps, Functions, App Configurations, and Linked Accounts
- `rules/aci-dev-rules.yml` — Spectral ruleset enforcing ACI.dev conventions on the OpenAPI spec
- `vocabulary/aci-dev-vocabulary.yml` — Domain vocabulary covering ACI concepts, tools, integrations, and governance terms
- `examples/` — Request/response examples for Search Functions, Execute Function, and Link OAuth2 Account

## Maintainers

- Kin Lane — [API Evangelist](https://apievangelist.com) — `@apievangelist`
