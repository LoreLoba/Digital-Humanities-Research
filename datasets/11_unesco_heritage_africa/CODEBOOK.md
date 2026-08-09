# UNESCO World Heritage sites in Africa — codebook

**One row is** one inscribed World Heritage site.

World Heritage sites in the UNESCO Africa region, with the year they were inscribed, coordinates, category and whether they are listed as in danger. Small enough to read end to end, which makes it good for careful work.

- **Rows:** 115
- **Columns:** 12 (12 of 20 source columns)
- **Source:** [UNESCO World Heritage Centre — XML list](https://whc.unesco.org/en/list/)
- **Licence:** © UNESCO World Heritage Centre — used for teaching with attribution
- **Attribution:** UNESCO World Heritage Centre, World Heritage List.
- **Retrieved:** 2026-08-09

## Columns

| Column | Type | Description | % missing | Distinct | Example |
|---|---|---|---:|---:|---|
| `site_name` | text | Name of the site | 0.0 | 115 | W-Arly-Pendjari Complex |
| `country` | text | State Party or Parties the site is in | 0.0 | 45 | Benin,Burkina Faso,Niger |
| `category` | text | Cultural, Natural, or Mixed | 0.0 | 3 | Natural |
| `year_inscribed` | whole number | Year the site joined the World Heritage List | 0.0 | 40 | 1996 |
| `in_danger` | whole number | 1 if on the List of World Heritage in Danger, else 0 | 0.0 | 1 | 0 |
| `iso_code` | text | ISO country code(s), comma-separated | 0.0 | 45 | bf,bj,ne |
| `unesco_region` | text | UNESCO administrative region | 0.0 | 1 | Africa |
| `transnational` | whole number | 1 if the site spans more than one country | 0.0 | 2 | 1 |
| `criteria` | text | The World Heritage criteria it was inscribed under | 0.0 | 41 | (ix)(x) |
| `url` | text | Link to the site's UNESCO page | 0.0 | 115 | https://whc.unesco.org/en/list/749 |
| `description` | text | Short official description, HTML stripped | 0.0 | 115 | This transnational extension (Benin, Burkina Faso) to the W  |
| `n_states` | whole number | How many states the site spans — derived from `country` | 0.0 | 3 | 3 |

## What was done to the source data

- Parsed from the official XML list; filtered to the UNESCO Africa region.
- Numeric columns coerced; HTML stripped and whitespace collapsed in descriptions.
- Added `n_states`, derived from the comma-separated states list.

## Known limits

- UNESCO's 'Africa' region excludes North African states, which sit in the Arab States region — so this is not every site on the continent.
- Inscription reflects nomination effort and state capacity, not heritage value.
- The XML carries no coordinates or area, so mapping needs an external join.
