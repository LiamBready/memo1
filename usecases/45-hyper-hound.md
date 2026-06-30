# Hyper-Hound

## Persona
Developer with ADHD who has incredible hyperfocus sessions followed by complete inability to remember what they were doing or why the branch is called "fix-thing-maybe."

## The Problem They Have
Great ideas disappear between Telegram and the editor, hyperfocus commits become 800-line PRs nobody can review, and the evening is full of ideas that will definitely still seem important tomorrow (they won't).

## The NanoClaw Setup
- Captures every #idea and TODO from Telegram to memory with branch context so nothing evaporates
- Nudges after 90-minute idle stretches ("you went quiet — still on the auth thing?")
- Auto-summarizes big hyperfocus commits into PR templates: what changed, why, how to test
- Converts the evening idea log into real GitHub issues before sleep so future-you has something actionable

## Sample Telegram Interaction
> **Agent:** You've been quiet for 2h. Last active: auth/jwt.py. Still on that?
> **Dev:** No I went down a rabbit hole about caching. I have 400 lines of changes.
> **Agent:** PR #84 opened: "Cache JWT in localStorage — reduces login latency ~120ms." Linked your original idea note. Want me to break it up?
> **Dev:** Yes please. 🐶

## Why It's a Digital Twin
It holds the context you lose so the ideas survive the context switch.
