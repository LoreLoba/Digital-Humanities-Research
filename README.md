# DH Group Assignment Data Pack

Thirteen curated datasets for group work in digital humanities, each with a codebook, a group brief and a starter notebook.

Every dataset is a real published source, fetched and prepared rather than invented. Each has been cut down to a **teaching subset**: a width a group can hold in their head, with every column documented. The codebook always says how many of the source columns were kept.

## How to use it

1. Each group takes one dataset folder.
2. Read `CODEBOOK.md` first — what each column means and how much is missing.
3. Read `BRIEF.md` — the seven steps, and the trap specific to that dataset.
4. Work in Excel (`data.xlsx`, which has Data / Codebook / Source sheets) or in Python (`starter.ipynb`, which loads the data and stubs the steps).

See [ASSIGNMENT.md](ASSIGNMENT.md) for the shared task and the marking guide.

## The datasets

| # | Dataset | One row is | Rows | Cols | Licence |
|---|---|---|---:|---:|---|
| 01 | [Humanities researchers on research data management](datasets/01_humanities_rdm_survey/) | one survey response from a humanities researcher | 372 | 22 | CC BY 4.0 |
| 02 | [Bechdel test results for 1,794 films](datasets/02_bechdel_films/) | one film | 1,794 | 11 | CC BY 4.0 |
| 03 | [Knoedler stock books — the New York art market](datasets/03_getty_knoedler/) | one transaction recorded in the Knoedler gallery stock books | 40,253 | 14 | CC0 1.0 Universal (public domain dedication) |
| 04 | [US public libraries — staffing, funding and use](datasets/04_imls_public_libraries/) | one public library system in the 2020 financial year | 9,245 | 20 | US Government public domain |
| 05 | [Journal of Open Humanities Data — every paper](datasets/05_johd_dataset_papers/) | one data paper published in JOHD | 365 | 9 | Crossref metadata — CC0 |
| 07 | [Trans-Atlantic slave trade — voyages](datasets/07_slave_voyages/) | one recorded slaving voyage | 36,110 | 9 | SlaveVoyages data, redistributed via TidyTuesday for teaching |
| 08 | [African languages — Glottolog](datasets/08_african_languages/) | one language or dialect spoken in Africa | 8,037 | 10 | CC BY 4.0 |
| 09 | [African films on Wikidata](datasets/09_african_films/) | one film with an African country of origin | 5,582 | 6 | CC0 1.0 (Wikidata) |
| 10 | [African-origin objects in museum collections](datasets/10_african_artworks_in_museums/) | one object, in one museum collection | 1,928 | 5 | CC0 1.0 (Wikidata) |
| 11 | [UNESCO World Heritage sites in Africa](datasets/11_unesco_heritage_africa/) | one inscribed World Heritage site | 115 | 12 | © UNESCO World Heritage Centre — used for teaching with attribution |
| 12 | [Digital humanities research from African institutions](datasets/12_african_dh_scholarship/) | one publication with at least one African institutional affiliation | 3,500 | 9 | CC0 1.0 (OpenAlex) |
| 13 | [Wikipedia attention to African writers](datasets/13_wikipedia_reception_african_writers/) | one writer in one month | 750 | 5 | CC0 1.0 (Wikimedia analytics) |
| 06 | [Geographic Locations in English-Language Literature, 1701-2011](https://wiki.htrc.illinois.edu/display/COM/Geographic+Locations+in+English-Language+Literature%2C+1701-2011) — *link only* | a place mentioned in a literary volume | — | — | not redistributed |

## Provenance and licensing

Every dataset here is redistributed under a licence that permits it — CC0, CC BY 4.0, or public domain — except where noted. Attribution for each is in its codebook and on the `Source` sheet of its workbook. One source (#06) is documented and linked but **not** redistributed, because its terms could not be confirmed.

Built 2026-08-09 by `dh_data_pack/build_dh_pack.py`. Re-running it refetches everything from source.

Note that #13 queries a live API, so its numbers move between builds; the other twelve are stable snapshots.
