# Group brief — Journal of Open Humanities Data — every paper

**Your dataset:** `data.csv` / `data.xlsx` — 365 rows, 6 columns.
**One row is** one data paper published in JOHD.

JOHD publishes short papers describing reusable humanities datasets. This is the journal's whole output as metadata: who publishes data papers, on what, from where, and what gets cited. A dataset about datasets.

Read `CODEBOOK.md` before you touch the data. It tells you what every column means, how much of it is missing, and what was already done to it.

## The trap in this dataset

Citation counts are heavily confounded by age: a 2016 paper has had years to accumulate citations that a 2024 paper has not. Comparing raw `cited_by` across years measures how old a paper is. Compare within a year, or use citations per year since publication.

Your write-up should show you noticed it.

## Suggested starting questions

- **Descriptive:** How many data papers has JOHD published per year?
- **Analytical:** Has the typical number of authors changed over time?
- **Compare:** Compare citation counts for papers with and without a recorded affiliation — and ask what that comparison is really measuring.

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

- **Source:** [Crossref — Journal of Open Humanities Data (ISSN 2059-481X)](https://openhumanitiesdata.metajnl.com/)
- **Licence:** Crossref metadata — CC0
- **Cite as:** Crossref REST API, Journal of Open Humanities Data metadata. CC0.
