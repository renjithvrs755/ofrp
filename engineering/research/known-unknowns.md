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
