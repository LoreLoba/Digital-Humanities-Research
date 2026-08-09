# Data Types

*Why the kind of data decides what you can do with it*

One of six short pre-workshop guides. No previous data or coding experience is assumed.

---

## Four kinds of column

*SECTION 1*

- **Categorical** — a label. Country, category, pass/fail
- **Numeric** — a quantity. Budget, population, number of visits
- **Date or time** — a point in time. Year inscribed, month of pageviews
- **Text** — free writing. A description, an open survey answer
- The type decides which questions and which charts are possible

> This is the concept most worth having before Wednesday. Everything else follows from it. You cannot take an average of a country name, and a bar chart of every unique description is meaningless. When you look at a column, name its type first; the method follows almost automatically after that.

## Categorical splits in two

*SECTION 1.1*

- **Nominal** — labels with no order: Nigeria, Kenya, Egypt
- **Ordinal** — labels with a real order: primary, secondary, tertiary
- Ordinal can be ranked; nominal cannot
- 'Cultural / Natural / Mixed' in the heritage data is nominal
- A survey's 'strongly agree → strongly disagree' is ordinal

> The distinction matters when you summarise. For ordinal data a median makes sense — the middle answer on a scale is meaningful. For nominal data it does not: there is no middle country. The commonest mistake is coding a survey scale as 1-5 and then taking a mean, which quietly assumes the gap between 'agree' and 'strongly agree' is the same size as between 'neutral' and 'agree'. It might not be.

## Numeric splits in two

*SECTION 1.2*

- **Discrete** — counts. Number of branches, number of authors. No halves
- **Continuous** — measures. Area, ratio, percentage. Halves are fine
- A count of 2.4 libraries is a sign something has gone wrong
- An average of 2.4 libraries per system is perfectly sensible

> The distinction sounds pedantic but catches real errors. If a value that should be a count comes out fractional in your raw data, something has gone wrong. But an average of counts is legitimately fractional — an average household of 4.2 people describes a population, not a household.

## What each type lets you do

*SECTION 2*

- Categorical → count, group by, bar chart, pivot table
- Numeric → mean, median, spread, histogram, scatter plot
- Date → sort, group by year, line chart over time
- Text → read it, code it into categories, then treat as categorical
- Categorical + numeric together → compare groups. This is most of the workshop

> Pin this slide. 'Compare groups' means splitting on a categorical column and summarising a numeric one — average budget by pass/fail, visits per person by urban and rural. That single move is the backbone of step 4 of your assignment, and it is a pivot table in Excel.

## Text is data too

*SECTION 2.1*

- Free text is the humanities' home ground — do not skip it
- The usual move: read a sample, invent categories, code each response
- That coding is a scholarly judgement, and you must document it
- Once coded, text behaves like any categorical column
- The survey dataset is built for exactly this

> This is where humanities training is an advantage rather than a handicap. Deciding that fifteen different free-text answers are all versions of the same concern is interpretive work, and it is the part a statistician often does worst. Write down your category definitions as you go; that document is part of your method, not a private note.

## The type is not always what the file says

*SECTION 3*

- A year stored as text will sort 1900, 1901, 1902, 200 — wrongly
- A number with a stray space becomes text and stops adding up
- 'N/A', '-', 'unknown' and blank are four different things to software
- Your datasets have had this cleaned already — real ones will not
- In Excel: numbers align right, text aligns left. A quick visual check

> The right-align trick is genuinely useful and takes a second. If a column of numbers is left-aligned, Excel thinks it is text and your sums will silently be wrong. This is the single most common spreadsheet bug in the world and you can spot it by looking.

## Try it before Wednesday

*SECTION 4*

- Open the Codebook sheet of your workbook
- It gives a type for every column — check three against the data itself
- Find one categorical and one numeric column that could be compared
- Write down the comparison as a sentence: 'average ___ by ___'
- That sentence is the beginning of your assignment

> This exercise produces the seed of their analytical question. If they arrive with 'average budget by pass/fail' written down, they are already at step 4.

---

## Before Wednesday

Do the five-minute exercise at the end of each deck, and bring one question about your dataset. A question is good preparation, not a gap to hide.
