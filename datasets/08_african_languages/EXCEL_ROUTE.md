# African languages — Glottolog — the Excel route

Every step of the assignment, done in Excel. No code at all.

Open **`data.xlsx`**. It has three sheets: **Data**, **Codebook** (what every column means) and **Source** (where it came from and how to cite it).

One row is one language or dialect spoken in Africa.

---

## 1. Frame your question

On the Codebook sheet, find one categorical column and one numeric column.
For this dataset, `level` and `n_countries` work well.

Write your question as a sentence: **average n_countries by level**.

## 2. The absence audit — worth 30% of the mark

The Codebook sheet already gives a **missing %** for every column. Read it.

To check it yourself, on the Data sheet use `=COUNTBLANK(C2:C1000)` on a column.

Then ask the harder questions, which no formula answers:

- What was never measured at all? (a missing **column**)
- Who is not in the table? (missing **rows**)
- Is the detail too coarse for your question?

The **Known limits** section of `CODEBOOK.md` is written to help you here.

## 3. Describe

Select the `n_countries` column and read the status bar at the bottom of the window — Excel shows Average and Count without you doing anything.

For the median use `=MEDIAN(range)`. **If the mean and median are far apart, the data is skewed and the median is the honest summary.** Say which you used.

## 4. Compare groups — the pivot table

This is the most important skill and it is drag-and-drop.

1. Click any cell in the data, then **Insert → PivotTable → OK**
2. Drag **`level`** into **Rows**
3. Drag **`n_countries`** into **Values**
4. Click the value, choose **Value Field Settings**, change **Sum** to **Average**
5. Drag **`n_countries`** in a second time and set it to **Count**

You now have the average and the group size side by side. **Ignore any group with fewer than about five rows** — an average of two things is not a finding.

## 5. Is the difference real?

Take your two largest groups. In Excel:

```
=T.TEST(range1, range2, 2, 3)
```

That gives a p-value. Below 0.05 means the difference is unlikely to be chance.

For the size of the difference, subtract the two averages and divide by `=STDEV.S(all values)`. Roughly: 0.2 small, 0.5 medium, 0.8 large.

**Report both.** A p-value alone says nothing about whether the difference matters.

## 6. One chart

1. **Sort your pivot table** by the average, largest first
2. Select it and **Insert → Bar chart**
3. Check the axis starts at zero — a truncated bar exaggerates differences
4. Title it with your **finding**, not the column names

Good: *Urban library systems record twice the visits per person of rural ones*
Weak: *Average visits by locale*

## 7. Limits

One page. Your finding, how you got it, how confident you are, and — specifically — what this data cannot support.

**The trap in this dataset:** The rows are not all the same kind of thing: `level` distinguishes languages from dialects and families. Counting all rows and calling the answer 'languages in Africa' inflates it substantially. Filter on `level` first and say which you counted.

---

**Source:** [Glottolog CLDF — languages.csv](https://glottolog.org/)  
**Licence:** CC BY 4.0  
**Cite as:** Hammarström, Forkel, Haspelmath & Bank, Glottolog. CC BY 4.0.
