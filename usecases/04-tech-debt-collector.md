# The Technical Debt Collector

## Persona
For the tech lead who has spent three years saying "we'll clean that up next sprint" and now runs a codebase that is 40% TODO comments and ambient guilt.

## The Problem They Have
Tech debt exists in their head as a formless dread rather than an actionable list, which means it grows faster than it shrinks because you cannot prioritize a feeling.

## The NanoClaw Setup
- Weekly scans the repo for TODO/FIXME/HACK comments, tracks them over time, reports the delta
- Pulls PR review comments flagged as "should refactor" into a backlog with author and date
- Cross-references backlog against sprint planning and flags items that keep getting skipped
- Sends a monthly "debt aging report" sorted by how many times items have been punted

## Sample Telegram Interaction
> **Agent (Monday, 8:30 AM):** Weekly debt report.
> TODOs: 847 (up 12 from last week — three of them are yours from Thursday).
> Oldest unaddressed: `// FIXME: this will break with timezones` — added by you, February 2023. Still true.
> You skipped the auth module cleanup for the 7th consecutive sprint. I am not judging. I am only counting.

## Why It's a Digital Twin
It is the part of you that actually remembers all the promises you made to the codebase.
