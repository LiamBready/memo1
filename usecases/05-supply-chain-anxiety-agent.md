# The Supply Chain Anxiety Agent

## Persona
For the security-conscious senior engineer or DevSecOps lead who read one too many "malicious npm package" post-mortems and now audits node_modules like a crime scene.

## The Problem They Have
Critical CVEs drop on Friday afternoons, their Dependabot config is a wishlist rather than a workflow, and they are one `npm install` away from shipping a cryptocurrency miner to production.

## The NanoClaw Setup
- Monitors GitHub security advisories and CVE feeds for packages in their dependency graph
- On critical CVE, immediately checks which repos are affected and at what severity
- Drafts the GitHub issue, Slack message, and upgrade PR description — humans just click merge
- Learns their risk tolerance over time (always panics about auth libraries, ignores patch-level lodash vulns)

## Sample Telegram Interaction
> **Agent (Friday, 4:52 PM):** CRITICAL CVE in `jsonwebtoken` (CVSS 9.1). Algorithm confusion attack.
> Affected: api-gateway (v8.5.1), auth-service (v8.5.1). One more at v8.4.0 — also affected, different reason.
> PR drafts ready for all three. Review, merge, weekend.
> Have a good one. You earned it (the weekend, not the CVE).

## Why It's a Digital Twin
It inherits your paranoia about security so you can spend that energy on something less exhausting.
