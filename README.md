# Opti-U

### The AI Performance Digital Twin for adaptive coaching

Wearables can tell us how we slept, how hard we trained and how today compares with yesterday. That is useful, but it stops too early.

The harder question is not simply *what happened?* It is *what helps this person, under these conditions, and how certain are we?*

Opti-U is built to answer that question. It connects longitudinal wearable and behavioural data with persistent state estimation, adaptive coaching and user-approved N-of-1 experiments.

```text
Sense → Estimate → Forecast → Experiment → Measure → Learn
  ↑                                                    │
  └──────────────── governed feedback ─────────────────┘
```

## The system in one minute

Opti-U combines five reinforcing layers:

1. A structured 12-week coaching journey.
2. A persistent, individual-specific Digital Twin.
3. State-aware adaptive protocols rather than static habits.
4. User-approved N-of-1 experiments that measure response.
5. Governed population learning that can advise but never overwrite the individual.

The intelligence core is independent of large language models. Generative AI can communicate and explain structured results, but it cannot own user state, determine safety, establish causal effects or silently increase its influence.

The central design principle is simple:

> **A trustworthy system must know when not to make a claim.**

Weak evidence, stale data or low confidence should cause suppression, refusal or a safe fallback—not a more fluent guess.

## Current position

Opti-U has completed controlled TRL5 technical validation using deterministic and generated scenarios. The platform includes:

- bounded domains with explicit ownership;
- wearable ingestion and normalisation;
- physiological and behavioural signal processing;
- typed events and narrow gateway interfaces;
- deterministic controls around consent, safety and decision authority;
- state estimation, forecasting and uncertainty handling;
- anomaly suppression and minimum-sample gates;
- traceable decisions, rollback and safe degradation.

This establishes that the integrated platform can operate under controlled representative conditions and respond conservatively to deliberately difficult inputs. It does not establish live-user effectiveness, calibrated forecasts on human cohorts, production reliability at scale or institutional operation. Those are the next TRL6–7 objectives.

Implementation, controlled validation, live operation and behavioural outcomes are separate stages and are reported separately.

## What is private

The production core remains private because it contains proprietary orchestration, behavioural specifications, safety policies and intervention-learning logic. Operational thresholds, internal contracts, infrastructure details, model artefacts, security findings and personal data are not published here.

The projects here cover three areas:

1. **Opti-U** — the product, architecture, governance model and path from TRL5 to production.
2. **Governed Digital Twin Reference** — confidence-gated state estimation, forecasting and traceable refusal.
3. **N-of-1 Evidence Gates** — sample, missingness, adherence and overlap gates for individual experiments.

The two smaller packages use generated data, generic signal names and invented constants. They contain no production modules, schemas, fixtures, tests or thresholds, and they are not medical tools.

## How it is built

The code uses typed interfaces, deterministic tests and continuous integration. Examples can be run locally, and the limitations of each model are documented alongside it.

## Start here

- [Why the category is missing](docs/category.md)
- [Architecture overview](docs/architecture-overview.md)
- [What “Digital Twin” means here](docs/digital-twin-definition.md)
- [Governance principles](docs/governance-principles.md)
- [Validation record](docs/evidence-ledger.md)
- [What remains to be proved](docs/trl5-to-trl7.md)
- [Repository boundaries](docs/evidence-boundaries.md)
- [A synthetic journey through the loop](examples/synthetic-user-journey.md)

## About

Opti-U was conceived and architected by [Spencer North](https://github.com/Snorth86), Founder, CEO and System Architect.

[opti-u.com](https://opti-u.com) · [Technology](https://opti-u.com/technology) · [snorth@opti-u.com](mailto:snorth@opti-u.com)
