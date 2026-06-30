# Open Source Maintainer's Lifeline

## Persona
Open-source maintainers drowning in issues, stale PRs, and the eternal quest to label "good first issue" for newcomers.

## The Problem They Have
Issues pile up faster than they can triage, PRs sit untouched for weeks, and potential contributors get lost — leading to burnout and slower releases.

## The NanoClaw Setup
- Watches the issue stream and auto-labels new items as bug/feature/question, posts a daily triage digest
- Sends a list of PRs older than 3 days without reviews, tagging likely reviewers based on recent commits
- Spawns a sub-agent that welcomes newcomers on "good first issue" items with a starter guide
- Generates a weekly maintainer mood report: dancing panda when you close >10 issues, screaming goat otherwise

## Sample Telegram Interaction
> **Agent:** 3 new issues: #422 (auth timeout), #423 (export to CSV), #424 (deploy question). Labeled, drafted starter comment for #424. PR #417 is 5 days without review — ping @alice?
> **You:** Yes please.

## Why It's a Digital Twin
It replicates your triage instincts and nudges contributors like a co-maintainer who never needs coffee.
