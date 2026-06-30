# NanoClaw vs Nanobot

> **Type:** Open-source Python AI agent framework (MCP-native, minimal)
> **Source:** [github.com/HKUDS/nanobot](https://github.com/HKUDS/nanobot) · [nanobot.club](https://nanobot.club/)

---

## What is Nanobot?

Nanobot is an ultra-lightweight open-source personal AI agent from the Data Intelligence Lab at the University of Hong Kong (HKUDS), released February 2, 2026. It delivers core agent functionality in ~4,000 lines of Python — MCP-native from the ground up, supporting 11+ LLM providers (OpenRouter, Anthropic, OpenAI, DeepSeek, Gemini, and more) and 8+ messaging platforms including Telegram, Discord, WhatsApp, Slack, and email.

---

## The Honest Comparison

| Dimension | NanoClaw | Nanobot |
|-----------|----------|---------|
| Language & runtime | Node.js / TypeScript, needs Docker | Pure Python, no external SDK dependency |
| License | MIT | MIT |
| Communication / UI | Telegram-native (cards, reactions, questions) | 8+ platforms: Telegram, Discord, WhatsApp, Slack, email, Feishu, DingTalk |
| Memory persistence | CLAUDE.local.md — editable, Git-friendly Markdown | Built-in memory; configurable persistence |
| Proactivity | schedule_task with bash pre-checks; sub-agent spawning | Automation management built-in; task scheduling |
| Credential handling | OneCLI transparent proxy — secrets never in agent code | Manual injection via env vars or config files |
| LLM support | Claude only (Anthropic SDK) | 11+ providers including OpenRouter, DeepSeek, Gemini, Ollama |
| Codebase size | Larger opinionated harness (Node.js) | ~4,000 lines Python — readable in an afternoon |
| Resource footprint | ~100–200 MB per container | Single Python process; no container overhead |

---

## Where NanoClaw Wins

- OneCLI credential proxy — secrets never in agent code; no manual env var management
- Version-controlled Markdown memory auditable by any team member
- send_card, ask_user_question, add_reaction interactive primitives ready-made
- Docker-per-agent provides strong OS-level security isolation
- Admin CLI (ncl) + MCP server support + install_packages for structured extensibility

## Where Nanobot Wins

- **LLM flexibility** — 11+ providers including free options (DeepSeek, local Ollama); not locked to Anthropic pricing
- **Lightweight deployment** — Python process, no Docker overhead; large fleets are far cheaper
- **Broader channel support** — 8+ messaging platforms natively including non-Western apps (Feishu, DingTalk, QQ)
- **Readability** — ~4k LOC Python core you can understand in an afternoon
- **MCP-native** — MCP support is first-class, not bolted on

---

## Verdict

**NanoClaw** for feature-rich proactive agents with secure credential handling and Telegram-first interaction, where Claude is the preferred model. **Nanobot** when you want a lightweight, multi-provider, MCP-native baseline you can deploy at scale without container overhead — or when your audience is on non-Western messaging platforms.

*Sources: [github.com/HKUDS/nanobot](https://github.com/HKUDS/nanobot) · [nanobot.club](https://nanobot.club/) · [BrightCoding](https://www.blog.brightcoding.dev/2026/05/10/nanobot-the-revolutionary-lightweight-ai-assistant)*
