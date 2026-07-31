# Opti-U

### The adaptive coaching layer above connected health

Wearables have made human signals abundant. They can tell us how we slept, how hard we trained and how today compares with yesterday.

That is useful. It also stops too early.

The harder question is not *what happened?* It is *what helps this person, under these conditions, and how certain are we?*

Opti-U is being built to answer that question: a closed-loop adaptive coaching system powered by a behavioural-physiological Digital Twin.

```text
Sense → Estimate → Forecast → Experiment → Measure → Learn
  ↑                                                    │
  └──────────────── governed feedback ─────────────────┘
```

This repository explains the public architecture thesis, the evidence posture and the boundaries around the private production system. It contains no production source code or proprietary decision logic.

## The system in one minute

Opti-U combines five reinforcing layers:

1. A structured 12-week coaching journey.
2. A persistent, individual-specific Digital Twin.
3. State-aware adaptive protocols rather than static habits.
4. User-approved N-of-1 experiments that measure response.
5. Governed population learning that can advise but never overwrite the individual.

The intelligence core is independent of large language models. Generative AI can help communicate and explain. It cannot own state, declare safety, establish causal effect or silently increase its influence.

The central design principle is simple:

> **A trustworthy system must know when not to make a claim.**

Weak evidence, stale data or low confidence should cause suppression, refusal or a safe fallback—not a more fluent guess.

## Start here

- [Why the category is missing](docs/category.md)
- [Public architecture overview](docs/architecture-overview.md)
- [What “Digital Twin” means here](docs/digital-twin-definition.md)
- [Governance principles](docs/governance-principles.md)
- [Evidence ledger](docs/evidence-ledger.md)
- [What remains to be proved](docs/trl5-to-trl7.md)
- [What is public and what stays private](docs/evidence-boundaries.md)
- [A synthetic journey through the loop](examples/synthetic-user-journey.md)

## Evidence, with the boundary attached

Opti-U has completed controlled TRL5 technical validation. That supports the claim that an integrated platform can operate under controlled representative conditions and degrade conservatively under deliberately difficult inputs.

It does **not** establish live-user effectiveness, calibrated forecasts on human cohorts, production reliability at scale or institutional operation. Those are explicit TRL6–7 objectives.

That distinction matters. Implementation evidence, controlled validation, live operational evidence and behavioural outcome evidence are different things. We publish them as different things.

## Public reference work

Two clean-room companion repositories make selected principles executable without reproducing Opti-U:

- **Governed Digital Twin Reference** — synthetic state estimation, confidence, forecasting and refusal.
- **N-of-1 Evidence Gates** — synthetic experimentation where `INCONCLUSIVE` is a valid result.

These are educational reference implementations. They are not medical tools and are not extracted from the production platform.

## About

Opti-U was conceived and architected by [Spencer North](https://github.com/Snorth86), Founder, CEO and System Architect.

[opti-u.com](https://opti-u.com) · [Technology](https://opti-u.com/technology) · [snorth@opti-u.com](mailto:snorth@opti-u.com)
