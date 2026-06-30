# Freelancer Gig Guardian

## Persona
Freelance AI engineers juggling multiple clients, invoices, and shifting deadlines who need a relentless sidekick to keep chaos in check.

## The Problem They Have
They double-book meetings, forget to invoice after milestones, and lose track of scope creep until the client sends a mildly annoyed email at midnight.

## The NanoClaw Setup
- Scans messages for project keywords ("deliverable", "deadline", "invoice") and creates calendar events automatically
- Auto-generates an invoice draft when a git tag `release/vX.Y` is pushed — ready to send with one tap
- Sends a scope-creep alert if a client asks for features outside the current milestone board
- Tracks time per client and warns when approaching budgeted hours

## Sample Telegram Interaction
> **You:** Client just asked for "real-time sentiment analysis" on top of the chatbot.
> **Agent:** ⚠️ Scope creep — adds ~8h. Update estimate or push back?
> **You:** Let's discuss tomorrow.
> **Agent:** Blocked a 10am slot and drafted a change-order email for your review.

## Why It's a Digital Twin
It learns your work patterns and acts like a proactive PM who only nudges when it matters.
