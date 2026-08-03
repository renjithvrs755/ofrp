---
record_id: WIR-0004
title: AMP-0001 Working System Topology
status: Draft — Community Report and Hypotheses
release: 0.3.1
owner: OFRP maintainers
last_updated: 2026-08-03
verification: V0/V1 as labeled
---

# WIR-0004 — AMP-0001 Working System Topology

> **WARNING:** This is not an approved wiring diagram. Output pairs are `V1`
> community reports from `SRC-0002`; all exact input, CAN, power, ground, and
> control pins are unresolved (`V0`). Connector orientation is unresolved.

```text
MIB/radio [identity/configuration unresolved]
   |
   +-- 4 reported audio input pairs [V1 report; exact pins unresolved V0]
   +-- Infotainment CAN [V1 hypothesis; exact pins unresolved V0]
   +-- Power/ground/control relationships [unresolved V0]
   |
   v
Panasonic 5C6 035 456 / AMP-0001 [applicability not established]
   |
   +-- LF woofer:    18 /  6 [V1 SRC-0002]
   +-- LF midrange:  13 / 14 [V1 SRC-0002]
   +-- LF tweeter:     8 / 20 [V1 SRC-0002]
   +-- RF woofer:    15 /  3 [V1 SRC-0002]
   +-- RF midrange:  12 / 11 [V1 SRC-0002]
   +-- RF tweeter:   19 /  7 [V1 SRC-0002]
   +-- LR speaker:     9 / 21 [V1 SRC-0002]
   +-- RR speaker:   22 / 10 [V1 SRC-0002]
   +-- Sub coil 1:   16 /  4 [V1 SRC-0002]
   +-- Sub coil 2:     5 / 17 [V1 SRC-0002]
```

The diagram does not establish signal direction, electrical levels, polarity,
channel loading, crossover behavior, CAN bus identity, or wake-up behavior.

> **SAFETY GATE — NO POWER:** Do not apply power to the amplifier until:
> - connector orientation is verified,
> - battery positive is verified,
> - ground is verified,
> - no output pin is shorted, and
> - supply is fused and current-limited.
