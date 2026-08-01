---
document_id: OFRP-110
title: Engineering Documentation Standard
revision: 1.0
status: Approved
release: 0.2.0
owner: OFRP maintainers
last_updated: 2026-08-01
---

# OFRP-110 — Engineering Documentation Standard

## 1. Purpose

This standard defines how OFRP engineering information is identified, written,
supported, reviewed, changed, and validated. It applies to all project manuals,
hardware records, wiring information, research, decisions, tests, measurements,
and media added after its approval.

The standard exists to ensure that a reader can determine:

1. what is known;
2. how it is known;
3. which physical item or configuration a statement concerns;
4. whether the information has been independently checked; and
5. what changed and why.

## 2. Source of truth and repository layout

Markdown files in the Git repository are the source of truth. Generated
artifacts such as PDF, DOCX, ZIP, and repository bundles are release outputs and
must not be committed.

| Path | Purpose |
|---|---|
| `manual/` | Controlled project and technical documents |
| `engineering/decisions/` | Engineering decisions and their rationale |
| `engineering/research/` | Research questions and evidence tracking |
| `engineering/build-log/` | Chronological records of work on the vehicle or bench |
| `engineering/tests/` | Test plans and raw or summarized test results |
| `engineering/validation/` | Validation records against defined acceptance criteria |
| `engineering/measurements/` | Measurement records and instrument details |
| `engineering/context/` | Imported context that is not itself verified evidence |
| `assets/diagrams/` | Project-created diagrams |
| `assets/photos/` | Original project photographs |
| `assets/scans/` | Scans of labels or documents the project may distribute |
| `assets/datasheets/` | Distributable manufacturer data sheets |
| `assets/screenshots/` | Diagnostic and software screenshots |
| `knowledge/` | Shared terminology, abbreviations, and references |
| `history/` | Release notes, meeting notes, and retrospectives |
| `templates/` | Approved templates for repeatable records |

Use lowercase directory names. Controlled manual filenames use
`<document-id>_<descriptive_title>.md`; record filenames use
`<record-id>_<short-description>.md`. Use ASCII letters, digits, hyphens, and
underscores only. Do not encode a revision in a filename: Git and document
metadata preserve revision history.

## 3. Document numbering

Controlled documents have a permanent `OFRP-NNN` identity.

| Range | Subject |
|---|---|
| `OFRP-100–199` | Project governance and documentation standards |
| `OFRP-200–299` | System architecture and requirements |
| `OFRP-300–309` | Hardware overview and inventory |
| `OFRP-310–319` | Amplifier |
| `OFRP-320–329` | Speakers and subwoofer |
| `OFRP-330–339` | Head unit and source equipment |
| `OFRP-340–349` | Connectors and terminals |
| `OFRP-400–499` | Wiring, power, grounding, and networks |
| `OFRP-500–599` | Coding and configuration |
| `OFRP-600–699` | Diagnostics and troubleshooting |
| `OFRP-700–799` | Bench tests and validation procedures |
| `OFRP-900–999` | Appendices and reference material |

The next unused number in the applicable range is assigned and never reused,
even after a document is withdrawn.

## 4. Engineering identifiers

Physical items, evidence, and engineering records receive stable IDs on first
entry. IDs use a prefix, hyphen, and zero-padded four-digit sequence.

| Prefix | Entity | Example |
|---|---|---|
| `AMP` | Amplifier | `AMP-0001` |
| `HU` | Head unit | `HU-0001` |
| `SPK` | Speaker or tweeter | `SPK-0001` |
| `SUB` | Subwoofer | `SUB-0001` |
| `CON` | Connector | `CON-0001` |
| `HAR` | Harness | `HAR-0001` |
| `IMG` | Photograph, scan, or screenshot | `IMG-0001` |
| `MEAS` | Measurement record | `MEAS-0001` |
| `TEST` | Test record | `TEST-0001` |
| `VAL` | Validation record | `VAL-0001` |
| `EDL` | Engineering decision | `EDL-0001` |
| `RR` | Research item or known unknown | `RR-0001` |

References to an entity must use its ID. A part number does not replace an
engineering ID because multiple physical specimens may share a part number.

## 5. Required metadata

Each controlled manual document begins with YAML front matter containing:

