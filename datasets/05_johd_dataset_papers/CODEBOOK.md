# Journal of Open Humanities Data — every paper — codebook

**One row is** one data paper published in JOHD.

JOHD publishes short papers describing reusable humanities datasets. This is the journal's whole output as metadata: who publishes data papers, on what, from where, and what gets cited. A dataset about datasets.

- **Rows:** 365
- **Columns:** 9
- **Source:** [Crossref — Journal of Open Humanities Data (ISSN 2059-481X)](https://openhumanitiesdata.metajnl.com/)
- **Licence:** Crossref metadata — CC0
- **Attribution:** Crossref REST API, Journal of Open Humanities Data metadata. CC0.
- **Retrieved:** 2026-08-09

## Columns

| Column | Type | Description | % missing | Distinct | Example |
|---|---|---|---:|---:|---|
| `doi` | text | Digital Object Identifier | 0.0 | 365 | 10.5334/johd.1 |
| `title` | text | Paper title — usually names the dataset it describes | 0.0 | 365 | Vagrant Lives: 14,789 Vagrants Processed by the County of Mi |
| `year` | whole number | Year of publication | 0.0 | 12 | 2015 |
| `type` | text | Crossref record type (journal-article and similar) | 0.0 | 1 | journal-article |
| `n_authors` | whole number | Number of listed authors | 0.0 | 18 | 3 |
| `first_author_affiliation` | text | Affiliation of the first author, where recorded | 0.0 | 1 |  |
| `subjects` | text | Crossref subject terms, semicolon-separated | 0.0 | 1 |  |
| `cited_by` | whole number | Times cited according to Crossref | 0.0 | 15 | 3 |
| `url` | text | Link to the paper | 0.0 | 365 | https://doi.org/10.5334/johd.1 |

## What was done to the source data

- Harvested through the Crossref cursor API and flattened to one row per paper.
- Title truncated to 300 characters; authors reduced to a count plus the first author's affiliation.

## Known limits

- Crossref affiliation data is patchy — many records have none.
- Citation counts are Crossref's, and undercount compared with other indexes.
- One journal, so nothing here generalises to data publishing as a whole.
