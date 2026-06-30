# The Slide Sherpa

## Persona
Conference speaker prepping talks, juggling demo rehearsals, last-minute slide tweaks, and travel chaos across three time zones.

## The Problem They Have
They forget to update demo API keys, rehearse once at 80% speed, and discover the laptop battery is at 4% thirty seconds before taking the stage.

## The NanoClaw Setup
- Watches the speaker's repo for slide and demo changes, warns if any demo endpoint returns non-200 or uses credentials older than 30 days
- Sends a full-rehearsal reminder 24h before each talk with a checklist: slides, demo, clicker, adapters
- Posts a funny countdown in the final hour with a motivational GIF (intensity scales with time remaining)
- Spawns a sub-agent to generate a backup "slides-went-nuclear" deck filled with relevant cat pictures, just in case

## Sample Telegram Interaction
> **Agent:** ⚠️ Your live demo hits `api.example.com/v2` but it returned 401. Did you rotate the key?
> **Speaker:** Oops. Regenerate and push.
> **Agent:** Done. Also: 18h to showtime — have you run the full demo yet? Rehearsal set for 8pm. 🦸

## Why It's a Digital Twin
It mirrors your speaker instincts and keeps you stage-ready without the last-minute panic spiral.
