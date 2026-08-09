# Group brief — African-origin objects in museum collections

**Your dataset:** `data.csv` / `data.xlsx` — 1,928 rows, 5 columns.
**One row is** one object, in one museum collection.

Objects Wikidata records as originating in an African country and held in a named museum collection. The restitution question as a spreadsheet: what is held, by whom, and from where.

Read `CODEBOOK.md` before you touch the data. It tells you what every column means, how much of it is missing, and what was already done to it.

## The trap in this dataset

Two traps, and the second is easy to miss. First, this table records where objects *are* and says nothing about how they got there — there is no acquisition column, so it cannot distinguish a purchase from a looted object. Second, `country_of_origin` is not a clean list of modern states: it contains historical polities because Wikidata assigns them a continent too. Run `value_counts()` on it before you group by it, or your 'countries' will include empires that no longer exist.

Your write-up should show you noticed it.

## Suggested starting questions

- **Descriptive:** Which institutions hold the most African-origin objects here?
- **Analytical:** Are objects from particular countries concentrated in particular collections?
- **Compare:** Compare two holding institutions on the range of origins represented.

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

- **Source:** [Wikidata, queried via QLever](https://query.wikidata.org/)
- **Licence:** CC0 1.0 (Wikidata)
- **Cite as:** Wikidata contributors. CC0 1.0. Retrieved via the QLever mirror.
