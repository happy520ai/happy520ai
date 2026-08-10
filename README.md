# Jiongjiong Chen | Open-Source AI Infrastructure

I build terminal-first infrastructure for models, agents, knowledge, and tools,
with explicit human control at every real-provider boundary.

陈炯炯，正在构建开放、终端优先、可治理，并始终由人掌握最终控制权的 AI 基础设施。

## Featured Project: Unified AI System

[Unified AI System](https://github.com/happy520ai/unified-ai-system) is an
Apache-2.0 self-hosted AI gateway and MCP server for Codex, Cursor, Cline, CLI,
HTTP, and SDK workflows. It turns rough natural-language requests into
structured, reviewable prompts before execution.

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
  <a href="https://registry.modelcontextprotocol.io/v0.1/servers/io.github.happy520ai%2Funified-ai-system/versions/0.4.8">
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

Verify the published container with visible evidence:

```bash
docker run --rm ghcr.io/happy520ai/unified-ai-system/ai-gateway-service:0.4.8 pnpm gateway demo "Build a small API for my team" --enhance --profile coding --evidence
```

### Why It Matters

- Plain-language requests become inspectable execution, output, and completion requirements.
- Nine governed MCP tools expose prompt enhancement, health, readiness, local chat, knowledge, workflows, and workforce status.
- The credential-free fake provider is the default; real-provider calls require explicit enablement and authorization.
- Public CI verifies source checks, tests, containers, MCP discovery, clean-clone startup, and process cleanup.

### Use It With Codex

Install the repository plugin:

```bash
codex plugin marketplace add happy520ai/unified-ai-system --ref master
```

Or connect the pinned MCP container:

```bash
codex mcp add unified-ai-system -- docker run --rm -i ghcr.io/happy520ai/unified-ai-system/mcp-server:0.4.8
```

[Project site](https://happy520ai.github.io/unified-ai-system/) |
[60-second Codex guide](https://happy520ai.github.io/unified-ai-system/codex-mcp-docker-quickstart.html) |
[Release v0.4.8](https://github.com/happy520ai/unified-ai-system/releases/tag/v0.4.8) |
[Good first issues](https://github.com/happy520ai/unified-ai-system/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)

If the project saves setup time or gives an agent workflow a safer gateway,
[star the repository](https://github.com/happy520ai/unified-ai-system)
so more developers can discover and verify it.

Unified AI System is an engineering preview. Production readiness, L5 autonomy,
and AGI are not claimed without independent evidence.
