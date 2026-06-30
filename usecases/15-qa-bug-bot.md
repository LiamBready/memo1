# QA Engineer's Bug Bot

## Persona
QA engineers chasing flaky tests, regressions, and "works on my machine" bugs while trying to keep the test suite green.

## The Problem They Have
Tests mysteriously fail after merges, flaky tests waste hours on reruns, and important edge cases aren't added until a customer finds them in production.

## The NanoClaw Setup
- Watches CI pipelines and alerts when a test's success rate drops below 90% over 5 runs, tagging the likely offending commit
- Suggests new test cases based on recent production errors from Sentry/Datadog
- Auto-creates a JIRA ticket for any flaky test with pre-filled description and repro steps
- Sends a daily "test-health haiku" summarizing pass/fail counts (because QA engineers deserve poetry)

## Sample Telegram Interaction
> **Agent:** 🚨 `test_api_auth_revoke` flaky — 62% success over last 5 runs. Likely: race condition in token cache (commit a1b2c3d). File a ticket?
> **You:** Yes, and draft a test for the missing refresh token case.
> **Agent:** QA-1874 created. Test draft added to backlog.

## Why It's a Digital Twin
It continuously mirrors your test suite's vitals and predicts failures before they bite.
