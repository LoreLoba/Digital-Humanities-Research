# African films on Wikidata — codebook

**One row is** one film with an African country of origin.

Every film Wikidata records as originating in an African country, with year, genre and director. The Bechdel dataset's African counterpart — and a good way to see what a crowd-built knowledge base does and does not cover.

- **Rows:** 5,582
- **Columns:** 6
- **Source:** [Wikidata, queried via QLever](https://query.wikidata.org/)
- **Licence:** CC0 1.0 (Wikidata)
- **Attribution:** Wikidata contributors. CC0 1.0. Retrieved via the QLever mirror.
- **Retrieved:** 2026-08-09

## Columns

| Column | Type | Description | % missing | Distinct | Example |
|---|---|---|---:|---:|---|
| `wikidata_id` | text | Wikidata item identifier (Q-number) | 0.0 | 5,582 | Q100105983 |
| `title` | text | Film title, English label | 0.0 | 5,519 | Dakara - The confession of a thug |
| `country` | text | Country of origin | 0.0 | 65 | Madagascar |
| `year` | whole number | Year of publication, where recorded | 11.0 | 108 | 2020 |
| `genre` | text | Genres, semicolon-separated | 0.0 | 409 | crime film; drama film; thriller film |
| `director` | text | Directors, semicolon-separated | 0.0 | 1,869 | Lemena Vintsy |

## What was done to the source data

- SPARQL query for films whose country of origin is in Africa.
- Multi-valued genre and director collapsed to one semicolon-separated row per film.
- Wikidata URIs reduced to bare Q-numbers.

## Known limits

- Wikidata coverage is uneven: better for countries with active editor communities.
- Missing year, genre or director means nobody has added it, not that it is unknown.
- English labels only, which biases which films appear at all.
