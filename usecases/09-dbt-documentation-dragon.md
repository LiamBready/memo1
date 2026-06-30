# The dbt Documentation Dragon

## Persona
CTO of a data startup who loves dbt models but hates chasing down outdated schema docs when onboarding new analysts.

## The Problem They Have
The docs site lags behind the dbt project by weeks. New hires file "where is this field?" tickets and the answer is always "ask someone who was there."

## The NanoClaw Setup
- Hooks into dbt run completion and parses manifest.json for new or changed models and columns
- Drafts a documentation PR with descriptions, test coverage, and lineage — named "🦖 Dragon Update"
- If the PR sits idle for 6h, pings the model owner on Telegram
- On merge, posts "Docs are fire-breathing fresh" and logs the changelog entry

## Sample Telegram Interaction
> **Agent:** 📜 dbt run done. New model `fct_user_engagement` — 3 undocumented columns.
> **Dev:** I'll add descriptions later.
> **Agent:** (2h later) 🦖 Still no docs. Draft PR ready — want to merge it?
> **Dev:** Looks good, merging.
> **Agent:** Dragon satisfied. 🔥

## Why It's a Digital Twin
It embodies the CTO's desire for accurate docs — sprouting updates the moment the code changes.
