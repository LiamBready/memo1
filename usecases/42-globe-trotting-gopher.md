# Globe-Trotting Gopher

## Persona
Developer advocate who travels constantly — three conferences a month, five time zones, one laptop, and one prayer that the hotel Wi-Fi holds.

## The Problem They Have
Demo containers go stale on the flight, hotel Wi-Fi dies at the worst moment, and the next talk's timezone is always the one they forget to double-check.

## The NanoClaw Setup
- Parses the Google Calendar, surfaces next talk's location + local time 2h before showtime
- Confirms demo container health 30 minutes before the talk and pre-caches assets
- Auto-switches to a pre-recorded fallback if Wi-Fi drops below threshold mid-demo
- Logs post-event retro notes with follow-up action tags while the details are fresh

## Sample Telegram Interaction
> **Agent:** Talk in 30 min. Local time: 14:30 CEST. Demo health: green. Wi-Fi: 12 Mbps down. Assets pre-cached. If it drops I'll switch to the fallback automatically. You've got this.
> **DevRel:** What would I do without you.
> **Agent:** Miss flights, probably.

## Why It's a Digital Twin
It handles the operational anxiety of constant travel so you can focus on actually inspiring people.
