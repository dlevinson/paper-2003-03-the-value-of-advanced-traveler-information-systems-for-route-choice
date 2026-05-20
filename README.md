# The Value of Advanced Traveler Information Systems for Route Choice

## Bibliographic Information

- Row ID: `paper-2003-03`
- Authors: David M. Levinson
- Venue: Transportation Research Part C 11(1):75-87 (2003)
- DOI: https://doi.org/10.1016/S0968-090X(02)00023-2
- Citation: Levinson, David M. (2003). The Value of Advanced Traveler Information Systems for Route Choice. Transportation Research Part C 11(1):75-87. https://doi.org/10.1016/S0968-090X(02)00023-2

## Package Boundary

This is a public upload candidate for the paper-specific legacy Excel/VBA simulation model. The inspected paper describes a stylized two-link queueing simulation for recurrent and non-recurring congestion, with informed and uninformed travelers, Poisson arrivals, randomized service times, and scenario sweeps by percent informed and capacity/service assumptions. It does not describe survey microdata or a person-level dataset to archive.

The package keeps the two paper-specific PATH-ATIS workbooks:

- `code/original/Qi2.xls`: incident/service-rate scenario workbook.
- `code/original/Qr2.xls`: recurrent/arrival-rate scenario workbook.

The original `.xls` filenames are retained because the embedded macros call workbook names such as `Qi2.xls!Macro1` and `Qr2.xls!Copier`. Modern `.xlsx` copies are provided only for easier inspection; the original `.xls` files remain the authoritative macro-bearing artifacts.

## Contents

- `paper/ATIS.pdf`: local reference copy used for audit validation. Review publisher rights before including this PDF in any public GitHub release.
- `code/original/`: original legacy Excel `.xls` workbook model files.
- `code/modernized/`: LibreOffice-converted `.xlsx` copies for inspection.
- `code/extracted_vba/`: extracted VBA source text from the original workbooks.
- `documentation/`: source review, release notes, and shared-source pointer.
- `metadata/`: source map, workbook sheet summary, and macro module summary.

## Shared Source Pointer

The overlapping `Qp2`, `Qpi2`, and `ServiceTime` workbooks are not duplicated here. They are staged once in:

`/Users/dlev2617/Documents/Code/Agents/github-packages/_shared_sources/probe-atis-spreadsheet-model`

That shared source is used by `paper-2002-01` and related traveler-information/probe model work. This package points to it rather than uploading duplicate copies.

## Release Notes

The staged workbook model appears to be author/project-created legacy code. The reviewed package contains no raw person-level records, no third-party source data, and no letters, drafts, presentations, or autonomous audit sidecars. Before public repository creation, add the final chosen license/provenance language for the author-created workbook code/model and keep the publisher PDF reference-only unless rights review clears it.

<!-- package-hardening-status:start -->
## Package Hardening Status

Generated: 2026-05-20 15:23:47 AEST

- Pipeline: `READY-TO-UPLOAD/PUBLIC`
- Sidecars added/updated: `PACKAGE_STATUS.md`, `PACKAGE_MANIFEST.csv`, `LICENSE_STATUS.md`.
- Paper reference copies are for local audit convenience and are not public-upload assets without rights review.
- Final GitHub upload should use the manifest include statuses and the license-status note.
<!-- package-hardening-status:end -->
