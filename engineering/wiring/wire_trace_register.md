---
record_id: WIR-0002
title: Wire Trace Register
status: Draft
release: 0.3.0
owner: OFRP maintainers
last_updated: 2026-08-01
verification: V0
---

# WIR-0002 — Wire Trace Register

Record only observed or measured traces. `Unknown`, `Not tested`, and `Pending`
are required where evidence does not exist; blank cells must not imply a result.

| Wire ID | From component | From cavity | To component | To cavity | Color | Gauge | Measured resistance | Continuity verified | Polarity | Test record | Status |
|---|---|---|---|---|---|---|---|---|---|---|---|
| `WH-NNNN` | Unknown | Unknown | Unknown | Unknown | Unknown | Unknown | Not measured | No | Unknown | Pending | V0 — Not traced |

Measurements must identify instrument, range, lead-zero compensation, isolation
state, date, and operator in the linked test or measurement record. Continuity
alone does not establish circuit function or safe current capacity.
