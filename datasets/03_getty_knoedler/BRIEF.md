# Group brief — Knoedler stock books — the New York art market

**Your dataset:** `data.csv` / `data.xlsx` — 40,253 rows, 14 columns.
**One row is** one transaction recorded in the Knoedler gallery stock books.

M. Knoedler & Co. was one of the most important art dealers in New York from the 1870s to 1970. Their stock books record what they bought, from whom, for how much, and who bought it. This is provenance research as a spreadsheet.

Read `CODEBOOK.md` before you touch the data. It tells you what every column means, how much of it is missing, and what was already done to it.

## The trap in this dataset

Prices sit in several currencies across a century, so summing or averaging the raw `price_amount` column is meaningless. Either restrict to one currency and one period, or say clearly that you are counting transactions rather than value.

Your write-up should show you noticed it.

## Suggested starting questions

- **Descriptive:** Which artists appear most often, and in which decades?
- **Analytical:** Did the gallery's purchase-to-sale margin differ by object type?
- **Compare:** Compare two decades on the mix of nationalities traded.

## The seven steps

Every group does these, on their own dataset, so the presentations compare.

### 1. Frame

Write one **descriptive** question and one **analytical** question this dataset can actually answer. Say which method each needs.

### 2. Absence audit

What did this dataset never record? Name a missing variable, a missing population, and a level of detail that is too coarse. Which absence most limits your questions?

### 3. Describe

Summarise the variable at the centre of your question. Choose between mean and median deliberately and justify it — for skewed data one of them describes nothing real.

### 4. Compare

Split the data into two groups that matter and compare them. State the size of the difference in the units a reader thinks in.

### 5. Test

Could that difference be chance? Run an appropriate test **and** report an effect size. If you test more than one thing, correct for it.

### 6. Show

One chart. Sorted deliberately, with a reference line if there is a meaningful threshold, and a caption saying what you filtered.

### 7. Limits

One page: your finding, the method, the uncertainty, and an explicit list of sentences this data does **not** support.

## What to hand in

- **A one-page brief** — finding, method, uncertainty, limits.
- **One chart**, captioned.
- **Your workbook or notebook**, so the steps can be checked.

## Source and licence

- **Source:** [Getty Provenance Index — Knoedler stock books](https://github.com/thegetty/provenance-index-csv)
- **Licence:** CC0 1.0 Universal (public domain dedication)
- **Cite as:** Getty Research Institute, Getty Provenance Index®. CC0 1.0.
