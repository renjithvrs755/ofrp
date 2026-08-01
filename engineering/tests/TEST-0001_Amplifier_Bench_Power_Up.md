---
record_id: TEST-0001
title: Amplifier Bench Power-Up Test Template
status: Draft Template — Not Run
release: 0.3.0
owner: OFRP maintainers
last_updated: 2026-08-01
verification: V0 — Not executed
---

# TEST-0001 — Amplifier Bench Power-Up

> **WARNING — NOT AUTHORIZED:** This is an unexecuted template, not a wiring
> instruction or completed test. Do not energize `AMP-0001` until every gate in
> `VAL-0001` passes and an independent reviewer approves the filled record.

> **WARNING:** Do not apply 12–14.4 V to any amplifier cavity until battery
> positive and ground assignments are supported by at least two independent
> evidence sources, one of which must be OEM documentation or direct physical
> verification.

## Test administration

| Field | Entry |
|---|---|
| Test ID | `TEST-0001` |
| Status | Not Run |
| Date/time | Pending |
| Operator | Pending |
| Reviewer | Pending |
| Amplifier specimen | `AMP-0001` |
| Connector specimen | `CON-0001` |
| Harness/breakout specimen | Pending (`HAR-NNNN`) |
| Applicable validation revision | `VAL-0001`, revision pending |

## Controlled test configuration

| Field | Planned / measured value | Evidence status |
|---|---|---|
| Power-supply make/model | Pending | V0 |
| Power-supply current limit | Not selected | V0; requires reviewed derivation |
| Fuse type and value | Not selected | V0; must not be invented or copied without applicable evidence |
| Test voltage | Not selected | V0; target range is not authorization |
| Positive cavity and evidence | Unknown | V0; two-source rule not met |
| Ground cavity and evidence | Unknown | V0; two-source rule not met |
| Wiring configuration / diagram | Pending | V0 |
| Lead sizes and protection | Pending | V0 |
| Wake-up method | Unknown | V0 |
| CAN status/configuration | Unknown / disconnected unless separately approved | V0 |
| Loads connected | None unless separately reviewed | V0 |

## Pre-power resistance checks

| Check | Acceptance criterion | Result | Instrument / evidence |
|---|---|---|---|
| Supply positive to ground | Pending engineering review | Not measured | Pending |
| Supply positive to enclosure | Pending engineering review | Not measured | Pending |
| Ground to enclosure | Pending engineering review | Not measured | Pending |
| Adjacent-cavity shorts at breakout | No unintended continuity; quantitative threshold pending | Not measured | Pending |
| Polarity and fuse continuity | Must match reviewed wiring diagram | Not checked | Pending |

## Expected behavior

Unknown (`V0`). Define observable current, timing, diagnostic, audio, and thermal
expectations from applicable evidence before approval. Absence of expected
behavior must not prompt ad-hoc voltage, cavity, CAN, or wake changes.

## Execution record

| Observation | Result |
|---|---|
| Initial voltage at supply and amplifier | Not measured |
| Measured idle current | Not measured |
| Peak/inrush current and duration | Not measured |
| Current-limit behavior | Not observed |
| Wake-up method attempted | None |
| CAN status/messages | Not captured |
| Diagnostic response | Not tested |
| Audio/output behavior | Not tested |
| Thermal observations and measurement points | Not measured |
| Odor/noise/other observations | Not observed |
| Result | **NOT RUN** |
| Anomalies | None recorded; test not run |

## Evidence files

- Reviewed wiring diagram: Pending.
- Setup photographs: Pending (`IMG-NNNN`).
- Supply log/current capture: Pending.
- Thermal measurements: Pending (`MEAS-NNNN`).
- CAN/diagnostic capture: Pending and subject to separate approval.

## Review

| Role | Name | Date | Decision / signature reference |
|---|---|---|---|
| Operator | Pending | Pending | Not executed |
| Independent reviewer | Pending | Pending | Not approved |

Any completed execution must retain the original planned values, deviations,
raw results, stop events, and evidence. Do not overwrite this template with a
claim of success lacking the required records.
