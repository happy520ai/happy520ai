# Building Open AI Infrastructure

Open, terminal-first infrastructure for models, agents, knowledge, and tools,
with explicit human control at every real-provider boundary.

正在构建开放、终端优先、可治理，并始终由人掌握最终控制权的 AI 基础设施。

## Unified AI System

[Unified AI System](https://github.com/happy520ai/unified-ai-system) turns rough
natural-language requests into structured work through a self-hosted AI gateway,
terminal CLI, HTTP API, shared SDK, and nine tested MCP tools for Codex and other
compatible clients.

**No account. No API key. One Docker command.**

<p>
  <a href="https://github.com/happy520ai/unified-ai-system/actions/workflows/ci.yml">
    <img alt="CI" src="https://github.com/happy520ai/unified-ai-system/actions/workflows/ci.yml/badge.svg?branch=master" />
  </a>
  <a href="https://registry.modelcontextprotocol.io/v0.1/servers/io.github.happy520ai%2Funified-ai-system/versions/0.4.0">
    <img alt="Official MCP Registry" src="https://img.shields.io/badge/Official_MCP_Registry-active-1f883d" />
  </a>
  <a href="https://github.com/happy520ai/unified-ai-system/blob/master/LICENSE">
    <img alt="Apache-2.0" src="https://img.shields.io/badge/license-Apache--2.0-blue" />
  </a>
</p>

<a href="https://github.com/happy520ai/unified-ai-system">
  <img
    src="https://raw.githubusercontent.com/happy520ai/unified-ai-system/master/docs/assets/terminal-demo.png"
    alt="Unified AI System credential-free terminal demo"
    width="100%"
  />
</a>

### Try The Gateway

```bash
docker run --rm ghcr.io/happy520ai/unified-ai-system/ai-gateway-service:0.4.0 pnpm gateway demo
```

### Install The Codex Plugin

```bash
codex plugin marketplace add happy520ai/unified-ai-system --ref master
```

### Connect Codex Through MCP

```bash
codex mcp add unified-ai-system -- docker run --rm -i ghcr.io/happy520ai/unified-ai-system/mcp-server:0.4.0
```

- Deterministic, credential-free fake provider for the default first run.
- Terminal commands for demo, prompt enhancement, serve, status, chat, and diagnostics.
- Nine MCP tools covering provider-free prompt enhancement, readiness, local
  chat, knowledge, workflows, and workforce status.
- Real-provider chat fails closed without explicit command authorization.
- Public multi-architecture containers, Linux CI, and clean-clone verification.

<p>
  <a href="https://github.com/happy520ai/unified-ai-system"><strong>Explore the project</strong></a>
  ·
  <a href="https://github.com/happy520ai/unified-ai-system/blob/master/docs/codex-mcp-quickstart.md">60-second Codex guide</a>
  ·
  <a href="https://github.com/happy520ai/unified-ai-system/releases/tag/v0.4.0">v0.4.0</a>
  ·
  <a href="https://github.com/happy520ai/unified-ai-system/issues?q=is%3Aissue%20is%3Aopen%20label%3A%22good%20first%20issue%22">Contribute</a>
</p>

If the project saves you setup time or gives your agents a safer gateway,
consider giving it a star. It helps more developers find the work.

Public preview. Production readiness, L5 autonomy, and AGI require independent
evidence beyond repository tests.
