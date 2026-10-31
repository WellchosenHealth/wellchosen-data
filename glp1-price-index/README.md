# GLP-1 Price Index: US Cash Prices for Online Programs and Maker Channels

All-in monthly cash prices for compounded and FDA-approved brand GLP-1 drugs (semaglutide, tirzepatide, Wegovy, Ozempic, Zepbound, Mounjaro, Foundayo) at US online programs and at maker, retail pharmacy, government, discount card, Medicare and copay card channels. Each price was read on the seller's own site and carries its source URL and checked date. Program rows add the Wellchosen Health verdict, the date and URL of the program's latest FDA warning letter, and its BBB grade.

- Publisher: Wellchosen Health, https://wellchosenhealth.com/
- Page: https://wellchosenhealth.com/glp-1/price-report/
- File: `glp1-price-index.csv` (57 rows, 14 columns; UTF-8, comma-separated, one header row)
- Download: https://wellchosenhealth.com/data/glp1-price-index/glp1-price-index.csv
- Rows checked: 2026-10-27
- Page last updated: 2026-10-27
- License: Creative Commons Attribution 4.0 International (CC BY 4.0), https://creativecommons.org/licenses/by/4.0/

## Columns

| Column | Type | Unit or format | Description |
| --- | --- | --- | --- |
| `program` | string |  | Program or channel name. Channel rows read "Channel: drug". |
| `slug` | string |  | Wellchosen Health ID for the program, matching its review at https://wellchosenhealth.com/reviews/ followed by the slug. Blank for channels. |
| `channel_type` | category |  | online_program, maker, retail_pharmacy, discount_card, government_portal, medicare or copay_card. |
| `verdict` | category |  | Wellchosen Health rating: Clean, Use caution, Avoid or Not yet rated. Blank for channels. |
| `fda_letter_date` | date | YYYY-MM-DD | Date of the most recent FDA warning letter to the company. Blank if none found. |
| `fda_letter_url` | url | URL | That letter on fda.gov. |
| `bbb_grade` | string |  | BBB letter grade, Not rated (NR), or Not checked. |
| `cheapest_compounded_all_in_usd` | number | US dollars per month | Lowest ongoing monthly price for a compounded GLP-1, including any required membership. Blank when not published, not sold or not readable. |
| `cheapest_brand_all_in_usd` | number | US dollars per month | Lowest ongoing monthly price for an FDA-approved brand GLP-1, including any required membership. For channel rows, the lowest price for the drug named. |
| `includes` | string |  | What the price covers, as the seller states it. For channel rows, the price as shown. |
| `commitment` | string |  | Plan length or prepayment the price needs. For channel rows, the conditions. |
| `checked_date` | date | YYYY-MM-DD | Date we read the price on the seller's own site. |
| `source_url` | url | URL | The page the price came from. |
| `notes` | string |  | Conflicts on the page, promotions we left out, and why a price is blank. |

Blank cells mean the value does not apply, was not published or was not found.

## Sources

- Each program's own pricing and product pages, read on the checked date (source_url).
- Maker and channel pages: LillyDirect, NovoCare Pharmacy, TrumpRx.gov and each retailer's own pages (source_url).
- FDA warning letters on fda.gov, matched from the Wellchosen Health FDA GLP-1 warning letter tracker (fda_letter_url).
- Better Business Bureau profiles on bbb.org (bbb_grade).

Every row carries its own source URL and checked date. The page lists every source in full.

## Checked dates

Rows were checked on 2026-10-27 (the `checked_date` column). Values can change after that date; treat each one as correct on its checked date.

## Update schedule

Monthly, as a dated edition of the GLP-1 Price and Safety Report (the Wellchosen Health data page lists this dataset as monthly). Each edition replaces this file, and rows also change between editions when we fix an error.

This file is rebuilt from the page's source data every time the site is built, so it always matches https://wellchosenhealth.com/glp-1/price-report/.

## Notes

- All-in means the monthly price of the medicine plus any membership, program or visit fee the seller requires, at the plan length in the commitment column. For online programs, first-month promotions, starter prices and promo codes are left out. Channel rows show each channel's lowest posted price, including starter prices.
- Compounded semaglutide and tirzepatide are not FDA-approved, and FDA does not review them for safety, effectiveness or quality.
- Verdicts (Clean, Use caution, Avoid, Not yet rated) follow the fixed rule on https://wellchosenhealth.com/editorial-standards/ and match each program's review.
- A blank price means the program did not publish one, does not sell that type, or the price could not be read; the notes column says which.
- No company paid for a place in this dataset, saw it before publication, or can change its row.

## License

CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/). You may copy, share, chart and adapt the data, including commercially, with credit to Wellchosen Health and a link to https://wellchosenhealth.com/glp-1/price-report/.

## How to cite

Wellchosen Health (2026). GLP-1 Price Index: US Cash Prices for Online Programs and Maker Channels [Data set]. https://wellchosenhealth.com/glp-1/price-report/

## Corrections

Spot an error or a change? Email contact@wellchosenhealth.com with the row and a source.
