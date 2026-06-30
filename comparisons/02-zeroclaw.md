# NanoClaw vs ZeroClaw

> **Type:** Open-source AI agent framework (Rust, privacy-first, edge-focused)
> **Source:** [github.com/zeroclaw-labs/zeroclaw](https://github.com/zeroclaw-labs/zeroclaw) · [zeroclaw.bot](https://zeroclaw.bot/)

---

## What is ZeroClaw?

ZeroClaw is a Rust-based autonomous AI agent runtime distributed as a single static binary. It targets edge devices, air-gapped environments, and scenarios where any cloud dependency is off-limits. Licensed Apache-2.0, it supports 30+ messaging channels, 20+ LLM providers (Anthropic, OpenAI, Ollama, any OpenAI-compatible endpoint), and provider fallback chains — all via config. As of June 2026 it has 32,100 GitHub stars.

---

## The Honest Comparison

| Dimension | NanoClaw | ZeroClaw |
|-----------|----------|----------|
| Language & runtime | Node.js / TypeScript, needs Docker | Rust — single static binary, zero runtime deps |
| License | MIT | Apache-2.0 |
| Deployment | One Docker container per agent | Single binary, runs directly on host OS |
| UI / comms | Telegram-native (cards, reactions, questions) | 30+ channels via config — Telegram, Discord, Matrix, email, webhooks, CLI |
| Memory | CLAUDE.local.md (plain Markdown, human-readable) | Embedded configurable storage |
| LLM coupling | Tightly coupled to Anthropic Claude SDK | Provider-agnostic — Anthropic, OpenAI, Ollama, 20+ providers; fallback chains |
| Resource footprint | ~100–200 MB per container + Node runtime | 3.4 MB binary, runs on Raspberry Pi-class hardware |
| Air-gap suitability | ❌ Needs Telegram API + Docker | ✅ Fully offline capable with local LLMs |
| Pricing | Self-hosted costs only | Free binary; pay only for LLM API usage |
| Community | Small but growing | 32k GitHub stars, active |

---

## Where NanoClaw Wins

- Telegram-native UI with send_card, ask_user_question, add_reaction built in — zero custom frontend
- OneCLI credential proxy — secrets never in agent code, no vault setup required
- Version-controlled Markdown memory auditable by any team member
- MCP server support + install_packages for extending capabilities
- Admin CLI (ncl) for live config changes with approval flow

## Where ZeroClaw Wins

- **True offline / air-gap** — works with local Ollama, no Telegram, no Docker Hub, no external anything
- **Minimal footprint** — 3.4 MB binary boots in under 10ms, runs on constrained hardware
- **LLM provider flexibility** — 20+ providers, fallback chains, swap via config not code
- **No container overhead** — share one process across agents; far cheaper at scale
- **30+ channel support** — broader than NanoClaw out of the box (Discord, Matrix, email, voice, webhooks)

---

## Verdict

**NanoClaw** for Telegram-centric proactive agents with Node.js and Claude at the core, where Docker is already part of the stack. **ZeroClaw** for edge hardware, air-gapped deployments, multi-channel breadth, or anywhere "no runtime dependencies" is a hard requirement.

*Sources: [github.com/zeroclaw-labs/zeroclaw](https://github.com/zeroclaw-labs/zeroclaw) · [lushbinary.com](https://lushbinary.com/blog/zeroclaw-openclaw-personal-ai-agents-compared-2026/) · [DEV Community](https://dev.to/wonderlab/open-source-project-of-the-day-part-26-zeroclaw-full-rust-autonomous-ai-assistant-7e0)*
