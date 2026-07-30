# Building Unified AI System

Open, terminal-first infrastructure for models, governed agents, knowledge,
tools, and human-controlled automation.

正在构建开放、终端优先、可治理，并始终由人掌握最终控制权的 AI 基础设施。

## Unified AI System

[Unified AI System](https://github.com/happy520ai/unified-ai-system) is an open,
local-first gateway for multi-model routing, governed agents, knowledge, tools,
approvals, and observable automation.

<a href="https://github.com/happy520ai/unified-ai-system">
  <img
    src="https://raw.githubusercontent.com/happy520ai/unified-ai-system/master/docs/assets/terminal-demo.png"
    alt="Unified AI System credential-free terminal demo"
    width="100%"
  />
</a>

<p align="center">
  <a href="https://github.com/happy520ai/unified-ai-system"><strong>Try the terminal CLI</strong></a>
  ·
  <a href="https://github.com/happy520ai/unified-ai-system/releases/tag/v0.2.0">v0.2.0 Release</a>
  ·
  <a href="https://github.com/happy520ai/unified-ai-system/issues?q=is%3Aissue%20is%3Aopen%20label%3A%22good%20first%20issue%22">Contribute</a>
</p>

```bash
git clone --branch v0.2.0 --depth 1 https://github.com/happy520ai/unified-ai-system.git
cd unified-ai-system
corepack enable
corepack prepare pnpm@9.15.4 --activate
pnpm install --frozen-lockfile
pnpm gateway demo
```

- Credential-free first run through a deterministic local fake provider.
- Terminal CLI for demo, startup, status, chat, and diagnostics.
- Multi-model gateway, agent, knowledge, approval, and evidence modules.
- Chat refuses real-provider execution without explicit command authorization.
- Apache-2.0, public GHCR image, Linux CI, and clean-clone verification.

[README](https://github.com/happy520ai/unified-ai-system#readme)
|
[简体中文](https://github.com/happy520ai/unified-ai-system/blob/master/README.zh-CN.md)
|
[Roadmap](https://github.com/happy520ai/unified-ai-system/blob/master/ROADMAP.md)
|
[v0.2.0](https://github.com/happy520ai/unified-ai-system/releases/tag/v0.2.0)

Public preview. Production readiness, L5 autonomy, and AGI require evidence
beyond repository tests.
