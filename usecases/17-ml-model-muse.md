# The Model Muse

## Persona
ML engineer obsessed with hyperparameter tuning, wandb logs, and that elusive 0.1% accuracy gain.

## The Problem They Have
They lose track of experiments, occasionally train on the test set by mistake, and miss data drift alerts until the model starts predicting nonsense in production.

## The NanoClaw Setup
- Monitors experiment tracking runs and suggests the next hyperparameter set via Bayesian optimization before you close your laptop
- Pings when data drift exceeds 5% on any feature, with a visual diff and suggested retraining schedule
- Auto-generates a README snippet for the best-performing model each night and opens a draft PR
- Spawns a sub-agent to purge stale S3 experiment artifacts when storage hits 80%

## Sample Telegram Interaction
> **Agent:** Validation accuracy dropped 2%. Data drift detected in `user_session_duration`.
> **Engineer:** Rollback to v3 and open a retraining ticket.
> **Agent:** Done. Ticket ML-204 created, v3 is live. Here's a confused panda for the post-mortem. 🐼

## Why It's a Digital Twin
It learns your modeling habits and preempts your next tweak before you even open a notebook.
