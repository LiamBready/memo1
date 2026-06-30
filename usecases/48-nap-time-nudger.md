# Nap-Time Nudger

## Persona
Developer who is also a parent of a small child -- coding in stolen 45-minute windows between naps, feeding, and everything else that is now life.

## The Problem They Have
By the time they open the IDE, context is gone, setup takes 10 minutes, the baby wakes up after 20, and nothing actually ships.

## The NanoClaw Setup
- Monitors baby nap start and immediately surfaces a micro-task that fits the exact window
- Pre-creates a branch and opens the right file so setup time is zero
- Auto-pushes a WIP commit when crying is detected so the mental handoff is clean and resumable
- Sends a 9pm recap: "you shipped X today" -- because parent-devs need to hear it

## Sample Telegram Interaction
> **Agent:** Nap started. Estimated 40 min. Branch ready, test failing on line 84 -- that is your task. Go.
> **Dev:** [20 min later] crying
> **Agent:** WIP commit pushed. "Fixed auth check, needs test." You will pick it up next nap. Go be a parent. You shipped something today.

## Why It's a Digital Twin
It compresses the context switch so every stolen window actually counts.
