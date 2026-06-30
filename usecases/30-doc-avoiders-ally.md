# Doc-Avoider's Ally

## Persona
Developer who would rather ship ten features than write one docstring, yet keeps getting PRs rejected with "where's the documentation?"

## The Problem They Have
They skip docstrings with sincere intentions of "doing it later" — leading to perpetual PR rejections, confused teammates, and a growing reputation as the person who makes the docs team cry.

## The NanoClaw Setup
- Scans every commit for new or modified public functions, classes, and endpoints that lack docstrings
- Auto-generates stub documentation from type annotations, function signatures, and inline comments
- Opens a draft PR titled "Add missing docs for [function]" — dev just reviews and approves, not writes
- Sends a Telegram nudge when the draft is ready with a one-line summary of what was auto-generated

## Sample Telegram Interaction
> **Agent:** `processOrder()` has no docstring. Draft:
> `"""Process a customer order, validate inventory, charge payment. Returns bool."""`
> **Dev:** Close enough, open a PR.
> **Agent:** PR #387 opened. One click to merge. You're welcome. 📝

## Why It's a Digital Twin
It embodies your desire to avoid doc work entirely — a lazy-but-thorough scribe that keeps the codebase documented without stealing a minute of coding time.
