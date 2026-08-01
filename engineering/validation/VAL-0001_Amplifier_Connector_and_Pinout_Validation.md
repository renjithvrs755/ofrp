---
record_id: VAL-0001
title: Amplifier Connector and Pinout Validation Plan
status: Draft
release: 0.3.0
owner: OFRP maintainers
last_updated: 2026-08-01
verification: V0 — Not executed
---

# VAL-0001 — Amplifier Connector and Pinout Validation

## Objective

Establish a repeatable, reviewable evidence chain for `AMP-0001` and `CON-0001`
connector orientation, cavity numbering, population, retained wire observations,
continuity relationships, and candidate circuit classes. This plan does not
authorize bench power and does not validate vehicle compatibility or coding.

## Hazards

- Incorrect power or ground may destroy the amplifier or test equipment and may
  overheat wiring or start a fire.
- Stored or externally supplied energy may cause shorts, arcing, or injury.
- Meter current or voltage may damage electronic inputs and communication pins.
- Oversized probes can spread terminals, create intermittent connections, or
  short adjacent cavities.
- Incorrect connector orientation can mirror every assignment.
- Loudspeaker drive or resistance-test signals can damage speakers or hearing.
- Depinning can damage locks, seals, housings, terminals, and evidence.

> **WARNING:** Do not apply 12–14.4 V to any amplifier cavity until battery
> positive and ground assignments are supported by at least two independent
> evidence sources, one of which must be OEM documentation or direct physical
> verification.

## Required tools

| Tool | Requirement | Status |
|---|---|---|
| Camera with macro capability | Legible label, cavity, key, pin, and wire images | Required; model not selected |
| Lighting and scale/color reference | Repeatable dimensional/color evidence | Required; not selected |
| Magnifier | Non-contact terminal inspection | Required; not selected |
| Digital multimeter | Resistance/continuity with known test voltage/current | Required; model/calibration unknown |
| Fine terminal-safe probes | Must not deform or bridge terminals | Required; size unknown pending terminal ID |
| Breakout/fixture | Individually protected access without loose probes | Required before any powered test; not designed |
| ESD controls | Appropriate mat/strap/storage for handling | Required; not documented |
| Current-limited bench supply and fuse | Reserved for later `TEST-0001` only | Prohibited until prerequisites pass |

## Prerequisites

- [ ] `AMP-0001` and `CON-0001` are photographed and visibly inspected.
- [ ] All items are disconnected from vehicle, supply, battery, and speakers.
- [ ] Meter model, settings, test behavior, and calibration status are recorded.
- [ ] Probe fit is verified on a noncritical sample or by dimensional evidence.
- [ ] An applicable OEM source is acquired and its applicability recorded.
- [ ] Connector orientation and numbering have an independent review path.
- [ ] Working registers are copied or revision-controlled before observations.
- [ ] Operator understands stop conditions and evidence naming.

Failure of any prerequisite is a **Stop** for the affected procedure.

## Inspection sequence

1. Assign image IDs; photograph amplifier label and all enclosure faces.
2. Photograph amplifier pins and connector before cleaning or manipulation.
3. Record visible condition without interpreting function.
4. Photograph connector mating and wire-entry faces square to the camera.
5. Record latch, keys, molded indices, housing markings, and secondary lock.
6. Record each populated/empty cavity and each retained wire segment.
7. Identify housing/terminal family only from molded marks or traceable primary
   documentation; retain `V0` if evidence is insufficient.
8. Update `AMP-0001`, `CON-0001`, and `WIR-0001`, citing image IDs.

## Connector-orientation confirmation

Create separate annotated images for mating-face and wire-entry-face views.
Each must show `TOP`, latch/key position, viewing direction, connector ID, date,
and image ID. Derive numbering from visible molded marks and applicable primary
documentation, never from assumed left-to-right sequence. A reviewer must check
that the two views were mirrored correctly. Until both agree, all cavity fields
remain `Unknown` and the numbering validation fails.

## Continuity-testing procedure

1. Confirm all involved items are de-energized and isolated. Measure for
   unexpected voltage before selecting resistance/continuity mode.
2. Record meter, leads, range, test voltage/current if known, and lead resistance.
3. Use terminal-safe probes without forcing or scraping contact surfaces.
4. Test only a documented pair of endpoints; never sweep adjacent amplifier
   pins indiscriminately.
