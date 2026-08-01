# Engineering Decision Log

## EDL-0001
Status: Accepted

Decision:
Use the OEM Panasonic Fender amplifier.

Reason:
- Matching OEM Fender speakers already available.
- OEM DSP tuning.
- Lower total retrofit cost than replacing the speaker system.

## EDL-0002
Status: Accepted

Decision:
Prohibit bench power to `AMP-0001` until battery-positive and ground
assignments have at least two independent supporting evidence sources, one of
which is OEM documentation or direct physical verification, and the remaining
`VAL-0001` power-readiness gates have passed review.

Reason:
- The current pinout, cavity numbering, protection, and power requirements are
  all `V0 — Unknown`.
- An incorrect assignment could damage equipment or create a heat/fire hazard.
- Separating passive validation from powered testing preserves evidence and
  makes the eventual test repeatable and reviewable.
