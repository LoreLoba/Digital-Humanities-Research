# Group assignment — working with a DH dataset

You have four hours of methods behind you. This assignment asks you to run the same arc on a dataset nobody has walked you through.

Every group does the same seven steps on a different dataset, so the presentations compare and you can see how much of the method is general and how much is about the particular data.

## What each group gets

A folder containing `data.csv`, `data.xlsx` (Data / Codebook / Source sheets), `CODEBOOK.md`, `BRIEF.md` and `starter.ipynb`. Use Excel or Python — the assignment is about the reasoning, not the tool.

## The seven steps

**1. Frame.** Write one **descriptive** question and one **analytical** question this dataset can actually answer. Say which method each needs.

**2. Absence audit.** What did this dataset never record? Name a missing variable, a missing population, and a level of detail that is too coarse. Which absence most limits your questions?

**3. Describe.** Summarise the variable at the centre of your question. Choose between mean and median deliberately and justify it — for skewed data one of them describes nothing real.

**4. Compare.** Split the data into two groups that matter and compare them. State the size of the difference in the units a reader thinks in.

**5. Test.** Could that difference be chance? Run an appropriate test **and** report an effect size. If you test more than one thing, correct for it.

**6. Show.** One chart. Sorted deliberately, with a reference line if there is a meaningful threshold, and a caption saying what you filtered.

**7. Limits.** One page: your finding, the method, the uncertainty, and an explicit list of sentences this data does **not** support.

## What to hand in

- **A one-page brief** — your finding, the method, the uncertainty, and an explicit list of sentences the data does not support.
- **One chart**, captioned, saying what you filtered.
- **Your workbook or notebook**, so the steps can be checked.
- **Five minutes** presenting the finding and the limits.

## How it is marked

| Weight | What we are looking for |
|---:|---|
| 30% | **The absence audit.** Did you work out what the data never recorded, and did that change what you claimed? |
| 25% | **Method fit.** Did you choose statistics the data can support, and justify the choice — median over mean where it matters, effect size alongside any p-value? |
| 20% | **Honest limits.** Are the sentences you rule out as specific as the ones you assert? |
| 15% | **The chart.** Sorted deliberately, reference line where one exists, caption that states the filter. |
| 10% | **Reproducibility.** Could someone else follow your steps and get your number? |

A group that finds no significant difference and says so clearly scores better than one that finds a spurious result and presents it confidently. The point of the method arc is knowing what you cannot conclude.

## Dataset allocation

| # | Dataset | One row is | Rows | Suits a group interested in |
|---|---|---|---:|---|
| 01 | Humanities researchers on research data management | one survey response from a humanities researcher | 372 | survey data, qualitative coding, cross-tabulation |
| 02 | Bechdel test results for 1,794 films | one film | 1,794 | film, gender, what a metric does not measure |
| 03 | Knoedler stock books — the New York art market | one transaction recorded in the Knoedler gallery stock books | 40,253 | art markets, provenance, historical records |
| 04 | US public libraries — staffing, funding and use | one public library system in the 2020 financial year | 9,245 | institutions, public services, funding |
| 05 | Journal of Open Humanities Data — every paper | one data paper published in JOHD | 365 | scholarly communication, open data |
| 07 | Trans-Atlantic slave trade — voyages | one recorded slaving voyage | 36,110 | African diaspora history, archives and silence |
| 08 | African languages — Glottolog | one language or dialect spoken in Africa | 8,037 | language, linguistic diversity, mapping |
| 09 | African films on Wikidata | one film with an African country of origin | 5,582 | African cinema, knowledge-base coverage |
| 10 | African-origin objects in museum collections | one object, in one museum collection | 1,928 | museums, restitution, cultural property |
| 11 | UNESCO World Heritage sites in Africa | one inscribed World Heritage site | 115 | heritage, conservation, international policy |
| 12 | Digital humanities research from African institutions | one publication with at least one African institutional affiliation | 3,500 | the DH field itself, bibliometrics, open access |
| 13 | Wikipedia attention to African writers | one writer in one month | 750 | reception, attention, literary celebrity |
| 06 | Geographic Locations in English-Language Literature, 1701-2011 *(download it yourselves)* | a place mentioned in a literary volume | — | literary geography, place and text |

> **Geographic Locations in English-Language Literature, 1701-2011** — HathiTrust-derived. Licence not stated on the source page, so this pack documents it and links to it rather than redistributing it. A group taking this option downloads it themselves and checks the terms.

## A note on dataset 07

The trans-Atlantic slave voyages dataset records voyages that carried enslaved people. It is offered because it is foundational to African diaspora digital humanities and because learning to work with it carefully is worth doing — not as a counting exercise. Any group taking it should begin with the absence audit and should be ready to say who the records name and who they do not. Groups may choose a different dataset without giving a reason.
