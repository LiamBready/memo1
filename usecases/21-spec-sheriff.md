# Spec Sheriff: The OpenAPI Enforcer

## Persona
API designer who lives and dies by OpenAPI YAML and hates when spec drift sneaks in between releases.

## The Problem They Have
Team members keep adding or renaming endpoints without updating the spec, turning every integration test into a surprise party gone very wrong.

## The NanoClaw Setup
- Watches GitHub PRs for changes to API source files and runs `openapi-validator` automatically
- Posts a diff summary to Telegram with a "breaking change" or "additive change" verdict
- Auto-generates a mock server link for quick manual testing, suggests a version bump on breaking changes
- Spawns a sub-agent to update markdown API docs so docs are never a separate chore

## Sample Telegram Interaction
> **Agent:** 🚨 PR #142 adds `/v2/users/{id}` but spec still only has `/v1/users`. Breaking change detected.
> **You:** Auto-bump to v2.0.0 and open a docs PR.
> **Agent:** Done. Mock server ready. Crisis averted. 🤠

## Why It's a Digital Twin
It mirrors your design intent and enforces spec fidelity before anyone else notices the drift.
