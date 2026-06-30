# NanoClaw vs AutoGen / AG2

> **Type:** Conversational multi-agent framework (microsoft/autogen is legacy; AG2 is the active successor)
> **Source:** [github.com/ag2ai/ag2](https://github.com/ag2ai/ag2) · [github.com/microsoft/autogen](https://github.com/microsoft/autogen)

---

## What is AutoGen / AG2?

AutoGen was Microsoft Research's open-source conversational multi-agent framework. When Microsoft placed the original repo (microsoft/autogen) into maintenance-only mode, the original authors immediately forked it as **AG2** (github.com/ag2ai/ag2), which remains actively developed. If you're evaluating "AutoGen" in 2026, you're almost certainly looking at AG2 — not the legacy Microsoft repo. AG2 supports multiple LLMs and retains the AutoGen Studio experimental visual builder.

---

## The Honest Comparison

| Dimension | NanoClaw | AG2 (AutoGen active successor) |
|-----------|----------|-------------------------------|
| Language & runtime | Node.js / TypeScript, needs Docker | Python; lightweight processes or threads |
| License | MIT | Apache-2.0 |
| LLM support | Claude only (Anthropic SDK) | LLM-agnostic — Azure OpenAI, OpenAI, HuggingFace, local |
| Deployment | One Docker container per agent | Standard Python processes; no container required |
| UI / interaction | Telegram-native (cards, questions, reactions) | AutoGen Studio (experimental visual builder) + console/CLI |
| Memory persistence | CLAUDE.local.md — editable Markdown, Git-versionable | In-memory conversation history; external storage via plugins |
| Proactivity | schedule_task with bash pre-checks; sub-agent spawning built-in | Must be coded manually; no native scheduling primitives |
| Credential handling | OneCLI transparent proxy | Developer-managed env vars and vaults |
| Resource overhead | ~100–200 MB per container | Lightweight Python processes |
| Development status | Active | Active (AG2); microsoft/autogen is legacy/unmaintained |
| Community | Small, growing | Larger; community split between legacy and AG2 |

---

## Where NanoClaw Wins

- Proactive design built-in: scheduling with pre-checks and sub-agent spawning without boilerplate
- OneCLI proxy keeps secrets out of agent code without extra vault plumbing
- Persistent Markdown memory enables version control and manual inspection
- Docker isolation provides strong per-agent security boundaries
- Telegram-native UI with no frontend build required

## Where AG2 Wins

- **LLM-agnostic** — use Azure OpenAI, local models, or anything OpenAI-compatible; not locked to Anthropic pricing
- **Visual tooling** — AutoGen Studio provides an experimental visual builder for defining agent workflows; NanoClaw has no equivalent
- **Lower resource overhead** — process-based agents vs container-per-agent; far cheaper at scale
- **Conversational multi-agent patterns** — group chat, consensus-building, and sequential agent dialogues are first-class; NanoClaw's sub-agents are more task-dispatch than conversation
- **No Telegram requirement** — flexible integration with any UI or platform

---

## Verdict

**NanoClaw** for Telegram-native proactive workflows, transparent credential handling, and Node.js/TypeScript comfort. **AG2** if you need LLM flexibility, Python ecosystem, lower runtime overhead, or conversational multi-agent patterns. If evaluating this space, target the AG2 fork — not the legacy Microsoft repo.

*Sources: [github.com/ag2ai/ag2](https://github.com/ag2ai/ag2) · [github.com/microsoft/autogen](https://github.com/microsoft/autogen) · [DataCamp](https://www.datacamp.com/tutorial/crewai-vs-langgraph-vs-autogen)*
