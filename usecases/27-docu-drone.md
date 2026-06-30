# Docu-Drone: The Write-Stuff Bot

## Persona
Technical writer tasked with keeping API guides, tutorials, and release notes in sync with a codebase that changes faster than they can type.

## The Problem They Have
They constantly forget to update docs after each merge, leading to outdated references, confused users, and an inbox full of "this page is wrong" tickets.

## The NanoClaw Setup
- Watches the repo for changes to OpenAPI/Swagger files and source annotations that affect public-facing docs
- Auto-generates draft markdown sections using templates calibrated to the team's writing style
- Opens a PR with doc changes and tags the writer for review — no chasing required
- Sends a Telegram summary of what changed, what was drafted, and any gaps it couldn't fill

## Sample Telegram Interaction
> **Agent:** New endpoint `/v2/payments/webhook` detected. Draft ready in PR #142 — 3 sections added, 1 example generated.
> **Writer:** Looks good, merge it.
> **Agent:** Merged. Docs live at /v2/payments. ✍️

## Why It's a Digital Twin
It embodies your drive to keep docs fresh — an editorial assistant that never misses a code change.
