# Source Review

The published paper describes an analytical and simulation treatment of advanced traveler information systems for route choice. The modeling section defines two parallel links, informed and uninformed drivers, Poisson vehicle arrivals, randomized service times, recurrent congestion scenarios, and incident/service-rate reductions. No survey microdata, person-level records, or third-party source data are described as paper inputs.

The local source folder `/Users/dlev2617/Documents/Data/~Nexus_Data/~PATH/PATH-ATIS` contains the relevant legacy Excel workbooks. The paper-specific files retained here are `Qi2.xls` and `Qr2.xls`. Both are Excel 97-2004 binary workbooks with embedded VBA project streams, so they are treated as spreadsheet-plus-macro model/code artifacts rather than passive data tables.

`Qi2.xls` contains sheets such as `ATI`, `ATU`, `ATO`, `T%I`, `T%U`, `SDI`, `SDU`, `Summary`, `Summary-Rec`, `RESULTS`, and `QUEUE`. These sheets include incident/service-rate and informed/uninformed travel-time and standard-deviation outputs.

`Qr2.xls` contains sheets such as `SummaryResults`, `AVGTI`, `AVGTU`, `AVGTO`, `STDI`, `STDU`, `DELTASTD`, `TSI`, `TSU`, `Summary`, `RESULTS`, and `QUEUE`. These sheets include recurrent/arrival-rate scenario outputs by percent informed.

The extracted VBA confirms workbook automation rather than a missing standalone script. `Macro1` repeatedly recalculates the workbook, `Copier` copies queue and result cells into the results sheet, and `Master*` procedures sweep scenario values for arrival/service assumptions and percent informed. The full extracted macro text is in `code/extracted_vba/`.

Modern `.xlsx` copies were created with LibreOffice for inspection. They should not be treated as complete macro-preserving replacements for the original `.xls` files.
