---
record_id: TEST-0003
title: Single-Channel Audio Output Check Template
status: Draft Template — Prohibited/Not Run
release: 0.3.1
owner: OFRP maintainers
last_updated: 2026-08-03
verification: V0 — Not executed
---

# TEST-0003 — Single-Channel Audio Output Check

> **POWERED TEST PROHIBITED:** This unexecuted template is not authorization.
> Run only after power and ground are independently verified, connector
> orientation passes `VAL-0001`, amplifier wake-up is confirmed, and the filled
> test configuration is independently reviewed.

> **SAFETY GATE — NO POWER:** Do not apply power to the amplifier until:
> - connector orientation is verified,
> - battery positive is verified,
> - ground is verified,
> - no output pin is shorted, and
> - supply is fused and current-limited.

## Preconditions

- [ ] Power and ground meet the independent-evidence rule.
- [ ] Wake-up method has a completed, reviewed validation record.
- [ ] Reported pair passed `TEST-0002` and has no short to chassis/other pairs.
- [ ] Current-limited, fused supply and emergency disconnect are verified.
- [ ] DC output acceptance criterion and stop threshold are reviewed.
- [ ] One sacrificial full-range or woofer test speaker is connected first.
- [ ] No tweeter or subwoofer is connected.
- [ ] Input begins at its minimum level.

## Administration and setup

| Field | Entry |
|---|---|
| Status/result | **NOT RUN** |
| Date/operator/reviewer | Pending |
| Specimen IDs | `AMP-0001`, `CON-0001`, speaker pending |
| Selected candidate pair | Pending |
| Verified power/ground evidence | Pending |
| Wake-up validation | Pending |
| Supply voltage/current limit/fuse | Pending; must be approved |
| Input source, signal, and level | Pending; start at minimum |
| Speaker impedance/rating | Pending |
| DC output before speaker connection | Not measured |
| Scope/meter evidence IDs | Pending |

## Initial candidate channels

| Channel | Reported pair | Eligibility |
|---|---|---|
| LF woofer | 18/6 | Deferred until all preconditions pass |
| RF woofer | 15/3 | Deferred until all preconditions pass |
| LR speaker | 9/21 | Deferred until all preconditions pass |
| RR speaker | 22/10 | Deferred until all preconditions pass |

Tweeter and subwoofer tests are deferred until crossover behavior, DC content,
frequency range, load limits, and topology are confirmed.

## Observations and stop conditions

Record idle/active current, DC output, waveform, sound, heat, noise, and
instability. Stop immediately for excessive current, heating, smoke, odor, DC
output beyond the reviewed threshold, abnormal noise, oscillation, intermittent
operation, or unstable supply behavior. Disconnect with the emergency control;
do not move to another pin pair as troubleshooting.

| Expected behavior | Actual result | Anomaly | Evidence IDs | Reviewer decision |
|---|---|---|---|---|
| Pending review | Not run | None recorded | Pending | Not approved |
