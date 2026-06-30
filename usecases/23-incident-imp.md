# Incident Imp: The On-Call Gremlin

## Persona
SRE drowning in alert fatigue who misses real incidents because everything is on fire all the time anyway.

## The Problem They Have
Monitoring tools scream at every tiny blip, hours get wasted on false positives, and when a real outage hits you forget to capture the timeline for the post-mortem.

## The NanoClaw Setup
- Correlates Prometheus alerts to suppress noise — only fires when a true anomaly persists >2 minutes
- Enriches each alert with recent metrics, relevant logs, and runbook links before hitting Telegram
- Suggests one-click mitigation steps approved via a Telegram reaction
- After resolution, auto-creates the incident ticket with a full timeline and saves the post-mortem draft

## Sample Telegram Interaction
> **Agent:** 🚨 `svc-api` latency 1.2s (baseline 200ms). Runbook linked. Rollback to v1.4.2?
> **You:** 👍
> **Agent:** Rolled back. Latency 180ms. INC-452 created. Draft post-mortem saved. Sleep well. 😈

## Why It's a Digital Twin
It mimics your SRE instincts, surfaces real incidents, and handles the noisy parts so you can focus on fixing things.
