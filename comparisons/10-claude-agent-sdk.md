# NanoClaw vs Claude Agent SDK (Anthropic raw SDK)

> **Type:** Opinionated harness vs raw SDK — both built on the same foundation
> **Source:** [github.com/anthropics/anthropic-sdk-python](https://github.com/anthropics/anthropic-sdk-python) · [github.com/anthropics/anthropic-sdk-typescript](https://github.com/anthropics/anthropic-sdk-typescript) · [sdk.anthropic.com](https://sdk.anthropic.com)

---

## What is the Claude Agent SDK?

The Anthropic Claude Agent SDK is the official library for building agents that interact with Claude models, available in Python and TypeScript. It provides core primitives — prompting, tool use, context management — and leaves UI, persistence, scheduling, and orchestration entirely to the developer. NanoClaw is built on top of it: the SDK is the engine, NanoClaw is the car.

---

## The Honest Comparison

| Dimension | NanoClaw | Claude Agent SDK (raw) |
|-----------|----------|------------------------|
| Language | Node.js / TypeScript | TypeScript or Python — your choice |
| Abstraction level | Opinionated harness — batteries included | Thin wrapper — you wire everything yourself |
| UI / interaction | Telegram-native, built-in | None — choose HTTP, CLI, WebSocket, whatever you want |
| Memory persistence | CLAUDE.local.md auto-managed, editable, Git-friendly | None — design your own storage from scratch |
| Proactivity | schedule_task with bash pre-checks; sub-agent spawning | Reactive only; you build scheduling and sub-agents manually |
| Credential handling | OneCLI transparent proxy — secrets never in agent code | You manage API keys directly in code or env vars |
| Deployment | One Docker container per agent | Wherever your process runs — no container enforced |
| Resource footprint | Higher — Docker overhead per agent | Minimal — just the SDK process |
| Extensibility | Admin CLI (ncl), MCP servers, install_packages | Your own code — no standard plugin system |
| Testing / CI | Harder — Docker + Telegram required for integration tests | Easy to unit-test in isolation; no external dependencies needed |
| Vendor lock-in | Infrastructure: none; Models: Claude only | Models: Claude only; no additional framework lock-in |

---

## Where NanoClaw Wins

- Telegram UI, persistent memory, scheduling, credential proxy, and sub-agent spawning all included — zero boilerplate
- send_card, ask_user_question, add_reaction make human-in-the-loop interactions trivial
- OneCLI proxy keeps secrets out of agent code, a real security gain
- Faster time-to-working-agent for solo developers and small teams

## Where the Raw SDK Wins

- **No container overhead** — ideal for high-scale deployments or embedding in existing services
- **Full UI freedom** — not Telegram-locked; build a web app, Slack bot, REST API, anything
- **No forced conventions** — use your own storage, your own deployment, your own patterns
- **Simpler to embed** — one install (`npm install @anthropic-ai/sdk` or `pip install anthropic`) and go
- **Testable in isolation** — unit-test agent logic without Docker or Telegram; NanoClaw's full stack makes CI setup significantly heavier
- **No Telegram requirement** — critical for enterprise, web-facing, or headless deployments

---

## Verdict

**NanoClaw** when you want a working proactive agent with UI, memory, and credential handling in minutes and are happy with Telegram + Docker as the runtime. **Raw Claude Agent SDK** when you need maximum flexibility, lower overhead, easier testability, or a custom UI/persistence layer — and are prepared to build those pieces yourself.

*Sources: [github.com/anthropics/anthropic-sdk-python](https://github.com/anthropics/anthropic-sdk-python) · [github.com/anthropics/anthropic-sdk-typescript](https://github.com/anthropics/anthropic-sdk-typescript) · [docs.anthropic.com](https://docs.anthropic.com/claude/docs/agents) · [morphllm.com](https://www.morphllm.com/ai-agent-framework)*
