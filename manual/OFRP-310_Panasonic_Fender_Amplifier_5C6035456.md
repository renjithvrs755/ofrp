---
document_id: OFRP-310
title: Panasonic Fender Amplifier 5C6 035 456 Dossier
revision: 0.2
status: Draft
release: 0.3.1
owner: OFRP maintainers
last_updated: 2026-08-03
verification: V0/V1/V3 as itemized
---

# OFRP-310 — Panasonic Fender Amplifier 5C6 035 456

## Purpose and scope

This dossier controls the identity, observations, hypotheses, and evidence gaps
for amplifier specimen [AMP-0001](../engineering/components/amplifiers/AMP-0001_Panasonic_5C6035456.md).
It is a validation work surface, not an installation guide or a final pinout.
Verification levels follow [OFRP-110](OFRP-110_Engineering_Documentation_Standard.md#6-evidence-and-verification-levels).

## Known hardware identity and label details

| Attribute | Recorded value | Status | Evidence / limitation |
|---|---|---|---|
| Component ID | `AMP-0001` | V3 — Observed | Project inventory assignment; applies only to the owned specimen. |
| OEM part number | `5C6 035 456` | V3 — Observed | Read from the amplifier label; label photograph remains required. |
| Manufacturer | Panasonic | V3 — Observed | Read from the amplifier label; label photograph remains required. |
| Label description | `10CH Audio Amplifier` | V3 — Observed | Read from the amplifier label; this text does not by itself prove ten independent outputs. |
| Product-family description | Fender amplifier | V1 — Reported | Seller/project description; a traceable OEM applicability source remains required. |
| Seller-reported donor | Working 2014 Passat | V1 — Reported | Seller statement only; donor VIN, market, platform, and vehicle records were not supplied. |
| Donor market/platform | Unknown | V0 — Unknown | Must not be inferred from model year or part-number prefix. |
| Associated connector | `CON-0001` | V3 — Observed | Connector is in project possession. |
| Original wiring remaining | A few centimetres | V3 — Observed | Short pigtails are available; colors and cavity locations are not yet recorded. |

## Physical inspection checklist

- [ ] Capture the complete label as `IMG-NNNN` without obscuring identifiers.
- [ ] Record all hardware/software, serial, date, and supplier fields verbatim.
- [ ] Photograph every enclosure face, connector interface, and mounting point.
- [ ] Check for cracked housing, corrosion, contamination, water marks, heat
      discoloration, impact damage, missing fasteners, or prior opening.
- [ ] Inspect pins with magnification for bending, recession, deposits, and
      evidence of arcing; do not probe or straighten pins during photography.
- [ ] Measure dimensions and mass and record the instruments used.
- [ ] Record mounting brackets, isolators, fasteners, and orientation markings.
- [ ] Link observations to the component record and image IDs.

Unchecked items are `V0 — Unknown`; a checked item must link to evidence before
its result is promoted to `V3 — Observed`.

## Connector overview

`CON-0001` is the connector presently associated with `AMP-0001` (`V3 —
Observed`). It retains only short pieces of original wiring (`V3 — Observed`).
Housing identity, terminal family, cavity count, keying, cavity numbering,
population, and every circuit assignment remain `V0 — Unknown`. See the
[connector record](../engineering/components/connectors/CON-0001_Panasonic_Fender_Amplifier_Connector.md)
and [pinout working register](../engineering/wiring/AMP-0001_pinout_working_register.md).

`SRC-0002` reports a 38-cavity connector and output functions on pins 3–22 for
a described 2012 Passat Fender system (`V1 — Community-reported/unverified`).
This does not establish `CON-0001` cavity count, orientation, population, or
applicability. Pins 1, 2, and 23–38 and every power, ground, CAN, input, wake,
and control assignment remain unresolved (`V0`).

## Power and communication hypotheses

| Hypothesis | Status | Validation route |
|---|---|---|
| Battery-positive and ground circuits exist at presently unidentified cavities. | V0 — Unknown | OEM documentation plus direct connector/PCB or controlled electrical verification under `VAL-0001`. |
| The amplifier requires CAN-based wake-up (`HYP-0001`). | V0 — Unknown | Identify any candidate differential pair without energizing; correlate OEM documentation and later capture communication during an approved test. |
| A discrete wake circuit may be present. | V0 — Unknown | Do not assume; resolve from OEM documentation and observed circuit behavior. |
| Audio may enter as analog differential or high-level signals (`HYP-0002`). | V0 — Unknown | Resolve from OEM documentation and signal measurements in a known donor-equivalent configuration. |

No voltage, polarity, fuse value, current requirement, CAN assignment, wake
method, or audio-input assignment is established by this document.

## Output-channel hypotheses

The label text `10CH Audio Amplifier` is an observed label detail (`V3`), but
channel count, topology, bridged pairs, load limits, speaker destinations,
polarity, and subwoofer allocation are all `V0 — Unknown`. No cavity may be
treated as a speaker output until supported by traceable evidence and recorded
testing. See `RR-0004` and the pinout working register.

## Compatibility notes

Compatibility of `AMP-0001` with the target Jetta, MIB2 head unit, available
speakers, connector family, software dataset, coding, component protection, and
vehicle networks is `V0 — Unknown`. Seller-reported Passat provenance (`V1`)
does not establish compatibility. Revision-sharing and dataset assumptions are
tracked as `HYP-0003` and `HYP-0005`.

## Verification status

| Area | Current status | Governing record / next evidence |
|---|---|---|
| Specimen identity and visible label text | V3 — Observed; image pending | `AMP-0001`; full label photograph |
| Seller-reported provenance | V1 — Reported | Purchase correspondence; donor records if obtainable |
| Physical condition | V0 — Unknown | Complete inspection checklist and photographs |
| Connector identity and numbering | V0 — Unknown | `CON-0001`, `RR-0002`, OEM connector documentation |
| Pinout, power, and ground | V0 — Unknown | `RR-0001`, `VAL-0001` |
| Wake-up and communication | V0 — Unknown | `RR-0003`, `HYP-0001`, controlled test evidence |
| Audio inputs and output mapping | V0 — Unknown | `HYP-0002`, `RR-0004`, continuity/signal evidence |
| Dataset, coding, and vehicle compatibility | V0 — Unknown | `HYP-0003`, `RR-0005`, OEM/diagnostic evidence |

## Safety warnings

> **WARNING:** This dossier contains hypotheses, not an approved pinout. An
> incorrect connection can damage the amplifier, vehicle electronics, wiring,
> test equipment, or power source and may create an overheating or fire hazard.

> **WARNING:** Do not apply 12–14.4 V to any amplifier cavity until battery
> positive and ground assignments are supported by at least two independent
> evidence sources, one of which must be OEM documentation or direct physical
> verification.

> **SAFETY GATE — NO POWER:** Do not apply power to the amplifier until:
> - connector orientation is verified,
> - battery positive is verified,
> - ground is verified,
> - no output pin is shorted, and
> - supply is fused and current-limited.

Do not infer cavity numbering from viewing direction, wire color, wire size,
adjacent cavities, internet diagrams, or another suffix revision. Do not use a
multimeter resistance or continuity mode on an energized circuit.

## Known unknowns

- `RR-0001`: complete amplifier pinout.
- `RR-0002`: connector cavity numbering and orientation.
- `RR-0003`: communication and wake-up behavior.
- `RR-0004`: output-to-speaker mapping.
- `RR-0005`: MIB2 coding and adaptations.
- `RR-0006`: connector housing and terminal identity.
- `RR-0007`: power, ground, protection, and current requirements.
- `RR-0008`: donor identity, market, platform, and original configuration.

## Required evidence

1. Dated, readable images of the amplifier label, enclosure, mounting points,
   pins, connector mating face, wire-entry face, and each retained pigtail.
2. An applicable OEM current-flow diagram or equivalent primary documentation,
   with vehicle applicability and revision recorded.
3. Connector housing and terminal identification supported by molded markings
   or manufacturer/OEM documentation.
4. Cavity orientation and numbering established before wire colors are mapped.
5. Repeatable continuity/resistance records made with all items de-energized.
6. A reviewed validation record and completed test record before any bench
   power application.
7. Diagnostic and signal evidence for wake-up, audio input, coding, and dataset
   claims in a documented configuration.

## Revision history

| Revision | Date | Status | Change |
|---|---|---|---|
| 0.1 | 2026-08-01 | Draft | Initial validation dossier; no pinout published. |
| 0.2 | 2026-08-03 | Draft | Added community-reported output-map references; power, ground, CAN, inputs, and orientation remain unresolved. |
