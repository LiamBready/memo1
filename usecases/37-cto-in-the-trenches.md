# CTO-in-the-Trenches

## Persona
Startup CTO who still codes but also runs investor calls, does hiring, and somehow has to review PRs before 9am.

## The Problem They Have
Deep work sessions get shredded by Slack, context-switching kills flow, and the team's PRs wait days because the CTO is always "in a meeting."

## The NanoClaw Setup
- Creates focus-block calendar events on "deep work" mentions and protects them from meeting invites
- Nudges stale PRs after 2h inactivity with a friendly "this one's blocking Alice"
- Sends a break reminder after 4h continuous coding (yes, CTOs need this)
- Spawns a sub-agent to summarize the day's commits into a one-liner for the weekly investor update

## Sample Telegram Interaction
> **Agent:** Focus block protected: 10am-12pm. PR #42 is blocking Alice's deploy — 3h unreviewed.
> **CTO:** On it. Also what did we ship today?
> **Agent:** Auth refactor merged, two bug fixes, one new endpoint. One sentence: "Hardened auth and shipped payment webhook." You're welcome.

## Why It's a Digital Twin
It's the co-founder who handles the meta-work so you can stay in the code.
