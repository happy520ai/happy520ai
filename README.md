# Jiongjiong Chen | Open-Source AI Infrastructure

I build terminal-first infrastructure for models, agents, knowledge, and tools,
with explicit human control at every real-provider boundary.

陈炯炯，正在构建开放、终端优先、可治理，并始终由人掌握最终控制权的 AI 基础设施。

## Featured Project: Unified AI System

[Unified AI System](https://github.com/happy520ai/unified-ai-system) is an
Apache-2.0 **self-hosted AI gateway** for OpenAI-compatible SDKs, MCP, A2A,
CLI, and HTTP workflows — with the feature set you'd expect from a commercial
LLM gateway: virtual keys with token budgets, exact + semantic response caching,
reverse MCP governance (any OpenAPI 3 spec becomes governed MCP tools), and
chat-native Prometheus/Langfuse observability.

<p>
  <a href="https://github.com/happy520ai/unified-ai-system">
    <img alt="GitHub stars" src="https://img.shields.io/github/stars/happy520ai/unified-ai-system?style=flat-square&amp;label=Stars" />
  </a>
  <a href="https://github.com/happy520ai/unified-ai-system/actions/workflows/ci.yml">
    <img alt="CI" src="https://img.shields.io/github/actions/workflow/status/happy520ai/unified-ai-system/ci.yml?branch=master&amp;style=flat-square&amp;label=CI" />
  </a>
  <a href="https://github.com/happy520ai/unified-ai-system/releases/latest">
    <img alt="Latest release" src="https://img.shields.io/github/v/release/happy520ai/unified-ai-system?style=flat-square" />
  </a>
  <a href="https://registry.modelcontextprotocol.io/v0.1/servers/io.github.happy520ai%2Funified-ai-system/versions/0.5.0">
    <img alt="Official MCP Registry: active" src="https://img.shields.io/badge/Official_MCP_Registry-active-1f883d?style=flat-square" />
  </a>
  <a href="https://github.com/happy520ai/unified-ai-system/blob/master/LICENSE">
    <img alt="Apache-2.0 license" src="https://img.shields.io/github/license/happy520ai/unified-ai-system?style=flat-square" />
  </a>
</p>

<a href="https://happy520ai.github.io/unified-ai-system/#enhance?prompt=Build+a+small+API+for+my+team&amp;profile=coding&amp;language=en">
  <img
    src="https://raw.githubusercontent.com/happy520ai/unified-ai-system/master/docs/assets/prompt-enhancement-demo.png"
    alt="Unified AI System turns a rough request into a structured coding prompt"
    width="100%"
  />
</a>

### Try It Without Installing

[Open a ready-to-run prompt-enhancement example](https://happy520ai.github.io/unified-ai-system/#enhance?prompt=Build+a+small+API+for+my+team&profile=coding&language=en).
It runs locally in the browser with no account, API key, or provider call.

Or run the full gateway in 60 seconds — no clone, no credentials:

```bash
docker run --rm ghcr.io/happy520ai/unified-ai-system/ai-gateway-service:0.5.0 pnpm gateway demo "Build a small API for my team" --enhance --profile coding
```

### Why It Matters

- Virtual keys (`uai-`) with daily/monthly token budgets, per-key rate limits,
  soft-budget alerts, spend attribution, and instant revocation — consumers
  never hold provider keys.
- Exact + semantic response cache on the chat hot path with byte-identical
  SSE replay and per-tenant isolation.
- Reverse MCP governance: aggregate upstream MCP servers (HTTP + stdio) behind
  one authenticated, audited, allow-listed surface; REST→MCP from any OpenAPI
  3 spec.
- The credential-free fake provider is the default; real-provider calls
  require explicit three-gate enablement and authorization.
- A repeatable 16-attack live security regression (cross-tenant cache reads,
  tenant forgery, budget bypass...) must stay green for every release.

### Use It With Codex

Install the repository plugin:

```bash
codex plugin marketplace add happy520ai/unified-ai-system --ref master
```

Or connect the pinned MCP container:

```bash
codex mcp add unified-ai-system -- docker run --rm -i ghcr.io/happy520ai/unified-ai-system/mcp-server:0.5.0
```

[Project site](https://happy520ai.github.io/unified-ai-system/) |
[中文 README](https://github.com/happy520ai/unified-ai-system/blob/master/README.zh-CN.md) |
[Release v0.5.0](https://github.com/happy520ai/unified-ai-system/releases/tag/v0.5.0) |
[Good first issues](https://github.com/happy520ai/unified-ai-system/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)

If the project saves setup time or gives an agent workflow a safer gateway,
[star the repository](https://github.com/happy520ai/unified-ai-system)
so more developers can discover and verify it.

Unified AI System is an engineering preview. Production readiness, L5 autonomy,
and AGI are not claimed without independent evidence.
