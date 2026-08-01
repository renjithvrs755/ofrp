---
record_id: CON-0001
title: Panasonic Fender Amplifier Connector Record
status: Draft
release: 0.3.0
owner: OFRP maintainers
last_updated: 2026-08-01
verification: V0/V3 as itemized
---

# CON-0001 — Panasonic Fender Amplifier Connector

## Identity and custody

| Field | Value | Evidence status | Evidence / action |
|---|---|---|---|
| Connector ID | `CON-0001` | V3 — Observed | Project inventory assignment. |
| Associated amplifier | [`AMP-0001`](../amplifiers/AMP-0001_Panasonic_5C6035456.md) | V3 — Observed | Fits/was supplied for the owned amplifier; mating inspection evidence pending. |
| Ownership | In project possession | V3 — Observed | Project custody. |
| Housing manufacturer | Not identified | V0 — Unknown | Photograph and transcribe molded marks. |
| Housing part number | Not identified | V0 — Unknown | Do not infer from similar-looking online listings. |
| Housing revision/index | Not identified | V0 — Unknown | Record all molded marks. |
| Terminal manufacturer/family | Not identified | V0 — Unknown | Identify without destructive removal where possible. |
| Terminal part number/size | Not identified | V0 — Unknown | Measurement and primary documentation required. |
| Cavity count | Not recorded | V0 — Unknown | Establish from oriented face photographs. |
| Keying/code | Not recorded | V0 — Unknown | Photograph housing and amplifier interface. |
| Lock/secondary lock | Not recorded | V0 — Unknown | Identify position before manipulation. |

## Photo placeholders

| Required view | Image ID | Status |
|---|---|---|
| Mating face, straight-on | `IMG-NNNN` | V0 — Not captured |
| Wire-entry face, straight-on | `IMG-NNNN` | V0 — Not captured |
| Each side and latch/key detail | `IMG-NNNN` | V0 — Not captured |
| Molded housing markings | `IMG-NNNN` | V0 — Not captured |
| Amplifier interface, straight-on | `IMG-NNNN` | V0 — Not captured |
| Each populated cavity and pigtail | `IMG-NNNN` | V0 — Not captured |

## Cavity-map placeholder

No cavity map is approved. Create a diagram only after orientation and molded
numbering are recorded under `VAL-0001`.

```text
VIEW: NOT ESTABLISHED — DO NOT NUMBER FROM THIS PLACEHOLDER

[ Photograph/diagram to be inserted after orientation validation ]
```

> **WARNING:** Cavity numbering depends on whether the connector is viewed from
> the mating face or wire-entry face, as well as connector orientation. Never
> mirror an internet diagram or number cavities by visual sequence. Record the
> viewing direction, latch/key position, molded indices, and image ID with every
> cavity reference.

## Short-pigtail observations

Only a few centimetres of original wiring remain (`V3 — Observed`). The number
of populated positions, wire colors, stripe colors, gauges, splices, terminal
seals, and original circuit destinations are not recorded (`V0 — Unknown`). A
short pigtail may preserve useful observations, but it does not prove a circuit
function or complete-harness reconstruction.

## Wire-color recording table

Color observations must use neutral lighting and a color reference when
possible. A color is descriptive evidence only and must not be treated as a
function assignment.

| Oriented cavity | Base color | Stripe/tracer | Apparent gauge | Terminal populated | Image ID | Evidence status | Notes |
|---|---|---|---|---|---|---|---|
| Unknown | Unknown | Unknown | Unknown | Unknown | Pending | V0 | Add one row per cavity after orientation is established. |

## Handling and depinning notes

- Keep `CON-0001` disconnected and de-energized during inspection.
- Use ESD-aware handling and protect the mating face from loose metal objects.
- Do not back-probe with an oversized tool or force a gauge into a terminal.
- Do not release the secondary lock until its mechanism and service position
  are identified (`V0`) from physical observation or applicable documentation.
- Do not depin solely to identify a wire. Photograph and label every position
  first; use the correct extraction tool only after terminal family is verified.
- If depinning becomes necessary, record operator, date, original cavity,
  orientation, image IDs, tool, terminal condition, and reassembly verification.
- Stop if the housing, lock, seal, or terminal begins to deform.

## Validation checklist

- [ ] Assign image IDs and capture all required views.
- [ ] Establish mating-face and wire-entry-face orientation.
- [ ] Record latch/key position and molded cavity indices.
- [ ] Independently review the cavity-numbering overlay.
- [ ] Record every populated and empty cavity without assigning functions.
- [ ] Record pigtail colors and apparent gauges.
- [ ] Identify housing and terminal family from primary evidence.
- [ ] Check housing, locks, seals, and terminals for damage.
- [ ] Transfer observations to the [pinout working register](../../wiring/AMP-0001_pinout_working_register.md).
- [ ] Complete [VAL-0001](../../validation/VAL-0001_Amplifier_Connector_and_Pinout_Validation.md).

Unchecked items and blank fields remain `V0 — Unknown`.
