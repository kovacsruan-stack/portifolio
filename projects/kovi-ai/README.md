# KOVI AI — Intelligence & Orchestration

**Principal project:** https://github.com/kovacsruan-stack/kovi-ai

KOVI AI is the intelligence layer of the KOVIAN ecosystem. It demonstrates how an AI system can combine model-provider abstraction, authorization, tools, memory, RAG, telemetry and domain integrations without giving the model unrestricted authority.

## Technical highlights

- Multi-provider model abstraction
- Provider routing and fallback
- Tool calling with explicit contracts
- RBAC and workspace isolation
- API keys, scopes and rotation
- Semantic memory and RAG
- Embedding lifecycle/versioning
- Idempotency
- Rate limiting
- Usage and cost telemetry
- Audit logging
- OpenAPI
- Governed domain-tool federation
- Fitness context integration
- Local Chromium/Playwright QA

## Architecture

```text
Client
  ↓
KOVI API
  ↓
Authentication / Workspace / RBAC
  ↓
Orchestrator
  ↓
Provider Router
  ├── Cloud providers
  ├── Free-capable providers
  └── Local OpenAI-compatible provider
  ↓
Tools / Memory / RAG
  ↓
Usage / Cost / Audit
  ↓
Response
```

## Security boundary

The model is not trusted for authorization.

A model-generated tool call is treated as an **intent**, while the application Tool Executor validates authorization, inputs, scopes and confirmation requirements before execution.

Domain products remain the source of truth for their data.

## Stack

TypeScript · Node.js · PostgreSQL/Supabase · pgvector · Vitest · Playwright · Docker

## Evidence

- [Original README](https://github.com/kovacsruan-stack/kovi-ai/blob/main/README.md)
- [Architecture](https://github.com/kovacsruan-stack/kovi-ai/blob/main/ARCHITECTURE.md)
- [Security policy](https://github.com/kovacsruan-stack/kovi-ai/blob/main/SECURITY.md)
