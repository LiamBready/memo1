# GitLab Merge Watcher

## Persona
Technical lead who gets pinged at 2 AM because a feature branch fell 30 commits behind main and caused a pipeline explosion.

## The Problem They Have
MRs sit idle for days, then suddenly conflict with a hot-fix, turning CI into a fireworks display of red logs and angry Slack messages.

## The NanoClaw Setup
- Watches all open MRs and calculates a "staleness score" based on age and diverging commits
- If an MR hasn't been updated in 12h and main has moved, messages the author: "Your MR is 5 commits behind — want a rebase?"
- Attempts auto-rebase and reports the outcome with a diff snippet
- After a successful merge, logs it and sends a celebratory message to the team channel

## Sample Telegram Interaction
> **Agent:** 🔔 MR #1423 (auth-refactor) is 18h old; main advanced 5 commits.
> **Lead:** I forgot about that one.
> **Agent:** 🔧 Auto-rebase succeeded. Diff: +12/−4. Ready to review.
> **Lead:** Merging.
> **Agent:** Pipeline green. 🎉

## Why It's a Digital Twin
It behaves like a vigilant co-lead who never sleeps, keeping the merge pipeline clean before you notice the drift.
