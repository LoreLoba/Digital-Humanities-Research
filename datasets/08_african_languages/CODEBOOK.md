# African languages — Glottolog — codebook

**One row is** one language or dialect spoken in Africa.

Every language Glottolog records for Africa, with coordinates, family, and the countries it is spoken in. Coordinates mean a group can make a real map without needing shapefiles, and the family column supports questions about linguistic diversity.

- **Rows:** 8,037
- **Columns:** 10 (10 of 15 source columns)
- **Source:** [Glottolog CLDF — languages.csv](https://glottolog.org/)
- **Licence:** CC BY 4.0
- **Attribution:** Hammarström, Forkel, Haspelmath & Bank, Glottolog. CC BY 4.0.
- **Retrieved:** 2026-08-09

## Columns

| Column | Type | Description | % missing | Distinct | Example |
|---|---|---|---:|---:|---|
| `glottocode` | text | Glottolog's stable identifier for the language | 0.0 | 8,037 | surm1244 |
| `language_name` | text | Language name | 0.0 | 8,037 | Surmic |
| `latitude` | number | Approximate centre of where the language is spoken | 0.7 | 3,800 | 6.881998770833333 |
| `longitude` | number | Approximate centre of where the language is spoken | 0.7 | 3,809 | 34.97338345833333 |
| `countries` | text | Countries it is spoken in, semicolon-separated | 69.3 | 250 | ER;ET;SD |
| `family_id` | text | Glottocode of the language family | 0.6 | 50 | surm1244 |
| `parent_language_id` | text | Glottocode of the parent language, for dialects | 47.7 | 1,005 | kuna1268 |
| `iso639_3` | text | ISO 639-3 code, where one exists | 71.5 | 2,288 | kun |
| `level` | text | language, dialect, or family | 0.0 | 3 | family |
| `n_countries` | whole number | How many countries it is spoken in — derived from `countries` | 0.0 | 9 | 0 |

## What was done to the source data

- Filtered to rows where Glottolog's Macroarea is Africa.
- Coordinates coerced to numbers; `n_countries` derived from the countries list.

## Known limits

- A single coordinate stands for a whole speech community, which may be vast.
- `level` mixes languages, dialects and families — filter before counting.
- Glottolog's boundaries between language and dialect are contested.
