# Reading Code Without Writing It

*Six of you asked for this. It is a real skill on its own*

One of six short pre-workshop guides. No previous data or coding experience is assumed.

---

## You can read code you could not write

*SECTION 1*

- This is normal, and true of most people who use code
- Reading is a separate skill from writing, and it is learnable faster
- The goal: look at a cell and say what it does and what comes out
- You do not need to be able to produce it from a blank page
- Your walkthrough notebook is written to be read, not filled in

> Say this plainly, because it addresses the anxiety directly. Understanding what a piece of analysis does is the skill that lets you evaluate someone else's work, which is what scholars mostly need. Being able to type it from memory is a separate, more mechanical skill.

## Four things to look for in any line

*SECTION 1.1*

- **What goes in?** Usually a table, often called `df`
- **What is the verb?** `groupby`, `mean`, `sort_values`, `plot`
- **What comes out?** A number, a smaller table, or a chart
- **Is it saved?** An `=` means the result is kept under a name
- Read left of the `=` last: it is just the label on the result

> This gives them a procedure rather than a vibe. Most lines of analysis code are 'take this table, do this verb, keep the result'. Once they see that shape, unfamiliar code becomes much less threatening.

## A line, read slowly

*SECTION 2*

- `df.groupby('country')['visits'].mean()`
- `df` — the whole table
- `.groupby('country')` — put the rows into piles, one per country
- `['visits']` — from each pile, look only at the visits column
- `.mean()` — average it. One number per country

> Walk this left to right at the pace of speech. Then say the crucial thing: this is a pivot table. They built the same thing in deck four by dragging. The code and the pivot table are the same operation in two notations, and neither is more real than the other.

## The same operation, three ways

*SECTION 2.1*

- **Excel:** drag `country` to Rows, `visits` to Values, set to Average
- **Python:** `df.groupby('country')['visits'].mean()`
- **English:** 'the average number of visits, for each country'
- Learn to translate between the three and code stops being foreign
- Start from the English. Always

> This slide is the heart of the deck. If they can move between the three notations they can work with either tool and, more importantly, they can check whether a piece of code does what its author claims.

## Errors are not failure

*SECTION 3*

- A red error message is the computer being specific, not being angry
- Read the **last** line first — that is the actual problem
- `KeyError: 'Country'` means the column is not spelled that way
- `FileNotFoundError` means it cannot find the file, not that you broke it
- Nothing you do in a notebook can damage the data

> This addresses the fear directly and concretely. Most beginner paralysis comes from thinking an error means they have broken something. Point out that the data file is separate and read-only in effect — the worst case is closing the notebook and reopening it. The KeyError example is worth demonstrating live because capitalisation errors are the most common thing that will happen to them.

## Try it before Wednesday

*SECTION 4*

- Open your dataset's `walkthrough.ipynb` in Google Colab
- Run the cells in order — just press play, do not change anything
- Read the comment above each cell before you look at the code
- Find one cell and write, in English, what it does
- Then change one thing — a column name, a number — and run it again

> The last instruction is where the learning is. Changing one value and seeing the output change is the moment code stops being magic. Reassure them that breaking the notebook is fine and expected — they can reload it.

---

## Before Wednesday

Do the five-minute exercise at the end of each deck, and bring one question about your dataset. A question is good preparation, not a gap to hide.