```yaml
---
document_id: OFRP-NNN
title: Descriptive title
revision: 0.1
status: Draft
release: Unreleased
owner: Name or role
last_updated: YYYY-MM-DD
---
```

Allowed document statuses are `Draft`, `In Review`, `Approved`, `Superseded`,
and `Withdrawn`. Records use the fields in their approved template.

## 6. Evidence and verification levels

Every safety-relevant, electrical, compatibility, coding, and pinout claim must
carry a verification level or cite a record that supplies one.

| Level | Label | Minimum basis |
|---|---|---|
| `V0` | Unknown | Open question; no usable evidence |
| `V1` | Reported | Community report, seller statement, or uncorroborated secondary source |
| `V2` | Documented | Traceable OEM publication, manufacturer data, or authoritative technical source |
| `V3` | Observed | Direct inspection, continuity check, diagnostic scan, or project measurement recorded with method |
| `V4` | Validated | Repeatable project test meets documented acceptance criteria in the target configuration |

`V1` information must be described as reported, not as fact. Conflicting
evidence retains the lower applicable level until resolved. A higher level does
not make a result universal: the record must state relevant vehicle, hardware,
software, and test conditions.

Evidence citations use a repository-relative link or a bibliographic entry and,
where possible, page, section, connector, or test-record detail. Chat exports
are project context only; their technical claims begin at `V0` or `V1` until
supported independently.

## 7. Traceability

A controlled technical claim should link the chain that applies:

```text
research question → source or measurement → decision → implementation
                  → test result → validation record
```

Test and validation records identify all applicable hardware IDs, document
revisions, coding state, tools, conditions, expected result, actual result, and
supporting media. Research items are not closed until their resolution points
to evidence and affected documents are updated.

## 8. Review and approval

1. An author creates or updates a document and marks it `Draft`.
2. The author checks links, identifiers, evidence levels, and consistency with
   related records, then marks it `In Review`.
3. A reviewer checks technical claims against cited evidence and checks that
   warnings and uncertainty are explicit.
4. Review findings are corrected or tracked as open research items.
5. The owner marks the document `Approved` and records the change in
   `CHANGELOG.md` when it is release-facing.

The author may also be the reviewer for low-risk editorial changes. Pinouts,
power connections, coding steps, and procedures capable of damaging equipment
require a second-person review or an explicit statement that independent review
is still pending.

## 9. Validation methodology

Validation must be planned before a claim is promoted to `V4`. A validation
record defines:

- objective and requirement or claim under test;
- applicable hardware and configuration IDs;
- prerequisites and safety controls;
- instruments, including model and calibration status when relevant;
- procedure detailed enough to repeat;
- quantitative or observable acceptance criteria;
- raw results and supporting evidence;
- deviations, anomalies, and uncertainties;
- pass/fail outcome, date, operator, and reviewer.

A failed or inconclusive test is retained. It may invalidate a claim, create a
research item, or require a revised procedure, but it must not be silently
removed.

## 10. Change control and versioning

OFRP releases follow Semantic Versioning:

- **major**: incompatible architecture, process, or scope change;
- **minor**: new controlled content, subsystem, or capability;
- **patch**: corrections and clarifications with no intended technical change.

Document revisions use `major.minor`. Increase the major revision when an
approved technical meaning or mandatory process changes; increase the minor
revision for additive or editorial changes. Git commits provide the detailed
audit trail. `CHANGELOG.md` summarizes user-visible repository changes.

Changes are made on a feature branch, reviewed as a diff, committed with a
descriptive message, and submitted through a pull request. Superseded content
is retained in Git history; active documents link to replacements where needed.

## 11. Safety and uncertainty language

Use `DANGER` for an imminent risk of serious injury, `WARNING` for a potential
injury or major equipment-damage risk, `CAUTION` for lesser equipment risk, and
`NOTE` for important supporting information. Do not use confident language to
hide uncertainty. Unknown connector orientation, pin numbering, voltage,
polarity, or coding state must be recorded as an open research item before work
continues.

## 12. Definition of done

A controlled document is done for a release when:

- metadata and identifiers conform to this standard;
- all nontrivial technical claims have evidence and a verification level;
- cross-references and repository-relative links resolve;
- open questions are present in the research register;
- required review and validation states are explicit;
- the roadmap and changelog reflect the work; and
- no generated release artifact has been committed.
