# The On-Call Therapist

## Persona
For the backend engineer whose phone anxiety is now clinically indistinguishable from being on-call — because they always are.

## The Problem They Have
PagerDuty wakes them at 3 AM, they spend 40 minutes finding the runbook, fix the thing, write nothing down, and repeat the exact same incident four months later.

## The NanoClaw Setup
- Monitors PagerDuty/OpsGenie alerts and correlates with service dashboards and recent deploys
- On alert, immediately sends a context package: last deploy, similar past incidents, relevant runbook section
- After resolution, prompts for a two-sentence post-mortem while details are fresh
- Maintains an incident memory so future alerts include "this happened before, here is what fixed it"

## Sample Telegram Interaction
> **Agent (3:17 AM):** payment-service is paging. Last deploy 47 min ago (Miguel, config change). Similar incident Nov 12 — DB connection pool exhaustion, fixed by bumping MAX_POOL_SIZE. Runbook section 4.2.
>
> Go fix it. I'll be here.
>
> *[22 min later]*
>
> **Agent:** Glad you're alive. Two sentences on what happened while it's fresh? I'll write the incident doc.

## Why It's a Digital Twin
It remembers every incident you've forgotten and uses that memory to make the next one shorter.
