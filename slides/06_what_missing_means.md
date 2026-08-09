# What 'Missing' Means

*The most valuable thing you will bring to this data*

One of six short pre-workshop guides. No previous data or coding experience is assumed.

---

## Three kinds of missing

*SECTION 1*

- **Empty cells** — the value exists in the world but not in the file
- **Missing columns** — the thing was never measured at all
- **Missing rows** — whole people or places absent from the dataset
- Only the first is visible in the spreadsheet
- The other two are the ones that change your conclusions

> This is the absence audit — step 2 of the assignment and 30% of the mark. It is also the step where humanities training is a genuine advantage. Empty cells are easy: COUNTBLANK finds them. The other two require you to ask what the record was for and who made it, which is source criticism.

## Empty cells: check before you average

*SECTION 1.1*

- `=COUNTBLANK(range)` gives the count immediately
- Your Codebook sheet gives a missing percentage for every column
- Excel's AVERAGE ignores blanks — so it averages a smaller group than you think
- A column that is 60% empty cannot support a confident claim
- Report the number of rows your figure is actually based on

> The point about AVERAGE silently ignoring blanks is the practical one. If a column is 60% missing, the average is of the 40% that remain — and those are usually not a random 40%. Always report the n alongside the average.

## Missing columns: what was never measured

*SECTION 2*

- The films data has no budget for most African films — so no budget analysis
- The heritage data has no coordinates — so no map without joining something else
- The artworks data has no acquisition column — so it cannot tell you what was looted
- No amount of cleverness recovers a column that is not there
- Naming this early saves you a wasted afternoon

> The artworks example is the sharpest. That dataset shows African objects sitting in European museums, and the question everyone immediately wants to ask is how they got there. The dataset simply cannot say. Recognising that in the first ten minutes is worth more than any statistic they could compute.

## Missing rows: who is not counted

*SECTION 2.1*

- The voyages data names ships and captains — and not one enslaved person
- The scholarship data misses journals that global databases do not index
- The films data reflects who edits Wikipedia, not who makes films
- Absence is rarely random — it usually follows power
- Ask: who made this record, and for what purpose?

> This is the most important slide in the six decks. Every dataset was created by someone, for a purpose, and what they did not record tells you about that purpose. The voyages example is the clearest and the most sobering: the records are administratively meticulous about cargo and silent about people, because that is what the record was for. Students who see this are doing digital humanities, not just data analysis.

## How to write it up

*SECTION 3*

- One short section: 'What this data does not record'
- Name a missing variable, a missing population, a granularity limit
- Then say what each one stops you claiming
- Be specific — 'correlation is not causation' alone earns nothing
- This is 30% of the mark and the easiest part to do well

> Give them the template explicitly, because a structure removes anxiety. Three bullets and a consequence each. The instruction to be specific is worth labouring: a generic caveat signals that they did not look, whereas 'this dataset has no acquisition column, so we cannot distinguish purchase from looting' shows they did.

## Try it before Wednesday

*SECTION 4*

- Open your Codebook and find the column with the most missing data
- Write one sentence on what that stops you saying
- Read the 'Known limits' section — it is written for you
- Read the 'trap' in your BRIEF.md — every dataset has one
- Arrive with those two sentences and you have started the assignment

> If they do only one of the six exercises, this is the one. It requires no software skill at all and it produces text that goes directly into their final write-up.

---

## Before Wednesday

Do the five-minute exercise at the end of each deck, and bring one question about your dataset. A question is good preparation, not a gap to hide.
