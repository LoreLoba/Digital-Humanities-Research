# Group brief — US public libraries — staffing, funding and use

**Your dataset:** `data.csv` / `data.xlsx` — 9,245 rows, 20 columns.
**One row is** one public library system in the 2020 financial year.

The annual census of US public library systems: what they hold, who works there, what they spend, and how much the public uses them. A clean panel for asking how library provision varies with the population it serves.

Read `CODEBOOK.md` before you touch the data. It tells you what every column means, how much of it is missing, and what was already done to it.

## The trap in this dataset

A row is a library *system*, not a library. One row may be a single rural branch and the next may be a city system with sixty buildings. Any per-row average mixes the two. Normalise by `population_served` or by building count before comparing.

Your write-up should show you noticed it.

## Suggested starting questions

- **Descriptive:** How many visits per person served does a typical system record?
- **Analytical:** Does spending per person predict visits per person?
- **Compare:** Compare urban and rural systems on staffing per 1,000 people served.

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

- **Source:** [IMLS Public Libraries Survey FY2020](https://www.imls.gov/research-evaluation/surveys/public-libraries-survey-pls)
- **Licence:** US Government public domain
- **Cite as:** Institute of Museum and Library Services, Public Libraries Survey FY2020.
