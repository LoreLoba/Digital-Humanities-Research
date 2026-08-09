# Humanities researchers on research data management — codebook

**One row is** one survey response from a humanities researcher.

A 2022 survey of humanities researchers about how they manage, store and share research data. Rich in categorical answers and free text, which makes it the best dataset in the pack for cross-tabulation and for coding open-ended responses by hand.

- **Rows:** 372
- **Columns:** 22 (22 of 115 source columns)
- **Source:** [Figshare — STM humanities subgroup survey 2022](https://figshare.com/articles/dataset/21207239)
- **Licence:** CC BY 4.0
- **Attribution:** STM Association humanities subgroup (2022), via Figshare. CC BY 4.0.
- **Retrieved:** 2026-08-09

## Columns

| Column | Type | Description | % missing | Distinct | Example |
|---|---|---|---:|---:|---|
| `respondent_id` | number | Respondent id | 0.3 | 371 | 114016773780.0 |
| `start_date` | date | Start date | 0.3 | 371 | 2022-04-25 14:40:16 |
| `end_date` | date | End date | 0.3 | 371 | 2022-04-25 14:55:50 |
| `are_you_happy_for_your_anonymised_answers_to_be_shared_online` | text | Are you happy for your anonymised answers to be shared online | 0.0 | 2 | Response |
| `in_which_humanities_discipline_is_your_research_based` | text | In which humanities discipline is your research based | 10.2 | 12 | Response |
| `how_many_research_articles_have_you_published_in_academic_journals_or_conference_proceedings` | text | How many research articles have you published in academic journals or conference proceedings | 10.5 | 7 | Response |
| `how_long_have_you_been_an_active_researcher_in_the_humanities` | text | How long have you been an active researcher in the humanities | 10.5 | 7 | Response |
| `in_what_region_are_you_based` | text | In what region are you based | 10.5 | 9 | Response |
| `what_is_your_gender` | text | What is your gender | 10.5 | 5 | Response |
| `do_you_recognise_the_term_research_data_as_a_supporting_output_of_your_research_process` | text | Do you recognise the term research data as a supporting output of your research process | 17.2 | 4 | Response |
| `what_terminology_do_you_feel_best_describes_the_information_that_supports_the_outcomes_of_your_research_to_help_with_understanding_and_clarity_we_will_use_the_term_research_data_in_the_remainder_of_this_survey` | text | What terminology do you feel best describes the information that supports the outcomes of your research to help with understanding and clarity we will use the term research data in | 16.9 | 7 | Response |
| `how_important_do_you_think_research_data_management_is_for_research_studies_in_the_humanities_please_select_one_answer` | text | How important do you think research data management is for research studies in the humanities please select one answer | 17.2 | 5 | Response |
| `how_important_do_you_think_it_is_to_share_research_data_with_others_in_the_humanities_please_select_one_answer` | text | How important do you think it is to share research data with others in the humanities please select one answer | 16.7 | 5 | Response |
| `do_you_consider_how_you_will_manage_your_research_data_while_in_the_planning_stages_of_your_project` | text | Do you consider how you will manage your research data while in the planning stages of your project | 21.8 | 5 | Response |
| `are_you_aware_of_the_concept_of_a_data_management_plan` | text | Are you aware of the concept of a data management plan | 22.3 | 4 | Response |
| `have_you_ever_completed_a_data_management_plan_for_a_project` | text | Have you ever completed a data management plan for a project | 22.6 | 4 | Response |
| `do_you_have_access_to_funds_to_help_with_any_costs_involved_in_research_data_management_for_example_long_term_preservation_or_curation` | text | Do you have access to funds to help with any costs involved in research data management for example long term preservation or curation | 22.3 | 4 | Response |
| `what_are_the_biggest_challenges_you_have_in_planning_the_research_data_considerations_of_a_new_research_project_please_select_all_that_apply` | text | What are the biggest challenges you have in planning the research data considerations of a new research project please select all that apply | 69.9 | 1 | Lack of training/support |
| `unnamed_24` | text | Unnamed 24 | 57.3 | 1 | Lack of funding |
| `do_you_generate_your_own_research_data_in_the_course_of_your_research_practice` | text | Do you generate your own research data in the course of your research practice | 26.6 | 4 | Response |
| `what_tools_equipment_have_you_used_to_capture_research_data_select_all_that_apply` | text | What tools equipment have you used to capture research data select all that apply | 54.0 | 1 | Physical notebooks |
| `unnamed_29` | text | Unnamed 29 | 55.4 | 1 | Electronic lab/notebooks |

## What was done to the source data

- Column headers (long question text) normalised to snake_case.
- Kept 22 columns answered by more than a quarter of respondents; the rest were near-empty and would only add noise.
- Rows that were entirely blank removed.

## Known limits

- Self-selected respondents — not a random sample of humanities researchers.
- One point in time (2022); nothing here supports a claim about change.
- Free-text answers are unedited and inconsistent in length and language.
