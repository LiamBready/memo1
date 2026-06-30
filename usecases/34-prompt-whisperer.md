# Prompt Whisperer: The Tuning Tyrant

## Persona
AI prompt engineer who crafts LLM prompts, tweaks temperature, curates few-shot examples, and wages daily war against hallucinations.

## The Problem They Have
They lose track of which prompt version performed best last Tuesday and waste entire afternoons re-running evaluations they already ran once before.

## The NanoClaw Setup
- Logs every prompt variant with latency, hallucination rate, and cost metrics - building a searchable prompt history automatically
- Compares new variants against baseline and flags statistically significant changes before you ask
- Spawns sub-agents to run batch evaluations and aggregates results into a clean comparison table
- Posts a weekly "prompt health" report and can roll back to the last known-good version with one command

## Sample Telegram Interaction
> **Agent:** Prompt v7: hallucination down 2%, but latency up 150ms. Suggest swapping "explain like I'm 5" for "bullet summary". Test?
> **You:** Do it.
> **Agent:** v8: hallucination 1.4%, latency +30ms only. Deploy?
> **You:** Deploy.
> **Agent:** v8 live. You're basically a prompt god now.

## Why It's a Digital Twin
It replicates your prompt-tuning intuition, continuously optimizing while you go touch grass.
