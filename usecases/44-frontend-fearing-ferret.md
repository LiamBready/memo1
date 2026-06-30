# Frontend-Fearing Ferret

## Persona
Backend developer who is very good at systems and very allergic to CSS, who nonetheless has to review frontend PRs because the team is small.

## The Problem They Have
They approve frontend PRs with zero idea if they actually work, secretly scared of the day something breaks in Safari and everyone figures out they just clicked "approve."

## The NanoClaw Setup
- Auto-runs ESLint + Stylelint on new frontend PRs and reports in plain English ("this button is invisible on mobile")
- Schedules "I'll look at this later" reminders with pre-chewed MDN docs for the specific CSS in the PR
- Visual-diffs staging vs main for pixel regressions so nothing changes invisibly
- Sends a Friday frontend digest in backend-friendly language: "3 PRs, 0 regressions, 1 flex-wrap issue fixed"

## Sample Telegram Interaction
> **Agent:** PR #55: no lint errors, no visual regressions, one unused CSS variable. Safe to approve without touching a single semicolon.
> **Dev:** This is what courage feels like.
> **Agent:** You were brave today.

## Why It's a Digital Twin
It translates the frontend into a language backend engineers can actually act on.
