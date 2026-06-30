# The YAML Whale

## Persona
Developer who over-engineers everything — five abstraction layers for a timestamp, a microservice for a config file.

## The Problem They Have
PRs take 3 hours to review because nobody can figure out what the code actually does, and the architecture diagram looks like a plate of spaghetti.

## The NanoClaw Setup
- Scans commits for unnecessary abstraction layers and nested complexity, flags PRs exceeding cyclomatic complexity thresholds
- Auto-generates Mermaid architecture diagrams so reviewers can actually understand the PR
- Posts a whale meme when complexity is "impressive" and a gentle "maybe simpler?" suggestion
- Tracks complexity trends over time so the engineer can see their own pattern

## Sample Telegram Interaction
> **Agent:** PR #88: 9 classes to format a timestamp. Cyclomatic complexity: 47. Mermaid diagram attached. It is... beautiful. And wrong.
> **Dev:** I was just formatting a timestamp.
> **Agent:** I know. That's why I'm here.

## Why It's a Digital Twin
It mirrors your ambition while gently reflecting back what the codebase actually needs.
