# Known Unknowns Register

This register tracks unresolved technical questions. Status and verification
terms follow [OFRP-110](../../manual/OFRP-110_Engineering_Documentation_Standard.md).

| ID | Question | Priority | Status | Owner | Verification | Evidence / next action |
|---|---|---|---|---|---|---|
| RR-0001 | What is the verified pinout of amplifier `AMP-0001`? | Critical | Open | Unassigned | V0 | Identify connector and obtain OEM current-flow diagram before applying power. |
| RR-0002 | How are the amplifier connector cavities numbered in the installed orientation? | Critical | Open | Unassigned | V0 | Photograph connector faces and correlate molded markings with OEM documentation. |
| RR-0003 | Does `AMP-0001` require CAN-bus wake-up, a discrete remote signal, or both? | High | Open | Unassigned | V0 | Review OEM diagram, then create a current-limited bench test. |
| RR-0004 | Which amplifier output maps to each Fender speaker? | High | Open | Unassigned | V0 | Correlate OEM diagram, harness continuity, and speaker impedance measurements. |
| RR-0005 | Which coding and adaptations are required for the MIB2-to-Fender configuration? | High | Open | Unassigned | V0 | Capture baseline scan and identify an equivalent OEM vehicle configuration. |
