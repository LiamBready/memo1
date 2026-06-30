# Junior Dev Buddy

## Persona
Junior developers eager to contribute but often lost in large codebases, unsure when to ask for help.

## The Problem They Have
They spend hours on cryptic error messages, fall into rabbit holes, and hesitate to ping seniors for fear of looking clueless.

## The NanoClaw Setup
- Monitors git activity and flags when they've been stuck on the same file >30 min, suggesting relevant docs or similar closed issues
- Schedules a daily learning nudge at 10am ("Today's tip: use `git bisect` to find regressions")
- Spawns a sub-agent that drafts a polite question template when they fail the same test three times in a row
- Sends a weekly PR activity summary with encouragement and next-step recommendations

## Sample Telegram Interaction
> **Agent:** You've been touching `auth/service.py` for 45 min. Want a hint?
> **You:** Sure!
> **Agent:** Add `logging.debug` before JWT validation — logs show a missing `aud` claim.
> **You:** Thanks! 🙌

## Why It's a Digital Twin
It mirrors your coding habits, anticipates blockers, and gives senior-mentor guidance without you having to ask.
