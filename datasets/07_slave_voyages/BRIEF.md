# Group brief — Trans-Atlantic slave trade — voyages

**Your dataset:** `data.csv` / `data.xlsx` — 36,110 rows, 9 columns.
**One row is** one recorded slaving voyage.

Voyages of the trans-Atlantic slave trade: the ship, where it sailed from, where people were purchased, where it arrived, the year, and how many people survived the crossing. It is the foundational dataset of African diaspora digital humanities, and the most demanding one in this pack to write about responsibly.

Read `CODEBOOK.md` before you touch the data. It tells you what every column means, how much of it is missing, and what was already done to it.

> **Handling note.** Every row of this dataset is a voyage that carried enslaved people, and `n_slaves_arrived` is a count of human beings who survived a forced crossing. Work with it as historical evidence of a crime against people, not as a neutral counting exercise. Begin with the absence audit, not with the statistics.

## The trap in this dataset

This dataset names ships and captains. It names not one enslaved person. Every statistic you compute is therefore built from records kept by the people running the trade, for their own purposes. Before reporting any number, state whose record-keeping produced it and who is absent from it — that is the finding, as much as anything you can calculate.

Your write-up should show you noticed it.

## Suggested starting questions

- **Descriptive:** How many recorded voyages arrive per century, and at which ports?
- **Analytical:** Does the recorded number arriving per voyage change over time?
- **Compare:** Compare two arrival regions on voyage counts — then ask whether you are comparing the trade or the survival of its paperwork.

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

- **Source:** [SlaveVoyages, via the TidyTuesday mirror](https://www.slavevoyages.org/)
- **Licence:** SlaveVoyages data, redistributed via TidyTuesday for teaching
- **Cite as:** Trans-Atlantic Slave Trade Database (slavevoyages.org); mirror: TidyTuesday 2020-06-16.
