---
record_id: HYP-REGISTER
title: Engineering Hypothesis Register
status: Draft
release: 0.3.1
owner: OFRP maintainers
last_updated: 2026-08-03
verification: V0
---

# Engineering Hypothesis Register

Hypotheses are testable propositions, not facts. Every entry below is `V0 —
Unverified`; wording does not authorize wiring, coding, or power application.

| ID | Hypothesis | Related research | Status | Verification | Required evidence / falsification route |
|---|---|---|---|---|---|
| HYP-0001 | `AMP-0001` wakes over Infotainment CAN. | [RR-0003](known-unknowns.md#rr-0003) | Open | V0 — Unverified; community report exists | Applicable OEM communication/wiring documentation plus controlled observation; evidence of operation without CAN would narrow or falsify it. |
| HYP-0002 | `AMP-0001` accepts analog differential or high-level audio input from the head unit. | [RR-0009](known-unknowns.md#rr-0009) | Open | V0 — Unverified | Applicable OEM signal description and measurements in a known configuration; evidence of a different transport would falsify it. |
| HYP-0003 | The amplifier DSP dataset is vehicle-specific. | [RR-0010](known-unknowns.md#rr-0010) | Open | V0 — Unverified | Compare traceable OEM dataset/application records and diagnostic identification across known donor configurations. |
| HYP-0004 | `CON-0001` retains enough evidence to reconstruct the complete harness. | [RR-0011](known-unknowns.md#rr-0011) | Open | V0 — Unverified | Complete cavity inventory plus OEM diagrams; missing/ambiguous circuits or unavailable terminals may falsify it. |
| HYP-0005 | Relevant `5C6 035 456` revisions share the reported output mapping and connector family. | [RR-0012](known-unknowns.md#rr-0012) | Open | V0 — Unverified | Primary connector/application data and directly observed keyed interfaces/pin maps for each exact revision. |
| HYP-0006 | `AMP-0001` has no conventional remote turn-on wire. | [RR-0013](known-unknowns.md#rr-0013) | Open | V0 — Unverified | Applicable OEM diagram plus observation of wake behavior; absence cannot be inferred solely from CAN wake reporting. |
| HYP-0007 | Pins 3–22 contain all ten amplified output channel pairs reported by `SRC-0002`. | [RR-0014](known-unknowns.md#rr-0014) | Open | V0 — Unverified for AMP-0001 | Oriented cavity inspection, applicable OEM diagram, passive testing, and later controlled output tests. |
| HYP-0008 | Pins 1, 2, and 23–38 contain power, ground, CAN, audio inputs, and control circuits. | [RR-0015](known-unknowns.md#rr-0015) | Open | V0 — Engineering inference only | Resolve every cavity individually; the unresolved group is not itself evidence of these functions. |
| HYP-0009 | The front stage uses separately amplified woofer, midrange, and tweeter channels. | [RR-0016](known-unknowns.md#rr-0016) | Open | V0 — Unverified for AMP-0001 | OEM topology plus continuity and controlled frequency/output measurements. |
| HYP-0010 | The subwoofer is dual-coil with each coil independently driven. | [RR-0017](known-unknowns.md#rr-0017) | Open | V0 — Unverified for AMP-0001 | Physical subwoofer inspection, coil resistance, OEM topology, and controlled output evidence. |

Resolution must link evidence, record configuration limits, update affected
documents, and retain rejected hypotheses for traceability.
