---
record_id: AMP-0001
title: Panasonic 5C6 035 456 Amplifier Component Record
status: Draft
release: 0.3.1
owner: OFRP maintainers
last_updated: 2026-08-03
verification: V1/V3 as itemized
---

# AMP-0001 — Panasonic 5C6 035 456

## Identity and provenance

| Field | Value | Evidence status | Evidence / action |
|---|---|---|---|
| Component ID | `AMP-0001` | V3 — Observed | Assigned to the project-owned specimen. |
| OEM part number | `5C6 035 456` | V3 — Observed | Label observation; capture `IMG-NNNN`. |
| Manufacturer | Panasonic | V3 — Observed | Label observation; capture `IMG-NNNN`. |
| Label description | `10CH Audio Amplifier` | V3 — Observed | Label observation; capture `IMG-NNNN`. |
| Hardware label field | Not recorded | V0 — Unknown | Transcribe from label without interpretation. |
| Software label field | Not recorded | V0 — Unknown | Transcribe from label without interpretation. |
| Serial/date fields | Not recorded | V0 — Unknown | Transcribe and photograph. |
| Source | Used-parts seller | V1 — Reported | Preserve purchase correspondence if available. |
| Donor | Working 2014 Passat | V1 — Reported | Seller statement; donor VIN/market/platform unverified. |
| Purchase condition | Purchased used | V3 — Observed | Project ownership record; price/date not recorded here. |
| Operational condition | Seller reported working | V1 — Reported | No OFRP functional test completed. |
| Current verification level | Mixed V1/V3 | — | Applies only to itemized identity/provenance; electrical behavior remains V0. |

## Connector status

| Field | Value | Evidence status |
|---|---|---|
| Associated connector | [`CON-0001`](../connectors/CON-0001_Panasonic_Fender_Amplifier_Connector.md) | V3 — Observed |
| Connector ownership | In project possession | V3 — Observed |
| Original wiring | Only a few centimetres retained | V3 — Observed |
| Spare connector | Reported ordered | V1 — Reported; receipt and identity unverified |

## Visible-condition checklist

| Check | Result | Evidence status / reference |
|---|---|---|
| Label legible | Not recorded | V0 — Unknown; `IMG-NNNN` |
| Housing cracks or impact | Not inspected | V0 — Unknown; `IMG-NNNN` |
| Corrosion or liquid ingress | Not inspected | V0 — Unknown; `IMG-NNNN` |
| Heat discoloration or odor | Not inspected | V0 — Unknown |
| Connector pins bent/recessed | Not inspected | V0 — Unknown; macro images required |
| Fasteners or seals disturbed | Not inspected | V0 — Unknown; do not open solely to complete this check |
| Mounting points damaged | Not inspected | V0 — Unknown; `IMG-NNNN` |

## Physical properties and mounting

| Field | Recorded value | Evidence status |
|---|---|---|
| Length × width × height | Not measured | V0 — Unknown |
| Mass | Not measured | V0 — Unknown |
| Measurement instruments | Not assigned | V0 — Unknown |
| Bracket(s) supplied | Not recorded | V0 — Unknown |
| Donor mounting location/orientation | Not independently verified | V0 — Unknown |
| Target mounting location/orientation | Not selected | V0 — Unknown |

## Evidence references

- [Amplifier dossier](../../../manual/OFRP-310_Panasonic_Fender_Amplifier_5C6035456.md)
- [Connector and pinout validation plan](../../validation/VAL-0001_Amplifier_Connector_and_Pinout_Validation.md)
- [Pinout working register](../../wiring/AMP-0001_pinout_working_register.md)
- Image records: not yet assigned (`V0`).
- OEM documentation: not yet acquired (`V0`).

Electrical characteristics, compatibility, pinout, coding, and functional
condition are outside this identity record and remain `V0 — Unknown` until
their linked evidence satisfies OFRP-110.

> **SAFETY GATE — NO POWER:** Do not apply power to the amplifier until:
> - connector orientation is verified,
> - battery positive is verified,
> - ground is verified,
> - no output pin is shorted, and
> - supply is fused and current-limited.
