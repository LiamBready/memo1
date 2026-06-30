# Meta-Manager Mimic

## Persona
Engineering manager juggling standups, retros, hiring panels, and stakeholder updates while trying to keep five engineers unblocked simultaneously.

## The Problem They Have
Blockers scatter across Jira, Slack, and email and are forgotten until a deadline looms — at which point three people have been stuck for a week and nobody said anything.

## The NanoClaw Setup
- Aggregates open tickets, Slack threads, and calendar events into a unified blocker board, updated in real time
- Sends a daily digest each morning: blockers, owners, ETAs, and who hasn't updated their ticket in >24h
- Nudges assignees with friendly reminders and escalates if there's no movement after 24 hours
- Runs anonymous pulse polls after retros and saves team sentiment to memory over time

## Sample Telegram Interaction
> **Manager:** What's blocking the team today?
> **Agent:** 3 blockers: auth timeout (Alice, ETA Fri), missing feature-flag docs (Bob, ETA Thu), flaky test suite (Carol, investigating). Ping Alice?
> **Manager:** Yes.
> **Agent:** Done. I'll follow up if no update by 18:00.

## Why It's a Digital Twin
It mirrors your need for situational awareness — a proactive chief of staff who never lets a blocker slip.
