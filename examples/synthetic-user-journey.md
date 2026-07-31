# A synthetic journey through the loop

This fictional example illustrates information flow only. It is not a product screenshot, protocol, recommendation engine or clinical scenario.

## Day 1: there is not enough history

Alex connects a fictional wearable feed and completes a short behavioural check-in.

The system has observations, but no stable personal baseline. It records state as uncertain and keeps support general. It does not turn a population average into a personal conclusion.

**Output:** `NOT_ENOUGH_HISTORY`

## Day 12: a baseline is beginning to form

The signal stream is sufficiently complete to compare recent observations with Alex's own history. A pattern of later sleep timing and lower self-reported energy appears.

The system can describe the pattern. It still cannot claim what caused it.

**Output:** `PATTERN_OBSERVED`

## Day 15: Alex approves a small experiment

Alex chooses a simple, fictional routine change. The system records the question, observation window and outcome measure before the experiment begins.

The choice belongs to Alex. The system does not silently enrol them or change the target afterwards.

**Output:** `EXPERIMENT_ACTIVE`

## Day 25: the tempting answer is refused

Early observations look positive, but adherence was inconsistent and several outcomes are missing. A fluent system could still tell a persuasive story. A governed system does not.

**Output:** `INCONCLUSIVE`

## Day 36: evidence supports a bounded conclusion

After a better-quality comparison, the measured outcome is directionally positive and uncertainty is inside the fictional demonstration's declared boundary.

The result is recorded with its data window, missingness, adherence and uncertainty. It can inform the next user-approved step. It does not become a universal rule.

**Output:** `KEEP`, bounded to this person and this question

## What compounds

The valuable asset is not a stream of recommendations. It is the longitudinal record connecting context, decision, exposure and measured response—together with every occasion when the evidence was not good enough to learn.
