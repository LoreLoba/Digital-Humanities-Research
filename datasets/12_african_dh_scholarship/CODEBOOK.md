# Digital humanities research from African institutions — codebook

**One row is** one publication with at least one African institutional affiliation.

Digital humanities publications indexed by OpenAlex with an African institutional affiliation. A dataset about the field the participants are joining — who publishes DH research on the continent, where, and how openly.

- **Rows:** 3,500
- **Columns:** 9
- **Source:** [OpenAlex API](https://openalex.org/)
- **Licence:** CC0 1.0 (OpenAlex)
- **Attribution:** OpenAlex (OurResearch). CC0 1.0.
- **Retrieved:** 2026-08-09

## Columns

| Column | Type | Description | % missing | Distinct | Example |
|---|---|---|---:|---:|---|
| `openalex_id` | text | OpenAlex work identifier | 0.0 | 3,500 | W2123428234 |
| `title` | text | Publication title | 0.0 | 3,382 | Archaeological Evidence for the Emergence of Language, Symbo |
| `year` | number | Year of publication | 0.1 | 74 | 2003.0 |
| `type` | text | Work type (article, book-chapter, …) | 0.0 | 19 | article |
| `venue` | text | Journal or publisher | 0.0 | 1,382 | Journal of World Prehistory |
| `first_african_institution` | text | First affiliation with a country code | 0.0 | 858 | Centre National de la Recherche Scientifique (FR) |
| `n_authors` | whole number | Number of listed authors | 0.0 | 21 | 12 |
| `cited_by` | whole number | Citation count according to OpenAlex | 0.0 | 110 | 509 |
| `is_open_access` | number | Whether OpenAlex records it as open access | 0.0 | 2 | False |

## What was done to the source data

- Harvested through the OpenAlex cursor API, filtered to the digital-humanities concept and African institutional affiliation.
- Authorship flattened to a count plus the first affiliation carrying a country.

## Known limits

- OpenAlex indexes journals unevenly by region and language.
- The 'digital humanities' concept is assigned algorithmically and is imperfect.
- Affiliation strings are inconsistent; the same university appears several ways.
