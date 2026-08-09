# Group brief — African languages — Glottolog

**Your dataset:** `data.csv` / `data.xlsx` — 8,037 rows, 10 columns.
**One row is** one language or dialect spoken in Africa.

Every language Glottolog records for Africa, with coordinates, family, and the countries it is spoken in. Coordinates mean a group can make a real map without needing shapefiles, and the family column supports questions about linguistic diversity.

Read `CODEBOOK.md` before you touch the data. It tells you what every column means, how much of it is missing, and what was already done to it.

## The trap in this dataset

The rows are not all the same kind of thing: `level` distinguishes languages from dialects and families. Counting all rows and calling the answer 'languages in Africa' inflates it substantially. Filter on `level` first and say which you counted.

Your write-up should show you noticed it.

## Suggested starting questions

- **Descriptive:** How many languages does each country have, and which has most?
- **Analytical:** Are cross-border languages (n_countries > 1) concentrated anywhere?
- **Compare:** Compare two language families on their geographic spread.

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

- **Source:** [Glottolog CLDF — languages.csv](https://glottolog.org/)
- **Licence:** CC BY 4.0
- **Cite as:** Hammarström, Forkel, Haspelmath & Bank, Glottolog. CC BY 4.0.
