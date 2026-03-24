# Proof Project 2: Data Quality Gate

## Summary
A lightweight service that validates incoming data against rules and blocks bad records while providing actionable error reports.

## Scope
- Input: CSV upload or API POST.
- Rules: required fields, regex format, numeric ranges, referential checks.
- Output: pass/fail report + cleaned output.

## Key Capabilities
- **Rule engine**: JSON/YAML rule definitions.
- **Reports**: per‑row error details + summary stats.
- **Integration**: returns cleaned file or rejects payload.

## Deliverables
- Web UI or CLI to submit data and view results.
- Example rule packs for common use cases.
- README with quickstart and demo steps.

## Acceptance Criteria
- At least 5 validation rules across required/regex/range checks.
- Report includes row‑level error details + summary stats.
- Clean output file generated for passing rows only.
