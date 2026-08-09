# What Is a Dataset?

*Before any analysis: what are you actually looking at?*

One of six short pre-workshop guides. No previous data or coding experience is assumed.

---

## One row is one thing

*SECTION 1*

- Every dataset answers the question: one row is one *what*?
- In your films dataset, one row is one film
- In your libraries dataset, one row is one library system — not one building
- In your voyages dataset, one row is one voyage — not one person
- Get this wrong and every number you calculate afterwards is wrong

> This is the single most important idea in the whole workshop, and it is not technical at all. Before you compute anything, say out loud what one row represents. The libraries example is the one that catches people: a row is a library *system*, which might be one rural branch or a city system with sixty buildings. If you average across rows you have averaged those two together as if they were the same kind of thing. The voyages example matters even more: a row is a voyage, not a person, so counting rows counts ships, not people.

## The three questions to ask of any table

*SECTION 1.1*

- **What is one row?** The unit of analysis
- **What is one column?** A single property, measured the same way for every row
- **How many rows and columns?** The shape
- You can answer all three by looking — no code needed
- Your codebook answers all three on its first page

> Every dataset in your pack ships with a CODEBOOK.md, and the first thing it tells you is what one row is. Read that before you open the data. The shape — how many rows and columns — tells you what kind of work is possible: 115 rows you can read end to end; 40,000 rows you cannot, and you will have to summarise.

## Tidy data: the shape that makes life easy

*SECTION 2*

- One row per observation, one column per variable, one value per cell
- No merged cells, no headers halfway down, no colour-coding as data
- Your datasets are already tidy — this is what 'prepared' meant
- Real archival data almost never arrives this way
- Most data work is getting from messy to tidy

> Your datasets have been cleaned into this shape deliberately, so you can spend the workshop on reasoning rather than on wrangling. Be aware that this is not what data looks like when you find it. A spreadsheet where someone has colour-coded rows to mean something is storing information in a way no software can read. The rule of thumb: if you had to explain the colours to a colleague, the colours are data and belong in a column.

## What a column is not

*SECTION 2.1*

- Not a place for two facts — 'Lagos, Nigeria' should be two columns
- Not a place for units — put '30' in the cell and '%' in the column name
- Not a place for notes — a comment column is fine, mixed-in notes are not
- A column should be answerable the same way for every single row

> This matters because you will be filtering and sorting. If one cell says '30%' and another says 'about thirty per cent', a filter cannot see they are the same. This is also why your data has separate columns for country and city where the source combined them.

## Try it before Wednesday

*SECTION 3*

- Open your group's `data.xlsx`
- Say out loud: one row is one ______
- Count the columns. Read three column names in the Codebook sheet
- Find one column you do not understand and write down the question
- That question is a good thing to bring, not a gap to hide

> The exercise takes five minutes and it is the whole foundation. Bringing a question about a column is exactly the right preparation — it means you read the data. Nobody in the room has seen your dataset before either.

---

## Before Wednesday

Do the five-minute exercise at the end of each deck, and bring one question about your dataset. A question is good preparation, not a gap to hide.
