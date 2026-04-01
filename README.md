# Denmark Historical Statistics 1814-1980

## Overview

This repository contains digitized data from **"Dansk Økonomisk Statistik 1814-1980"** (Danish Historical Statistics 1814-1980), a comprehensive statistical compendium covering nearly two centuries of Danish economic and demographic data.

The original document was published as a single volume and has been scanned into 5 PDF files. The tabular data has been extracted and organized into a single Excel workbook for easy analysis.

## Files

| File | Description |
|------|-------------|
| `Denmark_Historical_Statistics_1814_1980.xlsx` | Excel workbook with all extracted statistical tables (55 sheets) |
| `CONTENTS.md` | Detailed table of contents describing each sheet in the Excel file |
| `DNK_Dansk 0konomisk statistik-1.pdf` | Source PDF Part 1 (50 pages) – Introduction & Tables 1.x |
| `DNK_Dansk 0konomisk statistik-2.pdf` | Source PDF Part 2 (50 pages) – Tables 1.5–4.7 |
| `DNK_Dansk 0konomisk statistik-3.pdf` | Source PDF Part 3 (50 pages) – Tables 4.7–9.1 |
| `DNK_Dansk 0konomisk statistik-4.pdf` | Source PDF Part 4 (50 pages) – Tables 9.1–10.4 |
| `DNK_Dansk 0konomisk statistik-5.pdf` | Source PDF Part 5 (17 pages) – Bibliography |

## Topics Covered

The dataset covers the following areas of Danish economic history:

1. **Population** – Demographics, age distribution, regional development, occupational distribution
2. **Agriculture** – Land use, livestock, crop output, production values, labour force
3. **Industry** – Manufacturing, industrial production indices, factory statistics
4. **Foreign Trade** – Imports, exports, geographic distribution, terms of trade, balance of payments
5. **Transport & Communication** – Transport services, communication infrastructure
6. **Banking & Finance** – National Bank, commercial banks, exchange rates, interest rates
7. **Labour Market** – Trade unions, work stoppages, unemployment
8. **Prices** – Consumer and wholesale price indices
9. **State Finances** – Government revenue, expenditure, public debt
10. **National Accounts** – GDP, consumption, investment in current and constant prices

## Excel File Structure

- **Contents** sheet – Table of contents with all tables listed
- **57 data table sheets** – One sheet per statistical table, with:
  - Table title and number
  - Column headers with English descriptions
  - Numerical data organized by year/period
- **Bibliography** sheet – Sources and references

## How the Data Was Extracted

The data was extracted programmatically from the 5 source PDFs using Python (`pdfplumber`) with:
- OCR text extraction from scanned pages
- Pattern matching for table numbers, column descriptions, and data rows
- English translations preserved from the original bilingual column headers

## Notes

- The original document is in Danish with English column descriptions in parentheses
- Some OCR artifacts may exist due to the age and quality of the scanned source material
- Years are presented as found in the original (calendar years or fiscal years like "1867/68")
- Monetary values are in the currency units of the respective periods (rigsdaler, kroner)