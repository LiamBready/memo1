# Latency Llama: The Performance-Obsessed Sidekick

## Persona
Backend engineer who lives and breathes latency numbers and constantly refreshes dashboards to catch the slightest p99 spike.

## The Problem They Have
They waste hours manually checking metrics, missing SLO breaches until users complain — then scramble to firefight while pretending it was planned maintenance.

## The NanoClaw Setup
- Responds to `/latency <service>` commands with real-time p99/p95 stats from Prometheus/Grafana
- Auto-triggers load-testing sub-agents when p99 exceeds the configured threshold, before any human notices
- Suggests config tweaks (thread pools, timeouts, circuit breakers) and applies them via CI with one Telegram thumbs-up
- Posts a daily performance digest with trends, anomalies, and top optimizations ranked by impact

## Sample Telegram Interaction
> **Engineer:** What's the p99 for payment-service?
> **Agent:** 210ms — up 15% from baseline. Suggest: increase DB connection pool to 80.
> **Engineer:** Apply it.
> **Agent:** Pool updated. New p99: 180ms. Monitoring for regression. 🦙

## Why It's a Digital Twin
It mirrors your relentless performance obsession — a tireless latency conscience that never sleeps.
