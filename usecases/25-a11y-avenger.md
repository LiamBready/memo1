# A11y Avenger

## Persona
Accessibility engineer on a mission to catch inclusivity bugs before they reach users and cause angry tweets.

## The Problem They Have
Design reviews keep missing contrast failures, ARIA labels, and keyboard traps — leading to costly post-launch rework and a legal team asking uncomfortable questions.

## The NanoClaw Setup
- Runs `axe-core` on the built UI on every PR and posts violation comments with concrete fixes
- Maintains a living accessibility score (0–100) in memory with weekly trend digest
- If score drops below 80, spawns a sub-agent that records a 15s screen-capture of the failing component and posts it
- Suggests specific fixes ("contrast ratio → 4.5:1, use #2A2A2A") not just "fix this"

## Sample Telegram Interaction
> **Agent:** 🚨 PR #88: "Submit" button contrast 2.1:1 (fails WCAG AA). Fix: change bg to `#004080`.
> **You:** Done.
> **Agent:** Fix verified. Score: 92/100 — still green. 💚

## Why It's a Digital Twin
It internalizes your accessibility expertise and guards the inclusive experience 24/7 so you never catch the same slip twice.
