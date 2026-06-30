# Did You Know? — NanoClaw Facts (Batch 2, #6–10)

---
**Did you know? #6 — The Valet Who Never Asks for the Keys**

NanoClaw's OneCLI transparent proxy sits between your agent and any external API — Gmail, GitHub, Slack, Stripe — quietly slipping in the real credentials just before the request leaves the container. The agent itself never sees, stores, or even knows what those secrets look like, much like a valet who knows exactly which key to grab without you having to point.

*Source: [What is NanoClaw? — docs.nanoclaw.dev](https://docs.nanoclaw.dev/introduction)*

---
**Did you know? #7 — Elephant Memory vs Goldfish Brain**

Unlike stateless LLM calls that forget everything the moment the context window closes, NanoClaw companion agents persist their thoughts in CLAUDE.local.md, accumulating context over weeks and months across restarts and reboots. They remember your preferred coding style, open tickets, and that weird inside joke you made last Tuesday — think elephant, not goldfish.

*Source: [NanoClaw Tutorial: Build a Lightweight Local-First Agent — DataCamp](https://www.datacamp.com/tutorial/nanoclaw-tutorial)*

---
**Did you know? #8 — Brew Your Own AI Espresso**

NanoClaw is MIT-licensed, self-hostable on any machine, with zero vendor lock-in and zero usage fees — you can read every line of code that's thinking on your behalf. It's the difference between building your own espresso machine (you know exactly what's in the cup) versus a pod subscription that quietly decides what you're allowed to taste.

*Source: [nanocoai/nanoclaw — GitHub](https://github.com/nanocoai/nanoclaw)*

---
**Did you know? #9 — Every Agent Gets Its Own Office**

Each NanoClaw agent lives in its own Docker container with an isolated workspace, memory slice, and filesystem, so one agent's experiments can't accidentally overwrite another's notes or corrupt shared state. It's like giving every developer their own private office instead of forcing them to hot-desk on a chaotic open-plan floor where someone keeps stealing the good monitor.

*Source: [Don't Trust AI Agents, Says OpenClaw's Security-First Alternative, NanoClaw — Forbes](https://www.forbes.com/sites/gilpress/2026/03/13/dont-trust-ai-agents-says-nanoclaw-now-fully-integrated-with-docker/)*

---
**Did you know? #10 — Junior Developer With a Very Good Calculator**

Powered by Claude via the Anthropic Agent SDK, NanoClaw agents aren't glorified chatbots — they invoke tools, spin up sub-agents, call MCP servers, and reason across long contexts. Think the difference between a calculator and a junior developer who also happens to own a calculator: one answers your question, the other figures out what question you should have asked.

*Source: [nanocoai/nanoclaw — GitHub](https://github.com/nanocoai/nanoclaw)*
