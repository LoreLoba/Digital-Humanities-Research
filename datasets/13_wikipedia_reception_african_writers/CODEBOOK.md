# Wikipedia attention to African writers — codebook

**One row is** one writer in one month.

Monthly English Wikipedia pageviews for thirty African writers over two years. A reception dataset: not what was written, but what people looked up, and when. Prizes, deaths and adaptations show up as spikes.

- **Rows:** 750
- **Columns:** 5
- **Source:** [Wikimedia Pageviews API](https://wikimedia.org/api/rest_v1/)
- **Licence:** CC0 1.0 (Wikimedia analytics)
- **Attribution:** Wikimedia Foundation, Pageviews API. CC0 1.0.
- **Retrieved:** 2026-08-09

## Columns

| Column | Type | Description | % missing | Distinct | Example |
|---|---|---|---:|---:|---|
| `writer` | text | Writer, as titled on English Wikipedia | 0.0 | 30 | Chinua Achebe |
| `year` | whole number | Year | 0.0 | 3 | 2023 |
| `month` | whole number | Month number | 0.0 | 12 | 1 |
| `year_month` | text | Year and month as YYYY-MM, for sorting and charting | 0.0 | 25 | 2023-01 |
| `views` | whole number | Pageviews from human users that month (automated traffic excluded) | 0.0 | 709 | 32512 |

## What was done to the source data

- Queried the monthly pageviews endpoint for 30 writers, Jan 2023 – Dec 2024.
- Restricted to `user` traffic, which excludes known bots and spiders.
- Flattened to one row per writer-month.

## Known limits

- English Wikipedia only — this measures anglophone attention specifically.
- The list of 30 writers is a curated selection, not a sample of African literature.
- Two years only; no long-run trend is available.
