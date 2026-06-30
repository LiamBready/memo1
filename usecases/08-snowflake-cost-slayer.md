# Snowflake Cost Slayer

## Persona
Data engineer who wakes up to a Snowflake bill that looks like a small country's GDP and has no idea which query caused it.

## The Problem They Have
Ad-hoc queries run wild scanning terabytes while the team's credit balance dwindles faster than coffee during a sprint deadline.

## The NanoClaw Setup
- Monitors Snowflake query history via account usage schema, flags queries exceeding a cost threshold
- Messages the query owner with the query text, estimated credit cost, and a concrete optimization suggestion
- If the same user offends three times in a day, creates a GitHub/GitLab issue and assigns it to them
- Posts a daily cost summary at midnight and trends over time in memory

## Sample Telegram Interaction
> **Agent:** 💸 @sam: `SELECT * FROM events` ran 42 min, cost ≈ 12 credits.
> **Sam:** I was just checking timestamps.
> **Agent:** Add `WHERE date = CURRENT_DATE()` — cuts scans 90%. Re-run?
> **Sam:** Done.
> **Agent:** ✅ New cost: 0.8 credits. That's the spirit.

## Why It's a Digital Twin
It mirrors your cost-consciousness and intervenes before the bill lands.
