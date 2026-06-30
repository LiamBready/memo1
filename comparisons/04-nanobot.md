# NanoClaw vs Nanobot

> **Type:** Open-source Python AI agent framework (MCP-native, minimal)
> **Source:** [github.com/hku-ai/nanobot](https://github.com/hku-ai/nanobot) · [composio.dev](https://composio.dev/content/openclaw-alternatives)

---

## What is Nanobot?

Nanobot is a minimal (~4,000 lines) open-source Python agent framework from the Data Intelligence Lab at the University of Hong Kong (HKUDS), released February 2026 and growing to over 9,000 GitHub stars. It is MCP-native from the ground up, with a focus on readability, ease of extension, and keeping the codebase small enough to actually understand without a week of archaeology.

---

## The Honest Comparison

| Dimension | NanoClaw | Nanobot |
|-----------|----------|---------|
| Language & Runtime | Node.js + Anthropic Claude SDK, needs Docker | Pure Python, no external SDK dependency |
| Communication / UI | Telegram-native | Internal message bus; optional HTTP/WebSocket adapters |
| Memory persistence | CLAUDE.local.md — editable, Git-friendly Markdown | In-memory JSON store with optional file-based persistence plugin |
| Proactivity | schedule_task with bash pre-checks; dynamic sub-agent spawning | Basic task scheduler; no built-in sub-agent spawning |
| Credential handling | OneCLI transparent proxy — secrets never in agent code | Manual injection via env vars or config files |
| Resource footprint | One Docker container per agent | Single-process lightweight agents, no container overhead |
| LLM coupling | Tightly coupled to Claude/Anthropic SDK | SDK-agnostic; only standard Python libraries |
| Codebase size | Larger opinionated harness | ~4k LOC — readable and auditable in an afternoon |
| Community | Small but growing | Academic-origin; 9k GitHub stars, sparse docs |

---

## Where NanoClaw Wins

- Rich interaction toolkit: send_card, ask_user_question, add_reaction ready-made
- Advanced proactive features and sub-agent spawning out of the box
- OneCLI proxy for zero-secret-in-code security
- Version-controllable Markdown memory — diff, branch, audit with Git
- Docker isolation enforced at OS level, not application level

## Where Nanobot Wins

- **Lightweight deployment** — ordinary Python processes; no per-agent Docker overhead; large fleets are far cheaper
- **SDK independence** — MCP-native and LLM-agnostic; swap models via config, not code
- **Readability** — ~4k LOC core you can audit in an afternoon (NanoClaw's harness adds more)
- **Lower barrier for non-Telegram teams** — generic HTTP/WebSocket adapters fit any environment
- **Minimal dependencies** — faster startup, simpler debugging, easier CI

---

## Verdict

**NanoClaw** for feature-rich proactive agents with secure credential handling in Docker/Telegram environments. **Nanobot** when you want a lightweight, MCP-native, SDK-agnostic baseline you can read cover-to-cover and deploy at scale without container overhead.

*Sources: [github.com/hku-ai/nanobot](https://github.com/hku-ai/nanobot) · [composio.dev](https://composio.dev/content/openclaw-alternatives) · [aimastery.page](https://www.aimastery.page/articles/openclaw-alternatives)*
