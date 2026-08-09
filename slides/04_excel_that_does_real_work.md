# Excel That Does Real Work

*Four skills that cover most of the assignment*

One of six short pre-workshop guides. No previous data or coding experience is assumed.

---

## Why Excel is a serious tool here

*SECTION 1*

- Five of you asked for this, and it is the right instinct
- Everything in the assignment can be done in Excel
- Filter, sort, pivot table, one chart — that is the whole toolkit
- Your workbook already has three sheets: Data, Codebook, Source
- The reasoning is what is being marked, not the software

> Say this explicitly at the start. There is a persistent idea that Excel is the beginner's tool and Python the real one. For a table of a few thousand rows that is simply false — a pivot table answers 'average X by Y' faster than writing code does. What Python adds is repeatability, not correctness.

## Skill 1 — Freeze, filter, sort

*SECTION 2*

- **Freeze panes** so the header row stays visible when you scroll
- **Filter** (the funnel icon) to see only some rows
- Filtering does not delete anything — it hides
- **Sort** to find the extremes: the largest, the smallest
- Always sort a numeric column before believing you know its range

> The Data sheet in their workbook already has the header frozen and an autofilter applied, so these are one click. Worth demonstrating live: filter to one country, watch the row count at the bottom change. That count is a real finding — it is how many rows match.

## Skill 2 — The pivot table

*SECTION 2.1*

- Insert → PivotTable. The single most useful thing in Excel
- Drag a **categorical** column to Rows
- Drag a **numeric** column to Values
- Change 'Sum' to 'Average' or 'Count' in the value settings
- You have just compared groups — assignment step 4, done

> Demonstrate this slowly. A pivot table is exactly the 'group by' operation that in Python takes a line of code, and it is drag-and-drop. Most people's first pivot table sums when they wanted an average, so point at the value settings explicitly. Counting is often more useful than averaging when the column is categorical.

## Skill 3 — Five formulas worth knowing

*SECTION 2.2*

- `=AVERAGE(range)` and `=MEDIAN(range)` — and deck 5 explains when to prefer which
- `=COUNTA(range)` — how many cells actually have something in them
- `=COUNTBLANK(range)` — how many are empty. Your missing-data check
- `=COUNTIF(range, "Kenya")` — how many rows match a condition
- That is enough for most of the assignment

> Deliberately five, not fifty. COUNTBLANK is the one people never learn and it is the fastest possible absence audit: run it on every column and you have a missingness profile in two minutes. The Codebook sheet already reports missing percentages, so they can check their formula against it — a good way to build confidence that they used it correctly.

## Skill 4 — One chart, made deliberately

*SECTION 3*

- Bar chart for comparing categories. Sort it first, always
- Line chart for change over time, and only for time
- Histogram for the shape of one numeric column
- Bars must start at zero — a truncated bar exaggerates the difference
- Give it a title that states the finding, not the column names

> The sorting point is the one that most improves a student chart. An unsorted bar chart makes the reader do the ranking; a sorted one hands it to them. And a title saying 'Coastal sites are listed in danger more often' is worth far more than one saying 'Category by Danger'.

## Try it before Wednesday

*SECTION 4*

- Open your `data.xlsx` and make one pivot table — any two columns
- Run `=COUNTBLANK` on three columns and compare to the Codebook sheet
- Make one bar chart and sort it
- It does not have to be interesting. It has to exist
- Doing this once removes most of the fear

> This is the highest-value preparation on any of the six decks. The point is not the output; it is that they have already done the mechanical steps once, so the workshop can be about judgement rather than about finding the menu.

---

## Before Wednesday

Do the five-minute exercise at the end of each deck, and bring one question about your dataset. A question is good preparation, not a gap to hide.
