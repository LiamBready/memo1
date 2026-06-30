# Did You Know? — NanoClaw Facts (Batch 3, #11–15)

---
**Did you know? #11 — USB-C for Your AI Brain**

NanoClaw agents can plug into any MCP (Model Context Protocol) server — filesystem, GitHub, Slack, databases, or a custom tool you write yourself — just like sticking a USB-C dongle into a laptop. Because MCP is a standard protocol, the agent's core code never needs to change; you simply add new ports to expand its toolkit.

*Source: NanoClaw docs*

---
**Did you know? #12 — The Night Guard Who Only Gets Up When Needed**

When you use schedule_task, NanoClaw first runs a bash pre-check script; if it returns wakeAgent: false, the agent stays asleep and skips the LLM call entirely. Think of it as a security guard who glances at the camera feed before deciding whether to leave their chair — the agent is always watching, but only acts when something genuinely warrants it.

*Source: workshop repo README*

---
**Did you know? #13 — The Spaceship Bridge That Needs Two Officers to Fire**

The ncl admin CLI lets you inspect and modify live agent configuration — destinations, members, MCP servers, installed packages — without restarting the system. Every write command flows through an approval step so nothing changes silently, like a starship bridge console that requires a second officer to confirm before firing the photon torpedoes.

*Source: proactive-digital-twin-workshop exercises*

---
**Did you know? #14 — The Polite Coworker Who Actually Waits for Your Click**

With send_card and ask_user_question, an agent can render a real UI card in Telegram and then pause its entire turn until you tap a button — it genuinely cannot proceed until you've responded. No more AI that assumes your intent; this is the considerate coworker who won't book the meeting room until you've clicked "approve" rather than just nodding vaguely.

*Source: NanoClaw docs*

---
**Did you know? #15 — The Conductor Who Summons Extra Musicians Mid-Show**

NanoClaw agents can spawn sub-agents on the fly — a Researcher doing a deep web search, a Builder editing code in the background, a Reviewer checking the output — each a full standalone NanoClaw agent in its own container. It's like a conductor who, mid-performance, summons an entire orchestra section to handle the crescendo while keeping the melody going themselves.

*Source: general AI agent research*
