# Peptide FDA and HHS Status Tracker

US legal status of peptides people search for, from BPC-157 to retatrutide: FDA approval, 503A compounding category, Pharmacy Compounding Advisory Committee votes, approved products, WADA status and next steps, with dates and source URLs. A flag and the named forms and routes mark the six peptides in the draft HHS 503A enforcement discretion policy filed Oct 28, 2026: BPC-157, TB-500, KPV, MOTS-c, Semax and Epitalon.

- Publisher: Wellchosen Health, https://wellchosenhealth.com/
- Page: https://wellchosenhealth.com/peptides/
- File: `peptide-fda-status.csv` (27 rows, 21 columns; UTF-8, comma-separated, one header row)
- Download: https://wellchosenhealth.com/data/peptide-fda-status/peptide-fda-status.csv
- Rows checked: 2026-10-19 to 2026-10-29
- Page last updated: 2026-10-29
- License: Creative Commons Attribution 4.0 International (CC BY 4.0), https://creativecommons.org/licenses/by/4.0/

## Columns

| Column | Type | Unit or format | Description |
| --- | --- | --- | --- |
| `peptide_id` | string |  | Wellchosen Health ID for the entry. |
| `peptide` | string |  | Name used on the site. |
| `also_called` | string |  | Other names and brands, separated by "; ". |
| `status_code` | category |  | approved, compoundable, cosmetic, discretion, pending, under_review, unapproved, not_allowed or unknown. |
| `status` | string |  | Plain-language label for status_code. |
| `status_group` | category |  | legal, pending, blocked or unknown. See notes. |
| `in_hhs_draft_policy_2026_10_28` | boolean | true or false | true if the peptide is named in the draft HHS 503A peptide policy filed Oct 28, 2026. |
| `hhs_draft_form` | string |  | Form of the bulk substance the draft names (for example acetate or free base). Blank if not in the draft. |
| `hhs_draft_routes` | string |  | Routes of administration the draft covers, separated by "; ". Blank if not in the draft. |
| `hhs_draft_source_url` | url | URL | Appendix B of the draft, which sets the forms and routes. Blank if not in the draft. |
| `status_summary` | string |  | One-paragraph summary of where the peptide stands. |
| `fda_status` | string |  | FDA approval and 503A category history in detail. |
| `advisory_committee` | string |  | Pharmacy Compounding Advisory Committee review and votes. |
| `fda_approved_products` | string |  | FDA-approved drugs that contain the peptide, if any. |
| `wada_status` | string |  | Status on the WADA Prohibited List. |
| `what_happens_next` | string |  | The next regulatory step we know of. |
| `last_status_change_date` | date | YYYY-MM-DD | Date of the last change in status. Blank when there is no dated change. |
| `page_url` | url | URL | The peptide's page on wellchosenhealth.com, when one exists. |
| `source_url` | url | URL | First source cited in status_summary. |
| `all_source_urls` | string |  | Every source for the entry, separated by a single space. |
| `checked_date` | date | YYYY-MM-DD | Date we last checked the entry. |

Blank cells mean the value does not apply, was not published or was not found.

## Sources

- FDA's 503A bulk drug substance categories document, FDA safety pages, Pharmacy Compounding Advisory Committee briefing documents, minutes and law firm reports of the votes, and FDA-approved drug labels (source_url and all_source_urls per row).
- The draft HHS Enforcement Discretion Policy Regarding 503A Compounding Using Certain Peptide Bulk Drug Substances, FR Doc. 2026-22192, Docket HHS-OASH-2026-0496, and its Appendix B (hhs_draft_source_url).
- WADA Prohibited List (wada_status).

Every row carries its own source URL and checked date. The page lists every source in full.

## Checked dates

Rows were checked on 2026-10-19 to 2026-10-29 (the `checked_date` column). Values can change after that date; treat each one as correct on its checked date.

## Update schedule

No fixed schedule: updated when we recheck a source or fix an error, as stated on the Wellchosen Health data page. The page says: when FDA acts, the row changes.

This file is rebuilt from the page's source data every time the site is built, so it always matches https://wellchosenhealth.com/peptides/.

## Notes

- status_group is legal (FDA-approved, compoundable with a prescription, or cosmetic only), pending (draft HHS policy, waiting on FDA, or under FDA review), blocked (not allowed in compounding, or trials only) or unknown.
- The draft HHS policy is enforcement discretion, not FDA approval. It is not final, covers only products with one listed peptide in the named form and route, and does not cover 503B outsourcing facilities. HHS says it may revisit the policy.
- Rows are entries, not molecules: GHK-Cu has separate injectable and topical rows because FDA treats them differently, and KLOW is a blend.
- This is general information, not legal or medical advice.

## License

CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/). You may copy, share, chart and adapt the data, including commercially, with credit to Wellchosen Health and a link to https://wellchosenhealth.com/peptides/.

## How to cite

Wellchosen Health (2026). Peptide FDA and HHS Status Tracker [Data set]. https://wellchosenhealth.com/peptides/

## Corrections

Spot an error or a change? Email contact@wellchosenhealth.com with the row and a source.
