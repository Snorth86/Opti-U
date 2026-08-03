# A synthetic journey through the loop

This fictional example illustrates the public information flow only. It is not a product screenshot, protocol, recommendation engine or clinical scenario.

## Connection: the journey starts with history

Alex connects a fictional wearable and grants the relevant permission.

The system does not begin from an empty “Day 1” if historical data is available. Connection initiates a bounded backfill of the wearable history. Records are normalised into a provider-independent shape and processed in chronological order, with provenance, consent and duplicate handling preserved.

When the backfill completes, the system rebuilds the derived evidence once against the completed history:

```text
Wearable connected
        ↓
Historical data backfilled
        ↓
Signals canonicalised and quality-checked
        ↓
Personal baselines established from eligible history
        ↓
Current state, confidence and sentinels recalculated
        ↓
Daily incremental sync begins
```

Alex therefore enters the live coaching journey with a history-backed personal baseline wherever the connected data has sufficient coverage. A sparse or unavailable signal can still remain individually low-confidence; one weak metric does not turn the entire person into a cold start.

**Output:** `BASELINE_ESTABLISHED`, with confidence retained per eligible signal

## First live day: current state is personal from the start

The latest observation is interpreted against Alex's own historic distribution rather than a generic population average. The system can describe whether a signal is broadly in line with, above or below that recent personal baseline.

That is state estimation. It is not yet causal attribution.

**Output:** `CURRENT_STATE_ESTIMATED`

## A pattern develops

As daily incremental observations arrive, a pattern of later sleep timing and lower self-reported energy appears relative to Alex's established history.

The system can describe the pattern, its direction and its confidence. It still cannot claim what caused it.

**Output:** `PATTERN_OBSERVED`

## Alex approves a small experiment

Alex chooses a simple, fictional routine change. The system records the question, observation window and outcome measure before the experiment begins.

The choice belongs to Alex. The system does not silently enrol them or change the target after seeing the result.

**Output:** `EXPERIMENT_ACTIVE`

## The tempting answer is refused

Early observations look positive, but adherence was inconsistent and several outcomes are missing. A fluent system could still tell a persuasive story. A governed system does not.

The physiological baseline remains available; the experiment conclusion is what stays unresolved. Evidence is scoped rather than reduced to one global confidence score.

**Output:** `INCONCLUSIVE`

## Evidence supports a bounded conclusion

After a better-quality comparison, the measured outcome is directionally positive and uncertainty is inside the fictional demonstration's declared boundary.

The result is recorded with its data window, missingness, adherence and uncertainty. It can inform the next user-approved step. It does not become a universal rule.

**Output:** `KEEP`, bounded to this person and this question

## What compounds

The valuable asset is not a stream of recommendations. It is the longitudinal record connecting personal history, current context, decision, exposure and measured response—together with every occasion when the evidence was not good enough to learn.