5. Record raw resistance rather than relying only on an audible indication.
6. Reverse leads where semiconductor behavior is suspected and record both
   results; do not interpret either result without supporting evidence.
7. Repeat the observation and, where practical, have a second operator review.
8. Enter the result in `WIR-0001` and `WIR-0002` with the test-record reference.
9. Stop on unstable values, unexpected voltage, heating, odor, visible damage,
   terminal movement, or evidence of an energized/connected module.

## Resistance checks

With `AMP-0001` isolated, resistance measurements may document candidate
relationships but must not alone assign power, ground, CAN, input, or speaker
function. Record polarity, range, elapsed settling time, open/over-range results,
repeatability, and uncertainty. Do not apply insulation-resistance or megohmmeter
test voltages. Instrument test energy must be assessed before probing electronics.

## Speaker-pair identification method

Do not connect a speaker, battery, tone generator, or amplifier supply during
this validation stage. Candidate speaker pairs may be proposed only when an
applicable OEM source and de-energized continuity/impedance evidence agree.
Record both conductors, destination speaker ID, measured resistance, polarity
evidence, and uncertainty. Wire color, similar resistance, or paired routing
alone is insufficient. Acoustic polarity and channel identity require a later
reviewed test plan.

## Power-pin identification constraints

Wire gauge, terminal size, PCB-plane appearance, continuity to chassis, and
internet pinouts are hypotheses, not independent confirmation by themselves.
Candidate battery-positive and ground assignments must each have at least two
independent evidence sources, including applicable OEM documentation or direct
physical verification. Document source applicability, measurement method, and
review. No powered confirmation is permitted under this plan.

## CAN-pair identification constraints

Twist, colors, routing, resistance, and apparent differential structure can
identify a candidate pair only (`V0/V1` as applicable); they do not establish
CAN, bus segment, high/low polarity, bit rate, termination role, or wake-up
behavior. Resolve assignments using applicable OEM documentation plus passive
observation in a known, safely instrumented configuration under a separate
approved test. Do not inject messages or apply bias voltage under this plan.

## Bench-power prohibition

`TEST-0001` must remain `Not Run`. Bench power is prohibited until:

1. battery-positive and ground assignments meet the two-source rule above;
2. connector orientation and numbering pass review;
3. pre-power resistance checks have acceptance criteria and pass;
4. voltage, polarity, current limit, fuse, wiring, wake method, and stop controls
   are documented and independently reviewed; and
5. a fused, current-limited, touch-safe breakout is inspected.

## Pass/fail criteria

| Area | Pass | Fail / unresolved |
|---|---|---|
| Images | All required views are legible, identified, and preserve orientation. | Missing/ambiguous view or unreadable marks. |
| Orientation | Mating and wire-entry maps reconcile and reviewer agrees. | Mirroring, key position, or numbering remains ambiguous. |
| Population | Every cavity is recorded with image evidence. | Any cavity cannot be observed or identified. |
| Continuity | Repeated raw results identify endpoints with method and uncertainty. | Result is unstable, unrepeatable, unsafe, or lacks endpoint identity. |
| Function proposal | Source and evidence level are explicit; contradictions logged. | Function stated as fact without sufficient evidence. |
| Power readiness | Every bench-power prerequisite passes and review is recorded. | Any prerequisite missing; bench power remains prohibited. |

An unresolved area is not a failure of the project; it remains `V0` and creates
or updates a research item. The overall validation result remains `Not Executed`
until the plan is completed and reviewed.

## Evidence-capture requirements

- Preserve original images; reference repository-safe derivatives by `IMG` ID.
- Record date, operator, specimen IDs, orientation, tools, settings, and ambient
  conditions relevant to each observation.
- Link raw readings and annotated diagrams to `WIR-0001`, `WIR-0002`, and the
  applicable test or measurement record.
- Record contradictions and failed/inconclusive checks; never overwrite them.
- Use repository-relative links and verification levels for every conclusion.

## Rollback and stop conditions

Stop immediately on unexpected voltage/current, smoke, odor, heat, noise,
sparking, unstable readings, damaged insulation, deformed terminals, incorrect
probe fit, loss of orientation, uncertain meter mode, or conflict between
evidence sources. Disconnect any external energy if safe, preserve the setup in
photographs, record the anomaly, quarantine damaged parts, and return changed
locks/fixtures to a documented safe state. Do not improvise a powered test.
