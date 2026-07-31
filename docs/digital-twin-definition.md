# What “Digital Twin” means here

The phrase is used loosely in consumer technology. We use it in the engineering sense.

A Digital Twin is a live, individual-specific computational model of a real-world system, kept in step through a feedback loop and used to estimate present state and reason about likely future state.

For Opti-U, the real-world system is one person's behavioural and physiological state.

## Five required properties

### 1. Individual-specific

The model is anchored to personal history and baselines, not only a population average.

### 2. Continuously updated

New consented observations can update the model while preserving time, source and quality context.

### 3. State-bearing

It maintains an explicit estimate of current state rather than reconstructing a transient answer from a prompt.

### 4. Forward-looking

It can represent trajectory and uncertainty, not merely score the latest observation.

### 5. Closed-loop

Actions and outcomes return as evidence. The model can learn from measured response—but only when evidence gates allow it.

## What it is not

- a dashboard renamed as a twin;
- a chatbot with access to wearable summaries;
- a static user profile;
- a population score presented as personal truth;
- a claim of biological simulation at clinical fidelity.

## A twin should be allowed to say “not enough data”

Uncertainty is part of state, not an inconvenient footnote. If observations are sparse, stale or contradictory, the most accurate output may be suppression.

The companion **Governed Digital Twin Reference** demonstrates that principle with generic synthetic data. Its constants and algorithms are intentionally educational and do not reproduce the Opti-U implementation.
