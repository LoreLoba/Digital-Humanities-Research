# Trans-Atlantic slave trade — voyages — codebook

**One row is** one recorded slaving voyage.

Voyages of the trans-Atlantic slave trade: the ship, where it sailed from, where people were purchased, where it arrived, the year, and how many people survived the crossing. It is the foundational dataset of African diaspora digital humanities, and the most demanding one in this pack to write about responsibly.

- **Rows:** 36,110
- **Columns:** 9
- **Source:** [SlaveVoyages, via the TidyTuesday mirror](https://www.slavevoyages.org/)
- **Licence:** SlaveVoyages data, redistributed via TidyTuesday for teaching
- **Attribution:** Trans-Atlantic Slave Trade Database (slavevoyages.org); mirror: TidyTuesday 2020-06-16.
- **Retrieved:** 2026-08-09

## Columns

| Column | Type | Description | % missing | Distinct | Example |
|---|---|---|---:|---:|---|
| `voyage_id` | whole number | Identifier for the voyage in the source database | 0.0 | 36,110 | 81711 |
| `ship_name` | text | Name of the ship | 4.5 | 9,447 | Hannah |
| `port_origin` | text | Port the voyage began from | 12.4 | 243 | Liverpool |
| `place_of_purchase` | text | Where on the African coast people were purchased | 4.7 | 181 | Calabar |
| `port_arrival` | text | Port of disembarkation in the Americas | 11.8 | 273 | St. Vincent, port unspecified |
| `year_arrival` | whole number | Year the voyage arrived | 0.0 | 335 | 1787 |
| `n_slaves_arrived` | number | Number of enslaved people recorded as arriving alive | 49.1 | 817 | 390.0 |
| `captains_name` | text | Captain, where recorded | 11.2 | 18,895 | Smith, Bryan |
| `century` | whole number | Century of arrival, derived from year_arrival | 0.0 | 4 | 18 |

## What was done to the source data

- Year and count columns coerced to numbers.
- Added `century`, derived from `year_arrival`, as a grouping variable.
- No rows removed.

## Known limits

- Records survive unevenly: absence of voyages is not absence of trading.
- `n_slaves_arrived` counts survivors of the crossing, so it under-records how many people were embarked.
- Ports and places are as written in the sources, with inconsistent spellings.

## Handling note

Every row of this dataset is a voyage that carried enslaved people, and `n_slaves_arrived` is a count of human beings who survived a forced crossing. Work with it as historical evidence of a crime against people, not as a neutral counting exercise. Begin with the absence audit, not with the statistics.
