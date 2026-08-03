# Opti-U technical overview

Opti-U is a governed AI Performance Digital Twin built to connect longitudinal wearable and behavioural data with persistent state estimation, adaptive coaching and user-approved N-of-1 experiments.

## Current position

The platform has completed controlled TRL5 technical validation using deterministic and generated scenarios. The current implementation includes:

- bounded domains with explicit ownership;
- wearable ingestion and normalisation;
- physiological and behavioural signal processing;
- typed events and narrow gateway interfaces;
- deterministic controls around consent, safety and decision authority;
- state estimation, forecasting and uncertainty handling;
- anomaly suppression and minimum-sample gates;
- traceable decisions, rollback and safe degradation.

Large language models are limited to interaction and explanation. They do not own user state, determine safety or establish causal effects.

TRL6 and TRL7 work will address live-user outcomes, forecast calibration, production reliability, security assurance and institutional operation.

## Repository boundaries

The production core remains private because it contains proprietary orchestration, behavioural specifications, safety policies and intervention-learning logic. Operational thresholds, internal contracts, infrastructure details, model artefacts, security findings and personal data are not published.

The repositories cover three areas:

1. `opti-u` explains the product, system boundaries and path from TRL5 to production.
2. `governed-digital-twin-reference` implements confidence-gated state estimation with traceable refusal.
3. `n-of-1-evidence-gates` implements sample, missingness, adherence and overlap gates for individual experiments.

The two reference packages use generated data, generic signal names and invented constants. They are independent implementations and contain no copied production modules, schemas, fixtures, tests or thresholds.

## Engineering standard

Each code repository includes typed interfaces, deterministic tests, CI, reproducible examples, security guidance and explicit limitations. Results are stated with their scope; controlled validation is not presented as live-user or clinical evidence.
