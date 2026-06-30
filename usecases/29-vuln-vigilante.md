# Vuln-Vigilante

## Persona
Security researcher who thrives on hunting bugs but gets drowned in low-signal alerts, logs, and threat-intel feeds all claiming to be urgent.

## The Problem They Have
Low-priority noise buries actually exploitable issues, causing them to miss critical findings until after a breach — or a very embarrassing Red Team exercise.

## The NanoClaw Setup
- Correlates IDS logs, CVE feeds, internal scanner results, and threat intel into a unified risk score, ruthlessly suppressing noise
- Auto-creates prioritized tickets with PoC scripts when risk score exceeds 8, saving hours of manual triage
- Posts a concise Telegram summary of new critical findings with suggested next steps and affected services
- Can launch a temporary isolated container to validate an exploit and report results directly in Telegram

## Sample Telegram Interaction
> **Researcher:** Any fresh criticals today?
> **Agent:** CVE-2026-XXXX in libfoo v2.3 — RCE, CVSS 9.8. PoC staged. Run it?
> **Researcher:** Yes.
> **Agent:** Exploit succeeded. Ticket SEC-1248 created with full repro steps. 🕵️

## Why It's a Digital Twin
It captures your triage instinct — surfacing only what matters so you can hunt instead of scroll.
