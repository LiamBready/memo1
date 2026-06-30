# Roadmap Ronin: The Feature Prioritization Ninja

## Persona
Product manager constantly juggling stakeholder wishes, OKRs, and a perpetually out-of-date roadmap nobody trusts.

## The Problem They Have
Stakeholders keep slipping in "just one quick feature" and you forget to update the roadmap, leading to endless "but I thought we agreed on…" pings.

## The NanoClaw Setup
- Listens to a dedicated Telegram channel for feature requests and scores each one (impact, effort, strategic fit)
- Updates a living roadmap in CLAUDE.local.md and auto-creates a Jira issue when score exceeds the priority threshold
- Sends a "Roadmap Pulse" every Monday with changes, new entries, and what shipped last week
- Triggers a backlog-grooming sub-agent when the priority list shifts by more than 20%

## Sample Telegram Interaction
> **Stakeholder:** Can we add dark mode by Friday?
> **Agent:** Scored: Impact 8, Effort 5, Fit 7 → P2. Added to roadmap, Jira DSP-1027 created. Appears in Monday's pulse.

## Why It's a Digital Twin
It captures your product intuition and keeps the plan current so you never have to chase the roadmap yourself.
