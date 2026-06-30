# Pipeline Piper

## Persona
Data scientist turned ML engineer who has to keep models alive in production — retraining, monitoring, and explaining why the model suddenly started doing that.

## The Problem They Have
Feature distribution shifts silently, models degrade gradually, and nobody notices until a business metric tanks and someone sends a very polite but very pointed Slack message.

## The NanoClaw Setup
- Watches the feature store for distribution shift >10% and triggers a nightly retraining sub-agent
- Only pushes to the model registry if the retrained model actually improves on eval metrics
- Auto-updates model card READMEs with new performance stats after each deployment
- Sends a weekly "Model Health" digest with traffic-light status per model in production

## Sample Telegram Interaction
> **Agent:** user_session_duration shifted 12% since Tuesday. Likely the new onboarding flow. Retraining started.
> **Engineer:** Let me know the result.
> **Agent:** Retrained model: +1.8% accuracy. Deployed to registry. Model card updated. The onboarding team owes you one.

## Why It's a Digital Twin
It keeps your models honest so you don't have to babysit them at 2am.
