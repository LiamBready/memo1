# Agent Inception

## Persona
Developer building AI agents for their own company -- running a fleet of NanoClaw agents in production and needing someone to watch the watchers.

## The Problem They Have
One agent goes rogue at 3am, burns through the API budget, and nobody notices until the invoice arrives. The fleet is powerful but unattended.

## The NanoClaw Setup
- Sends a daily health digest per container: uptime, API calls, error rate, cost estimate
- Spawns a diagnostic sub-agent on error spikes before they cascade
- Surfaces caching opportunities from usage patterns ("agent-X calls the same endpoint 40 times a day")
- Throttles rogue agents before they eat the budget, wakes you only if human judgment is needed

## Sample Telegram Interaction
> **Agent:** Fleet health: 6 agents healthy, 1 elevated error rate (openrouter, 12% errors). Spawning diagnostic. Budget: 73% of daily limit used by 2pm -- recommend throttling researcher until tomorrow.
> **Dev:** Throttle it.
> **Agent:** Done. You built a good fleet.
> **Dev:** Thanks for watching them.
> **Agent:** That is what agents are for.

## Why It's a Digital Twin
It closes the loop -- the agent that watches all the other agents, so the system stays sane even when you are not looking.
