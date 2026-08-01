# OFRP Agent Instructions

## Project

Open Fender Retrofit Project (OFRP), documenting the retrofit of an OEM
Panasonic Fender audio system into a 2015 India-specification Volkswagen Jetta
PQ35 with a 7-inch MIB2 Composition Media head unit.

## Known hardware

- Panasonic Fender amplifier `5C6 035 456`, sourced from a 2014 US-spec Passat.
- OEM amplifier connector and a spare connector.
- OEM Fender speakers and tweeters.
- Known speaker part numbers include `5C6 035 453 A`, `5C6 035 453 B`, and
  `561 035 453 A`.

## Documentation rules

- Markdown is the source of truth.
- Follow `manual/OFRP-110_Engineering_Documentation_Standard.md`.
- Preserve semantic versioning and changelog history.
- Distinguish verified facts, measurements, OEM sources, community reports,
  and assumptions.
- Never present an unverified pinout or electrical claim as confirmed.
- Use the itemized validation workflow in
  `engineering/validation/VAL-0001_Amplifier_Connector_and_Pinout_Validation.md`
  before promoting amplifier wiring claims or authorizing a bench-power test.
- Do not commit generated PDF, DOCX, ZIP, or bundle files.
- Review changes before committing.
