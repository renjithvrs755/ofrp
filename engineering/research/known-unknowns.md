# Known Unknowns Register

This register tracks unresolved technical questions. Status and verification
terms follow [OFRP-110](../../manual/OFRP-110_Engineering_Documentation_Standard.md).

| ID | Question | Priority | Status | Owner | Verification | Evidence / next action |
|---|---|---|---|---|---|---|
| <a id="rr-0001"></a>RR-0001 | What is the verified pinout of amplifier `AMP-0001`? | Critical | Open | Unassigned | V0 | Identify connector and obtain an applicable OEM current-flow diagram before applying power. |
| <a id="rr-0002"></a>RR-0002 | How are the `CON-0001` cavities numbered for both mating-face and wire-entry views? | Critical | Open | Unassigned | V0 | Photograph both faces and correlate molded markings with applicable primary documentation. |
| <a id="rr-0003"></a>RR-0003 | Does `AMP-0001` require CAN-bus wake-up, a discrete remote signal, or another method? | High | Open | Unassigned | V0 | Evaluate [HYP-0001](hypothesis-register.md) using OEM documentation and a separately approved observation plan. |
| <a id="rr-0004"></a>RR-0004 | Which amplifier output, if any, maps to each available Fender speaker? | High | Open | Unassigned | V0 | Correlate OEM documentation, de-energized continuity, impedance, and later controlled signal evidence. |
| <a id="rr-0005"></a>RR-0005 | Which coding and adaptations are required for the MIB2-to-Fender configuration? | High | Open | Unassigned | V0 | Capture a baseline scan and identify a traceable equivalent OEM configuration. |
| <a id="rr-0006"></a>RR-0006 | What are the housing and terminal identities for `CON-0001`? | Critical | Open | Unassigned | V0 | Record molded marks and compare with manufacturer/OEM primary data. |
| <a id="rr-0007"></a>RR-0007 | What are the verified power, ground, protection, current, and thermal requirements for `AMP-0001`? | Critical | Open | Unassigned | V0 | Apply the two-source safety gate in `VAL-0001`; do not bench-power meanwhile. |
| <a id="rr-0008"></a>RR-0008 | What donor VIN, market, platform, and original configuration supplied `AMP-0001`? | Medium | Open | Unassigned | V0 | Seek seller/donor records; preserve the current Passat claim only as V1. |
| <a id="rr-0009"></a>RR-0009 | What audio-input transport and signal levels does `AMP-0001` accept? | High | Open | Unassigned | V0 | Evaluate [HYP-0002](hypothesis-register.md) using applicable OEM and measured evidence. |
| <a id="rr-0010"></a>RR-0010 | Is the DSP dataset vehicle-specific, and what dataset is present? | High | Open | Unassigned | V0 | Evaluate [HYP-0003](hypothesis-register.md) from diagnostic/OEM dataset evidence. |
| <a id="rr-0011"></a>RR-0011 | Does the short `CON-0001` pigtail retain enough evidence to reconstruct the complete harness? | High | Open | Unassigned | V0 | Inventory cavities and compare with the complete applicable OEM diagram. |
| <a id="rr-0012"></a>RR-0012 | Do `5C6 035 456` suffix revisions use the same connector family and keying? | High | Open | Unassigned | V0 | Compare exact-revision primary data and directly observed connector interfaces. |
| <a id="rr-0013"></a>RR-0013 | Is there a conventional remote turn-on circuit in addition to, or instead of, CAN wake-up? | High | Open | Unassigned | V0 | Review applicable OEM diagram and validate wake behavior without assuming absence from a forum report. |
| <a id="rr-0014"></a>RR-0014 | Do pins 3–22 on `AMP-0001` implement all ten `SRC-0002` reported output pairs? | Critical | Open | Unassigned | V0 for specimen; V1 source report | Establish orientation, perform `TEST-0002`, obtain OEM evidence, then use controlled output checks. |
| <a id="rr-0015"></a>RR-0015 | What are the individual functions of pins 1, 2, and 23–38? | Critical | Open | Unassigned | V0 | Resolve each pin independently; do not assign the group to power, ground, CAN, inputs, or control by elimination. |
| <a id="rr-0016"></a>RR-0016 | Does the owned system use separately amplified front woofer, midrange, and tweeter channels? | High | Open | Unassigned | V0 for specimen; V1 source report | Correlate speaker inventory, OEM topology, passive results, and later controlled signal tests. |
| <a id="rr-0017"></a>RR-0017 | Is the available subwoofer dual-coil and independently driven by the two reported pairs? | High | Open | Unassigned | V0 for specimen; V1 source report | Inspect/identify the subwoofer and correlate coil resistance with OEM and controlled output evidence. |
| <a id="rr-0018"></a>RR-0018 | What precisely does the TDIClub thread report about platform, wiring, wake-up, radio, coding, and speakers? | Medium | Open | Unassigned | V0 | Revisit `SRC-0001` when source access is available and record post author, date, number, and permalink. |
