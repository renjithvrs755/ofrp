---
record_id: SRC-0002
title: the12volt 2012 Passat Fender Wiring Source Review
status: Draft — Direct Source Access Pending
release: 0.3.1
owner: OFRP maintainers
last_updated: 2026-08-03
verification: V1 — Community-reported work-item extraction
---

# SRC-0002 — the12volt 2012 Passat Fender Wiring

## Source metadata and confidence

| Field | Value |
|---|---|
| Source type | Community installation forum; not OEM documentation |
| Thread | [2012 Passat Fender wiring discussion](https://www.the12volt.com/installbay/forum_posts.asp?tid=132259) |
| Thread ID | `132259` |
| Access attempted | 2026-08-03 |
| Access result | Source unavailable to the research environment (`401/403`) |
| Extraction basis | Mapping supplied in the v0.3.1 work item and attributed there to this thread |
| Source confidence | Low pending direct post review, connector orientation, OEM corroboration, and physical validation |
| Evidence level | `V1 — Community-reported/unverified` |

No post author, displayed timestamp, post number, or permalink could be verified.
Those fields are required before this extraction can be considered a complete
source review.

## Evidence classification

- **Source-reported:** the 38-cavity description, ten output pairs, wire colors,
  under-seat location, and CAN wake statement below (`V1`).
- **Engineering inference:** possible roles for unresolved cavities and
  applicability across revisions (`V0`, hypothesis register only).
- **Physically verified:** none of this source's electrical claims have been
  verified on `AMP-0001` or `CON-0001`.
- **Unresolved:** orientation, all non-output assignments, exact donor/source
  configuration, post-level citations, and OEM corroboration.

## Reported system context

| Claim | Status | Limitation |
|---|---|---|
| The mapping concerns a reported 2012 Passat Fender system. | V1 — Community-reported | Exact market, platform, build configuration, amplifier suffix, and source post remain unverified. |
| The amplifier uses a 38-cavity connector. | V1 — Community-reported | `CON-0001` cavity count and keying have not been physically recorded. |
| The amplifier location is reported as beneath the driver seat. | V1 — Community-reported | Direct thread text and donor applicability were not accessible; must be rechecked before use. |
| Wake-up is reported to occur over CAN. | V1 — Community-reported | Exact bus, pins, messages, termination, and absence of a discrete remote wire are unverified. |

## Reported 38-pin output mapping

Every row is `V1 — Community-reported/unverified`, is not OEM-confirmed, and is
only a candidate for `AMP-0001` until exact connector, amplifier, and vehicle
applicability are established.

| Channel | Positive pin | Negative pin | Positive wire colour | Negative wire colour | Evidence |
|---|---:|---:|---|---|---|
| Left front woofer | 18 | 6 | Brown/green | Brown/blue | V1 — SRC-0002 work-item extraction |
| Left front midrange | 13 | 14 | Blue/black | White/black | V1 — SRC-0002 work-item extraction |
| Left front tweeter | 8 | 20 | White | White/black | V1 — SRC-0002 work-item extraction |
| Right front woofer | 15 | 3 | Brown/red | Brown/black | V1 — SRC-0002 work-item extraction |
| Right front midrange | 12 | 11 | Red/gray | Brown/gray | V1 — SRC-0002 work-item extraction |
| Right front tweeter | 19 | 7 | Gray | Gray/black | V1 — SRC-0002 work-item extraction |
| Left rear speaker | 9 | 21 | Red/white | Brown/white | V1 — SRC-0002 work-item extraction |
| Right rear speaker | 22 | 10 | Red/purple | Brown/purple | V1 — SRC-0002 work-item extraction |
| Subwoofer coil 1 | 16 | 4 | White/red | Brown/red | V1 — SRC-0002 work-item extraction |
| Subwoofer coil 2 | 5 | 17 | Gray/red | Gray/brown | V1 — SRC-0002 work-item extraction |

## Unresolved cavities and functions

- Pins **1, 2, and 23–38**: exact functions unresolved (`V0`).
- Battery positive, ground, CAN high/low, any discrete wake/control, four
  reported radio audio-input pairs, coding, diagnostics, and all other control
  assignments: exact pins unresolved (`V0`).
- Connector viewing direction and whether the reported numbering is mating-face
  or wire-entry-face: unresolved (`V0`).

The unresolved group must not be summarized as containing particular functions;
that grouping is tracked separately as an engineering hypothesis.

## Contradictions and uncertainty

- The reported colors `white/black` and `brown/red` each appear on more than one
  reported circuit. Color therefore cannot uniquely identify a cavity/function.
- Reported positive/negative labels have not been checked against connector
  orientation, vehicle harness, speaker polarity, or amplifier topology.
- The thread's exact amplifier part number/suffix and whether all claims refer
  to one vehicle/configuration could not be checked.
- CAN wake reporting does not prove the absence of a discrete remote circuit.

## Applicability and cross-references

The report concerns a community-described 2012 Passat system, not the target
Jetta. It does not prove that [AMP-0001](../../components/amplifiers/AMP-0001_Panasonic_5C6035456.md)
or [CON-0001](../../components/connectors/CON-0001_Panasonic_Fender_Amplifier_Connector.md)
uses this mapping. See the [working output map](../../wiring/AMP-0001_reported_38pin_output_map.md)
and [VAL-0001](../../validation/VAL-0001_Amplifier_Connector_and_Pinout_Validation.md).

> **SAFETY GATE — NO POWER:** Do not apply power to the amplifier until:
> - connector orientation is verified,
> - battery positive is verified,
> - ground is verified,
> - no output pin is shorted, and
> - supply is fused and current-limited.
