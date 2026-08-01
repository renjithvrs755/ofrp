---
record_id: HYP-REGISTER
title: Engineering Hypothesis Register
status: Draft
release: 0.3.0
owner: OFRP maintainers
last_updated: 2026-08-01
verification: V0
---

# Engineering Hypothesis Register

Hypotheses are testable propositions, not facts. Every entry below is `V0 —
Unverified`; wording does not authorize wiring, coding, or power application.

| ID | Hypothesis | Related research | Status | Verification | Required evidence / falsification route |
|---|---|---|---|---|---|
| HYP-0001 | `AMP-0001` requires CAN-based wake-up. | [RR-0003](known-unknowns.md#rr-0003) | Open | V0 — Unverified | Applicable OEM communication/wiring documentation plus controlled observation; evidence of operation without CAN would narrow or falsify it. |
| HYP-0002 | `AMP-0001` accepts analog differential or high-level audio input from the head unit. | [RR-0009](known-unknowns.md#rr-0009) | Open | V0 — Unverified | Applicable OEM signal description and measurements in a known configuration; evidence of a different transport would falsify it. |
| HYP-0003 | The amplifier DSP dataset is vehicle-specific. | [RR-0010](known-unknowns.md#rr-0010) | Open | V0 — Unverified | Compare traceable OEM dataset/application records and diagnostic identification across known donor configurations. |
| HYP-0004 | `CON-0001` retains enough evidence to reconstruct the complete harness. | [RR-0011](known-unknowns.md#rr-0011) | Open | V0 — Unverified | Complete cavity inventory plus OEM diagrams; missing/ambiguous circuits or unavailable terminals may falsify it. |
| HYP-0005 | Part `5C6 035 456` and later suffix revisions share the same connector family. | [RR-0012](known-unknowns.md#rr-0012) | Open | V0 — Unverified | Primary connector/application data and directly observed keyed interfaces for each exact revision. |

Resolution must link evidence, record configuration limits, update affected
documents, and retain rejected hypotheses for traceability.
