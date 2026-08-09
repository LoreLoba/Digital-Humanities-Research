# Knoedler stock books — the New York art market — codebook

**One row is** one transaction recorded in the Knoedler gallery stock books.

M. Knoedler & Co. was one of the most important art dealers in New York from the 1870s to 1970. Their stock books record what they bought, from whom, for how much, and who bought it. This is provenance research as a spreadsheet.

- **Rows:** 40,253
- **Columns:** 14 (14 of 117 source columns)
- **Source:** [Getty Provenance Index — Knoedler stock books](https://github.com/thegetty/provenance-index-csv)
- **Licence:** CC0 1.0 Universal (public domain dedication)
- **Attribution:** Getty Research Institute, Getty Provenance Index®. CC0 1.0.
- **Retrieved:** 2026-08-09

## Columns

| Column | Type | Description | % missing | Distinct | Example |
|---|---|---|---:|---:|---|
| `pi_record_no` | text | Getty's record identifier for this transaction | 0.0 | 40,250 | K-40452 |
| `stock_book_no` | whole number | Which stock book the entry appears in | 0.0 | 11 | 4 |
| `page_number` | whole number | Page in the stock book | 0.0 | 278 | 29 |
| `entry_date_year` | number | Year Knoedler entered the work in the stock book | 4.9 | 100 | 1884.0 |
| `artist_name_1` | text | Artist, as recorded by Knoedler | 0.3 | 8,174 | Tamburini |
| `nationality_1` | text | Artist nationality, as recorded | 0.3 | 53 | Italian |
| `title` | text | Title of the work | 0.0 | 26,169 | Never too late to mend |
| `object_type` | text | Kind of object (painting, drawing, sculpture…) | 0.0 | 22 | Painting |
| `consign_name` | text | Who consigned the work to Knoedler | 95.7 | 80 | Goupil & Co. |
| `seller_name_1` | text | Seller | 22.6 | 5,256 | Arthur Tooth & Sons London |
| `price_amount` | number | What the work sold for | 36.2 | 2,451 | 237.5 |
| `price_currency` | text | Currency of the sale | 36.1 | 7 | dollars |
| `buyer_name_1` | text | Buyer | 31.9 | 8,087 | L.M. Palmer |
| `sale_date_year` | number | Year of sale | 31.6 | 100 | 1885.0 |

## What was done to the source data

- Kept 14 of 117 columns — the source records many authority-control and cross-reference fields that are not useful without the wider Getty vocabularies.
- Money and year columns coerced to numbers.
- No rows removed.

## Known limits

- One gallery's records — not the art market as a whole.
- Prices are nominal, in mixed currencies, and not inflation-adjusted.
- Names are as Knoedler wrote them; the same person may appear several ways.
