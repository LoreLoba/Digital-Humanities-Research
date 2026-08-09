# US public libraries — staffing, funding and use — codebook

**One row is** one public library system in the 2020 financial year.

The annual census of US public library systems: what they hold, who works there, what they spend, and how much the public uses them. A clean panel for asking how library provision varies with the population it serves.

- **Rows:** 9,245
- **Columns:** 20 (20 of 179 source columns)
- **Source:** [IMLS Public Libraries Survey FY2020](https://www.imls.gov/research-evaluation/surveys/public-libraries-survey-pls)
- **Licence:** US Government public domain
- **Attribution:** Institute of Museum and Library Services, Public Libraries Survey FY2020.
- **Retrieved:** 2026-08-09

## Columns

| Column | Type | Description | % missing | Distinct | Example |
|---|---|---|---:|---:|---|
| `library_system` | text | Name of the public library system | 0.0 | 8,460 | ANCHOR POINT PUBLIC LIBRARY |
| `state` | text | Two-letter US state code | 0.0 | 55 | AK |
| `county` | text | County | 0.0 | 1,659 | KENAI PENINSULA |
| `locale` | number | Urban / suburban / town / rural classification | 0.0 | 12 | 43.0 |
| `population_served` | number | Population of the legal service area | 0.6 | 7,600 | 2090.0 |
| `central_libraries` | number | Number of central library buildings | 0.2 | 2 | 1.0 |
| `branch_libraries` | number | Number of branch buildings | 0.2 | 46 | 0.0 |
| `total_staff_fte` | number | Total staff, full-time equivalent | 0.4 | 2,440 | 0.68 |
| `librarians_fte` | number | Librarians, full-time equivalent | 0.4 | 1,280 | 0.68 |
| `total_income` | number | Total operating income, US dollars | 0.4 | 9,130 | 57951.0 |
| `total_expenditure` | number | Total operating expenditure, US dollars | 0.4 | 8,527 | 4060.0 |
| `total_collection` | number | Total physical and electronic items held | 0.5 | 8,703 | 9150.0 |
| `ebooks` | number | Electronic books held | 0.4 | 4,267 | 0.0 |
| `visits` | number | Annual in-person visits | 0.5 | 7,959 | 4292.0 |
| `registered_borrowers` | number | Registered borrowers | 0.4 | 6,589 | 1854.0 |
| `total_circulation` | number | Annual items circulated | 0.5 | 8,642 | 7502.0 |
| `programmes` | number | Library programmes held in the year | 0.4 | 1,471 | 35.0 |
| `programme_attendance` | number | Total attendance at those programmes | 0.4 | 5,454 | 468.0 |
| `public_computers` | number | Internet computers available to the public | 0.3 | 358 | 5.0 |
| `computer_uses` | number | Annual uses of those computers | 0.5 | 5,590 | 1259.0 |

## What was done to the source data

- Kept 20 of 179 columns from the administrative-entity file.
- Renamed IMLS codes to readable names (e.g. POPU_LSA → population_served).
- IMLS negative sentinels for non-response converted to missing — they are codes, not counts, and averaging them would be badly wrong.

## Known limits

- One year only (FY2020), which was disrupted by COVID closures.
- A 'library system' can be one building or dozens — see the trap.
- US only.
