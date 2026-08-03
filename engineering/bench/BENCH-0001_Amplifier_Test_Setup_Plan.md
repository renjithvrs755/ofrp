---
record_id: BENCH-0001
title: Amplifier Test Setup Plan
status: Draft — Power Prohibited
release: 0.3.1
owner: OFRP maintainers
last_updated: 2026-08-03
verification: V0 — Not executed
---

# BENCH-0001 — Amplifier Test Setup Plan

> **PROPOSAL, NOT AUTHORIZATION:** The initial supply values in this plan are
> future test proposals only. Battery-positive and ground cavities, connector
> orientation, wake-up, and electrical limits remain unresolved.

> **SAFETY GATE — NO POWER:** Do not apply power to the amplifier until:
> - connector orientation is verified,
> - battery positive is verified,
> - ground is verified,
> - no output pin is shorted, and
> - supply is fused and current-limited.

## Bench block diagram

```text
                          [CAN interface — placeholder]
                                      |
[MIB/radio — placeholder] -------- [isolated breakout]
                                      |
[regulated supply]--[E-stop]--[fuse]--+-- CON-0001 -- AMP-0001
                                      |
                       [meter/scope test points]
                                      |
                  [sacrificial speaker — disconnected initially]
```

No block implies a verified pin, voltage, signal, or interconnection.

## Required tools and controls

| Item | Requirement / current status |
|---|---|
| Regulated power supply | Current-limited with voltage/current logging; model pending |
| Inline fuse and holder | Touch-safe, adjacent to source; value pending approval |
| Current limit | Adjustable and verified with a dummy load before connection |
| Emergency disconnect | One action, clearly labeled, accessible to operator |
| Connector breakout | Fused/protected, strain-relieved, cavity-labeled only after orientation review |
| Digital multimeter | Known test energy, protected terminal-safe probes |
| Oscilloscope | Where available; isolated/differential measurement method must be reviewed |
| CAN interface | Placeholder; isolated and listen-only initially; exact bus/pins unknown |
| MIB/radio source | Placeholder; exact audio-input pins and signal levels unknown |
| Sacrificial speaker | Known impedance/rating; disconnected during initial power/diagnostics |
| Camera/logging | Capture setup, labels, readings, waveforms, and anomalies |

## Proposed initial powered-test values

| Parameter | Future proposal | Verification status |
|---|---|---|
| Supply voltage | 12.0 V initial | V0 — Engineering proposal; not an amplifier requirement |
| Current limit | 0.5 A initial | V0 — Engineering proposal; adequacy/behavior unknown |
| Inline fuse | 2 A for wake/diagnostic testing | V0 — Engineering proposal; not an OEM fuse rating |
| Speaker load | No speakers connected initially | Safety proposal; output behavior unknown |

These values are not authorization to apply power and must be reviewed after
B+, ground, polarity, connector orientation, resistance checks, and safe-current
expectations are independently established.

## Phased plan and gates

### Phase 0 — No-power passive phase

Photograph and orient the connector, map pigtail colors, complete `TEST-0002`,
measure candidate pairs to chassis and one another, resolve unexpected
continuity, and obtain applicable OEM evidence. **Exit:** reviewed passive data;
power remains prohibited if any prerequisite is unresolved.

### Phase 1 — Powered diagnostics phase

After the power gate only, use a reviewed breakout, emergency disconnect,
inline fuse, current limit, no speakers, and no speculative communication or
audio injection. Record inrush, idle current, voltage, heat, odor, noise, and
diagnostic behavior. **Exit:** stable behavior inside preapproved limits.

### Phase 2 — CAN wake-up phase

Only after the physical bus pair, polarity, voltage domain, and interface safety
are confirmed. Begin listen-only in a known configuration. Do not inject frames
until a separate message-level plan is reviewed. **Exit:** repeatable wake state
supported by captures; otherwise retain `V0`.

### Phase 3 — Audio injection phase

Only after input pins, topology, common-mode range, amplitude, and source ground
relationship are verified. Begin at minimum level with outputs unloaded and
observe DC/waveform behavior. **Exit:** controlled output appropriate for the
planned sacrificial load.

### Phase 4 — Speaker-output phase

Use `TEST-0003`, one sacrificial non-tweeter speaker, one eligible channel, and
minimum input level. Tweeter and subwoofer testing remains deferred until
crossover and load behavior are established. **Exit:** reviewed evidence, not a
generalized pinout claim.

## Evidence-capture plan

- Photograph the complete bench before and after every configuration change.
- Record document revisions, specimen IDs, breakout diagram, wire IDs, cavity
  orientation evidence, supply/fuse/current-limit settings, instruments, date,
  operator, and reviewer.
- Preserve raw meter, supply, oscilloscope, CAN, diagnostic, thermal, and audio
  captures with stable evidence IDs.
- Log failed, stopped, contradictory, and inconclusive runs without deletion.
- Update `WIR-0001`, `WIR-0002`, `VAL-0001`, and research items only to the
  verification level supported by the evidence.
