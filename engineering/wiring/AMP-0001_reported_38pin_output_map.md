---
record_id: WIR-0003
title: AMP-0001 Reported 38-Pin Output Map
status: Draft — Community Report Only
release: 0.3.1
owner: OFRP maintainers
last_updated: 2026-08-03
verification: V1 — Community-reported/unverified
---

# WIR-0003 — AMP-0001 Reported 38-Pin Output Map

> **WARNING — NOT A VERIFIED PINOUT:** Connector orientation is not verified.
> This candidate map is community-reported for a 2012 Passat Fender system, is
> not OEM-confirmed, and has not been physically verified on `AMP-0001` or
> `CON-0001`. Do not wire or energize from this map.

> **SAFETY GATE — NO POWER:** Do not apply power to the amplifier until:
> - connector orientation is verified,
> - battery positive is verified,
> - ground is verified,
> - no output pin is shorted, and
> - supply is fused and current-limited.

## Reported channel grouping and topology

| Group | Channel | Positive cavity/colour | Negative cavity/colour | Status |
|---|---|---|---|---|
| Front left | Woofer | 18 — brown/green | 6 — brown/blue | V1 — SRC-0002 |
| Front left | Midrange | 13 — blue/black | 14 — white/black | V1 — SRC-0002 |
| Front left | Tweeter | 8 — white | 20 — white/black | V1 — SRC-0002 |
| Front right | Woofer | 15 — brown/red | 3 — brown/black | V1 — SRC-0002 |
| Front right | Midrange | 12 — red/gray | 11 — brown/gray | V1 — SRC-0002 |
| Front right | Tweeter | 19 — gray | 7 — gray/black | V1 — SRC-0002 |
| Rear | Left speaker | 9 — red/white | 21 — brown/white | V1 — SRC-0002 |
| Rear | Right speaker | 22 — red/purple | 10 — brown/purple | V1 — SRC-0002 |
| Subwoofer | Coil 1 | 16 — white/red | 4 — brown/red | V1 — SRC-0002 |
| Subwoofer | Coil 2 | 5 — gray/red | 17 — gray/brown | V1 — SRC-0002 |

The table reports separately amplified woofer, midrange, and tweeter pairs for
each front side, one pair per rear speaker, and two subwoofer-coil pairs. That
topology remains a `V1` report, not a physical finding about the owned system.

## Unresolved connector cavities

Pins 1, 2, and 23–38 are unresolved (`V0`). Power, ground, CAN, audio input,
wake/control, coding, and diagnostic assignments are unresolved (`V0`) and are
not assigned to that pin group. Viewing orientation is also unresolved (`V0`).

## Source references

- [SRC-0002](../research/source-reviews/SRC-0002_The12Volt_2012_Passat_Fender_Wiring.md)
- [Pinout working register](AMP-0001_pinout_working_register.md)
- [Passive validation plan](../validation/VAL-0001_Amplifier_Connector_and_Pinout_Validation.md)

## Validation checklist

- [ ] Photograph both connector faces with latch/key orientation.
- [ ] Establish molded numbering and reconcile mating/wire-entry views.
- [ ] Confirm `CON-0001` has 38 cavities without assuming this source applies.
- [ ] Record every retained pigtail colour under neutral lighting.
- [ ] Run `TEST-0002` de-energized for each reported pair.
- [ ] Record pin-to-chassis and channel-to-channel isolation results.
- [ ] Obtain an applicable OEM current-flow diagram.
- [ ] Resolve contradictions before promoting any row beyond `V1`.
