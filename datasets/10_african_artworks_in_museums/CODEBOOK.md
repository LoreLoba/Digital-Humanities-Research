# African-origin objects in museum collections — codebook

**One row is** one object, in one museum collection.

Objects Wikidata records as originating in an African country and held in a named museum collection. The restitution question as a spreadsheet: what is held, by whom, and from where.

- **Rows:** 1,928
- **Columns:** 5
- **Source:** [Wikidata, queried via QLever](https://query.wikidata.org/)
- **Licence:** CC0 1.0 (Wikidata)
- **Attribution:** Wikidata contributors. CC0 1.0. Retrieved via the QLever mirror.
- **Retrieved:** 2026-08-09

## Columns

| Column | Type | Description | % missing | Distinct | Example |
|---|---|---|---:|---:|---|
| `wikidata_id` | text | Wikidata item identifier (Q-number) | 0.0 | 1,627 | Q100891538 |
| `object` | text | Object name or title, English label | 0.0 | 1,570 | Head Ornament |
| `country_of_origin` | text | Country the object is recorded as originating in | 0.0 | 57 | Ottoman Empire |
| `held_by` | text | Museum or collection currently holding it | 0.0 | 188 | Khalili Collection: Enamels of the World |
| `inception_year` | whole number | Year the object was made, where recorded | 15.0 | 373 | 1900 |

## What was done to the source data

- SPARQL query for items with both a collection (P195) and an African country of origin (P495).
- Inception dates reduced to a year.
- One row per object-collection pair.

## Known limits

- Only objects somebody has catalogued on Wikidata — a small fraction of holdings.
- `country_of_origin` includes historical polities, not just modern states: the query selects anything Wikidata places on the African continent, so entities such as the Ottoman Empire appear alongside present-day countries. Check the distinct values before grouping by them.
- `held_by` mixes national museums with private collections.
- Nothing here records how an object was acquired.
