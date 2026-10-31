# Medicaid GLP-1 Coverage by State

Whether each of the 51 US Medicaid programs (the 50 states and the District of Columbia) covers GLP-1 drugs such as Wegovy, Zepbound and Foundayo for weight loss, with the drugs and prior authorization rules, coverage of Wegovy for heart risk and Zepbound for obstructive sleep apnea, the latest 2025 or 2026 policy change and its date, and the primary documents behind each row.

- Publisher: Wellchosen Health, https://wellchosenhealth.com/
- Page: https://wellchosenhealth.com/glp-1/medicaid-coverage-by-state/
- File: `medicaid-glp1-coverage-by-state.csv` (51 rows, 11 columns; UTF-8, comma-separated, one header row)
- Download: https://wellchosenhealth.com/data/medicaid-glp1-coverage-by-state/medicaid-glp1-coverage-by-state.csv
- Rows checked: 2026-10-18
- Page last updated: 2026-10-28
- License: Creative Commons Attribution 4.0 International (CC BY 4.0), https://creativecommons.org/licenses/by/4.0/

## Columns

| Column | Type | Unit or format | Description |
| --- | --- | --- | --- |
| `state` | string |  | State name, or District of Columbia. |
| `state_code` | string |  | Two-letter USPS code. |
| `weight_loss_coverage` | category |  | Covered, Covered with limits, Ended in 2026, Not covered or Not confirmed. See notes. |
| `drugs_and_rules` | string |  | Which drugs are covered or excluded and the prior authorization rules, as the program's documents state them. |
| `wegovy_heart_risk` | string |  | Coverage of Wegovy to lower cardiovascular risk, with any criteria noted. |
| `zepbound_sleep_apnea` | string |  | Coverage of Zepbound for obstructive sleep apnea, with any criteria noted. |
| `latest_change_date` | date | YYYY-MM-DD, YYYY-MM or YYYY | Date the latest 2025 or 2026 change took effect, or was announced or scheduled where latest_change says so. |
| `latest_change` | string |  | What changed, or "No 2025 or 2026 change found". |
| `source_url` | url | URL | First document cited for the row. |
| `all_source_urls` | string |  | Every document cited for the row, in citation order, separated by a single space. |
| `checked_date` | date | YYYY-MM-DD | Date we checked the row's documents. |

Blank cells mean the value does not apply, was not published or was not found.

## Sources

- Each Medicaid program's preferred drug list, prior authorization criteria and forms, provider bulletins and state rules (source_url and all_source_urls per row).
- State legislation and agency announcements where a row cites them.
- Secondary sources, such as KFF, only where a primary document could not be found; the drugs_and_rules text says so.

Every row carries its own source URL and checked date. The page lists every source in full.

## Checked dates

Rows were checked on 2026-10-18 (the `checked_date` column). Values can change after that date; treat each one as correct on its checked date.

## Update schedule

No fixed schedule: updated when we recheck a source or fix an error, as stated on the Wellchosen Health data page. When a reader sends a change or a document we missed, we update the row and its date.

This file is rebuilt from the page's source data every time the site is built, so it always matches https://wellchosenhealth.com/glp-1/medicaid-coverage-by-state/.

## Notes

- weight_loss_coverage is about obesity treatment only. Covered: at least one GLP-1 is covered for weight loss with prior authorization under rules close to the FDA label. Covered with limits: covered under tighter rules than the label. Ended in 2026: coverage ended during 2026. Not covered: the program excludes weight-loss drugs. Not confirmed: we could not confirm the policy from published documents. Full definitions are under How we check on the page.
- Status reflects each program's published policy for adults. Members under 21 can get a separate medical-necessity review under the federal EPSDT benefit in several states, as the rows note.
- Not confirmed in the heart risk or sleep apnea column means we could not find or read the criteria, not that the state refuses.
- latest_change_date is a full date (YYYY-MM-DD) where the source gives one, YYYY-MM where it gives only a month, and YYYY where it gives only a year. It is blank when we found no 2025 or 2026 change.

## License

CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/). You may copy, share, chart and adapt the data, including commercially, with credit to Wellchosen Health and a link to https://wellchosenhealth.com/glp-1/medicaid-coverage-by-state/.

## How to cite

Wellchosen Health (2026). Medicaid GLP-1 Coverage by State [Data set]. https://wellchosenhealth.com/glp-1/medicaid-coverage-by-state/

## Corrections

Spot an error or a change? Email contact@wellchosenhealth.com with the row and a source.
