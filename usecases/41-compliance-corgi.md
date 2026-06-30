# Compliance Corgi

## Persona
Developer in a regulated industry (finance, health) who has to keep code audit-ready while actually shipping features.

## The Problem They Have
Compliance evidence is scattered, audits arrive with 48h notice, and one unreviewed commit touching PHI data can turn a routine audit into a very expensive afternoon.

## The NanoClaw Setup
- Monitors commits touching PHI/compliance-relevant files and drafts change notes automatically
- Runs a daily audit-ready check and maintains a living evidence bundle
- Spawns a sub-agent to static-scan PRs for policy violations before they merge
- Fires a 24h heads-up before audit windows with the evidence bundle pre-packaged and attached

## Sample Telegram Interaction
> **Agent:** PR #221 touches patient_records.py — draft change note ready. PHI access log updated. No policy violations detected.
> **Dev:** Merge it.
> **Agent:** Merged. Evidence bundle updated. Audit window in 6 days — I'll send the full package in 5.
> **Dev:** You just saved me two hours of paperwork.
> **Agent:** That's what I'm here for. 🐾

## Why It's a Digital Twin
It carries the compliance burden so you can ship features without a legal anxiety attack.
