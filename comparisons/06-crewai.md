# NanoClaw vs CrewAI

> **Type:** Open-source Python framework for role-based multi-agent teams
> **Source:** [github.com/joaomdmoura/crewAI](https://github.com/joaomdmoura/crewAI) · [crewai.com](https://www.crewai.com)

---

## What is CrewAI?

CrewAI is a popular Python framework for building teams of AI agents, each defined by a role, goal, and backstory. Agents collaborate as a "crew" to accomplish complex tasks — think of it as casting characters for a play and letting them improvise toward a goal. It has a large community, an active open-source core, and a commercial enterprise edition with SLAs.

---

## The Honest Comparison

| Dimension | NanoClaw | CrewAI |
|-----------|----------|--------|
| LLM support | Claude only (Anthropic SDK) | Framework-agnostic — OpenAI, Anthropic, local models, etc. |
| Deployment | One Docker container per agent | Standard Python processes; containerization optional |
| UI / interaction | Telegram-native (cards, questions, reactions) | No built-in chat UI — must build your own |
| Memory & state | CLAUDE.local.md — plain Markdown, Git-versionable | Short-term task context; persistent memory requires custom implementation |
| Proactivity | schedule_task with bash pre-checks; dynamic sub-agent spawning | Reactive by default; proactive scheduling requires custom code |
| Credential handling | OneCLI transparent proxy | Manual — env vars or secrets manager |
| Community | Small, growing | Very large; abundant examples and tutorials |
| Commercial offering | MIT only | MIT core + commercial enterprise edition |
| Scale / resource use | Container-per-agent is heavy at scale | Lightweight processes; much easier to scale large fleets |

---

## Where NanoClaw Wins

- Proactive design: scheduling with bash pre-checks and sub-agent spawning without extra plumbing
- OneCLI credential proxy — secrets never appear in agent code
- Persistent, human-readable Markdown memory — diff and audit with Git
- Telegram-first UI with send_card, ask_user_question, add_reaction ready out of the box
- Self-hostable with strong per-agent Docker isolation enforced at OS level

## Where CrewAI Wins

- **LLM flexibility** — use any model; not locked to Claude pricing or availability
- **Community and ecosystem** — vastly larger; more examples, plugins, and StackOverflow answers
- **Scale efficiency** — process-based agents are far cheaper to run at scale than a container per agent
- **No UI lock-in** — embed into web apps, Slack bots, internal dashboards freely
- **Commercial support** — enterprise edition with SLAs for production-critical deployments

---

## Verdict

**NanoClaw** for self-hosted, Telegram-centric, proactive agents with secure credential handling and Claude at the core. **CrewAI** when you need LLM flexibility, a battle-tested large community, lower runtime costs at scale, and freedom to build any UI.

*Sources: [github.com/joaomdmoura/crewAI](https://github.com/joaomdmoura/crewAI) · [DataCamp](https://www.datacamp.com/tutorial/crewai-vs-langgraph-vs-autogen) · [pecollective.com](https://pecollective.com/blog/ai-agent-frameworks-compared/)*
