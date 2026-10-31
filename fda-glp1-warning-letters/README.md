# FDA Warning Letters Citing GLP-1 Drugs, 2024 to 2026

Every FDA warning letter posted on fda.gov, dated January 2024 or later, that cites a GLP-1 drug (semaglutide, tirzepatide, retatrutide or liraglutide, under any brand or code name) and went to a telehealth company, clinic, compounding pharmacy, outsourcing facility, online seller or drugmaker, with the letter date, the recipient, what FDA cited, the close-out status and a link to the letter.

- Publisher: Wellchosen Health, https://wellchosenhealth.com/
- Page: https://wellchosenhealth.com/glp-1/fda-warning-letters/
- File: `fda-glp1-warning-letters.csv` (153 rows, 8 columns; UTF-8, comma-separated, one header row)
- Download: https://wellchosenhealth.com/data/fda-glp1-warning-letters/fda-glp1-warning-letters.csv
- Rows checked: 2026-10-27
- Page last updated: 2026-10-27
- License: Creative Commons Attribution 4.0 International (CC BY 4.0), https://creativecommons.org/licenses/by/4.0/

## Columns

| Column | Type | Unit or format | Description |
| --- | --- | --- | --- |
| `letter_date` | date | YYYY-MM-DD | Date printed on the letter on fda.gov. |
| `company` | string |  | Recipient, as FDA names it. |
| `fda_cited` | string |  | What the letter cites: products, claims and the sections of the Food, Drug, and Cosmetic Act. |
| `status_note` | string |  | Recipient type, posting date where noted, and whether FDA has posted a close-out letter. |
| `provider_slug` | string |  | Wellchosen Health ID for the company, when we review it. Blank otherwise. |
| `review_url` | url | URL | Our review of the company, when one is published. |
| `source_url` | url | URL | The letter on fda.gov. |
| `checked_date` | date | YYYY-MM-DD | Date we opened the letter on fda.gov. |

Blank cells mean the value does not apply, was not published or was not found.

## Sources

- FDA warning letters on fda.gov, one letter per row (source_url). Every letter was opened on fda.gov on the checked date.

Every row carries its own source URL and checked date. The page lists every source in full.

## Checked dates

Rows were checked on 2026-10-27 (the `checked_date` column). Values can change after that date; treat each one as correct on its checked date.

## Update schedule

No fixed schedule: updated when we recheck a source or fix an error, as stated on the Wellchosen Health data page.

This file is rebuilt from the page's source data every time the site is built, so it always matches https://wellchosenhealth.com/glp-1/fda-warning-letters/.

## Notes

- Left out: letters to makers of bulk ingredients, letters about a drugmaker's safety reporting, close-out letters (the status_note column notes them), untitled letters and cease-and-desist letters.
- A warning letter is FDA's written position that a company broke federal drug law. It is not a court ruling.
- provider_slug and review_url are filled only for companies Wellchosen Health reviews.

## License

CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/). You may copy, share, chart and adapt the data, including commercially, with credit to Wellchosen Health and a link to https://wellchosenhealth.com/glp-1/fda-warning-letters/.

## How to cite

Wellchosen Health (2026). FDA Warning Letters Citing GLP-1 Drugs, 2024 to 2026 [Data set]. https://wellchosenhealth.com/glp-1/fda-warning-letters/

## Corrections

Spot an error or a change? Email contact@wellchosenhealth.com with the row and a source.
