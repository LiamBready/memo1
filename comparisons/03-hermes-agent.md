# NanoClaw vs Hermes Agent

> **Type:** Self-improving open-source AI agent framework
> **Source:** [github.com/NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) · [hermes-agent.nousresearch.com/docs](https://hermes-agent.nousresearch.com/docs/)

---

## What is Hermes Agent?

Hermes Agent is Nous Research's MIT-licensed open-source AI agent framework, released February 25, 2026. It became the fastest-growing agent framework of 2026, reaching 95,600 GitHub stars in seven weeks. Its defining feature is a self-improvement loop: after completing a task, a reflection module extracts a reusable skill and writes it to disk. Future similar tasks pull that skill without an API call, with internal benchmarks showing a 40% reduction in tokens and time for repeat tasks after 20+ accumulated skills.

---

## The Honest Comparison

| Dimension | NanoClaw | Hermes Agent |
|-----------|----------|--------------|
| Language & runtime | Node.js / TypeScript, needs Docker | Python; runs as a persistent daemon |
| License | MIT | MIT |
| Core focus | General-purpose proactive agent framework | Self-improving agents with automated skill accumulation |
| LLM coupling | Tightly coupled to Anthropic Claude SDK | LLM-agnostic — Anthropic, OpenAI, local, 16+ integrations |
| Deployment | One Docker container per agent | Single persistent process; containerization optional |
| UI / interaction | Telegram-native (cards, reactions, questions) | 16+ messaging platforms; no prescribed primary channel |
| Memory | CLAUDE.local.md — editable, versionable Markdown | Three-layer memory + self-written skills in ~/.hermes/skills/ |
| Proactivity | schedule_task with bash pre-checks; sub-agent spawning | Scheduled cron tasks; proactivity via skill-driven efficiency gains |
| Community | Small, growing | 95k+ GitHub stars; fastest-growing agent framework of 2026 |

---

## Where NanoClaw Wins

- Editable, version-controllable Markdown memory any team member can audit and change directly
- OneCLI credential proxy keeps secrets completely out of agent code
- Admin CLI (ncl) and install_packages for operational extensibility
- Docker isolation provides strong per-agent security boundaries
- send_card, ask_user_question, add_reaction primitives ready out of the box

## Where Hermes Agent Wins

- **Self-improvement loop** — agent refines its own skills from experience; repeat tasks get 40% cheaper over time
- **LLM-agnostic** — swap models without rewriting logic; not locked to Anthropic pricing or availability
- **Much larger community** — 95k stars vs NanoClaw's growing but modest audience
- **Broader channel support** — 16+ messaging platforms natively
- **No container overhead** — daemon-based, lighter for single deployments

---

## Verdict

**NanoClaw** for production-lean, extensible deployment with transparent ops, Telegram-first UI, and Claude at the core. **Hermes Agent** if you want an agent that genuinely improves itself through use and aren't locked to a single LLM provider.

*Sources: [github.com/NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) · [hermes-agent.nousresearch.com](https://hermes-agent.nousresearch.com/docs/) · [tokenmix.ai review](https://tokenmix.ai/blog/hermes-agent-review-self-improving-open-source-2026)*
