---
record_id: WIR-0001
title: AMP-0001 Pinout Working Register
status: Draft — Community Report Only
release: 0.3.1
owner: OFRP maintainers
last_updated: 2026-08-03
verification: V0/V1 as itemized
---

# WIR-0001 — AMP-0001 Pinout Working Register

This is an evidence worksheet, not an approved pinout or wiring diagram.
Connector orientation and numbering are not physically established. Pins 3–22
below reproduce the `SRC-0002` community report for a described 2012 Passat
Fender system; applicability to `AMP-0001` and `CON-0001` is unverified.

| Connector ID | Cavity number | Observed terminal populated | Original wire color | Wire gauge estimate | Proposed function | Source | Verification level | Continuity result | Destination | Notes |
|---|---|---|---|---|---|---|---|---|---|---|
| `CON-0001` | 3 | Unknown | Brown/black (reported) | Unknown | Right front woofer negative (reported) | [SRC-0002](../research/source-reviews/SRC-0002_The12Volt_2012_Passat_Fender_Wiring.md) | V1 — Community-reported/unverified | Not tested | Unknown | Viewing orientation unresolved. |
| `CON-0001` | 4 | Unknown | Brown/red (reported) | Unknown | Subwoofer coil 1 negative (reported) | SRC-0002 | V1 — Community-reported/unverified | Not tested | Unknown | Viewing orientation unresolved. |
| `CON-0001` | 5 | Unknown | Gray/red (reported) | Unknown | Subwoofer coil 2 positive (reported) | SRC-0002 | V1 — Community-reported/unverified | Not tested | Unknown | Viewing orientation unresolved. |
| `CON-0001` | 6 | Unknown | Brown/blue (reported) | Unknown | Left front woofer negative (reported) | SRC-0002 | V1 — Community-reported/unverified | Not tested | Unknown | Viewing orientation unresolved. |
| `CON-0001` | 7 | Unknown | Gray/black (reported) | Unknown | Right front tweeter negative (reported) | SRC-0002 | V1 — Community-reported/unverified | Not tested | Unknown | Viewing orientation unresolved. |
| `CON-0001` | 8 | Unknown | White (reported) | Unknown | Left front tweeter positive (reported) | SRC-0002 | V1 — Community-reported/unverified | Not tested | Unknown | Viewing orientation unresolved. |
| `CON-0001` | 9 | Unknown | Red/white (reported) | Unknown | Left rear speaker positive (reported) | SRC-0002 | V1 — Community-reported/unverified | Not tested | Unknown | Viewing orientation unresolved. |
| `CON-0001` | 10 | Unknown | Brown/purple (reported) | Unknown | Right rear speaker negative (reported) | SRC-0002 | V1 — Community-reported/unverified | Not tested | Unknown | Viewing orientation unresolved. |
| `CON-0001` | 11 | Unknown | Brown/gray (reported) | Unknown | Right front midrange negative (reported) | SRC-0002 | V1 — Community-reported/unverified | Not tested | Unknown | Viewing orientation unresolved. |
| `CON-0001` | 12 | Unknown | Red/gray (reported) | Unknown | Right front midrange positive (reported) | SRC-0002 | V1 — Community-reported/unverified | Not tested | Unknown | Viewing orientation unresolved. |
| `CON-0001` | 13 | Unknown | Blue/black (reported) | Unknown | Left front midrange positive (reported) | SRC-0002 | V1 — Community-reported/unverified | Not tested | Unknown | Viewing orientation unresolved. |
| `CON-0001` | 14 | Unknown | White/black (reported) | Unknown | Left front midrange negative (reported) | SRC-0002 | V1 — Community-reported/unverified | Not tested | Unknown | Viewing orientation unresolved. |
| `CON-0001` | 15 | Unknown | Brown/red (reported) | Unknown | Right front woofer positive (reported) | SRC-0002 | V1 — Community-reported/unverified | Not tested | Unknown | Viewing orientation unresolved. |
| `CON-0001` | 16 | Unknown | White/red (reported) | Unknown | Subwoofer coil 1 positive (reported) | SRC-0002 | V1 — Community-reported/unverified | Not tested | Unknown | Viewing orientation unresolved. |
| `CON-0001` | 17 | Unknown | Gray/brown (reported) | Unknown | Subwoofer coil 2 negative (reported) | SRC-0002 | V1 — Community-reported/unverified | Not tested | Unknown | Viewing orientation unresolved. |
| `CON-0001` | 18 | Unknown | Brown/green (reported) | Unknown | Left front woofer positive (reported) | SRC-0002 | V1 — Community-reported/unverified | Not tested | Unknown | Viewing orientation unresolved. |
| `CON-0001` | 19 | Unknown | Gray (reported) | Unknown | Right front tweeter positive (reported) | SRC-0002 | V1 — Community-reported/unverified | Not tested | Unknown | Viewing orientation unresolved. |
| `CON-0001` | 20 | Unknown | White/black (reported) | Unknown | Left front tweeter negative (reported) | SRC-0002 | V1 — Community-reported/unverified | Not tested | Unknown | Viewing orientation unresolved. |
| `CON-0001` | 21 | Unknown | Brown/white (reported) | Unknown | Left rear speaker negative (reported) | SRC-0002 | V1 — Community-reported/unverified | Not tested | Unknown | Viewing orientation unresolved. |
| `CON-0001` | 22 | Unknown | Red/purple (reported) | Unknown | Right rear speaker positive (reported) | SRC-0002 | V1 — Community-reported/unverified | Not tested | Unknown | Viewing orientation unresolved. |

Pins 1, 2, and 23–38 remain unresolved (`V0`) and have no proposed function.
Power, ground, CAN, audio-input, wake, and control pins remain unresolved (`V0`).

> **WARNING:** Do not infer power, ground, communication, input, or output
> functions from wire color, gauge, cavity position, or an unverified diagram.
> Each proposed function requires a traceable source and verification level.

> **SAFETY GATE — NO POWER:** Do not apply power to the amplifier until:
> - connector orientation is verified,
> - battery positive is verified,
> - ground is verified,
> - no output pin is shorted, and
> - supply is fused and current-limited.
