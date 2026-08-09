# Bechdel test results for 1,794 films — codebook

**One row is** one film.

Whether each film passes the Bechdel test — two named women who talk to each other about something other than a man — alongside budget and box office, inflation-adjusted to 2013 dollars. A compact dataset where the interesting question is what the measure does and does not capture.

- **Rows:** 1,794
- **Columns:** 11 (11 of 15 source columns)
- **Source:** [FiveThirtyEight — bechdel/movies.csv](https://github.com/fivethirtyeight/data/tree/master/bechdel)
- **Licence:** CC BY 4.0
- **Attribution:** FiveThirtyEight, 'The Dollar-And-Cents Case Against Hollywood's Exclusion of Women' (2014). CC BY 4.0.
- **Retrieved:** 2026-08-09

## Columns

| Column | Type | Description | % missing | Distinct | Example |
|---|---|---|---:|---:|---|
| `year` | whole number | Release year | 0.0 | 44 | 2013 |
| `title` | text | Film title | 0.0 | 1,768 | 21 &amp; Over |
| `clean_test` | text | Bechdel result in detail: ok, dubious, men (only men talk), notalk (women do not talk to each other), nowomen | 0.0 | 5 | notalk |
| `binary` | text | PASS or FAIL — clean_test collapsed to two values | 0.0 | 2 | FAIL |
| `budget` | whole number | Production budget in dollars of the release year | 0.0 | 272 | 13000000 |
| `domgross` | number | Domestic (US) gross, dollars of the release year | 0.9 | 1,750 | 25682380.0 |
| `intgross` | number | International gross, dollars of the release year | 0.6 | 1,756 | 42195766.0 |
| `budget_2013` | whole number | Budget adjusted to 2013 dollars — use this to compare across years | 0.0 | 1,188 | 13000000 |
| `domgross_2013` | number | Domestic gross in 2013 dollars | 1.0 | 1,775 | 25682380.0 |
| `intgross_2013` | number | International gross in 2013 dollars | 0.6 | 1,782 | 42195766.0 |
| `imdb` | text | IMDb identifier | 0.0 | 1,794 | tt1711425 |

## What was done to the source data

- Column names normalised; the `_2013$` columns renamed to `_2013`.
- Money columns coerced to numbers; unparseable values became missing.

## Known limits

- 1970-2013 only, and heavily weighted to US releases.
- Pass/fail is judged by volunteer contributors, not by a fixed procedure.
- No genre, director or cast columns — those must come from elsewhere.
