# Side-Project Squirrel

## Persona
Indie hacker running 3+ products simultaneously — each at a different stage, each with its own repo, each quietly demanding attention.

## The Problem They Have
One product gets all the focus, two others atrophy, and the "I'll get back to it" pile grows until a user tweets that the free tier is broken and has been for a month.

## The NanoClaw Setup
- Nightly cross-repo dashboard in memory: issues open, last commit, user activity, anything on fire
- Proactive nudges on idle branches after 48h ("project-b hasn't been touched in 3 days")
- Per-commit lint/test sub-agent so CI doesn't become a surprise
- Nightly priority suggestion based on issue weight and self-imposed deadlines

## Sample Telegram Interaction
> **Agent:** Nightly report: project-a healthy, project-b has 2 open bug reports + idle 4 days, project-c has a failing test from Tuesday.
> **Hacker:** Fix the test in project-c and open issues for the bugs in project-b.
> **Agent:** Branch created. Issues filed. 🐿

## Why It's a Digital Twin
It gives every project a heartbeat even when you can only be in one place at a time.
