# MMAT v.2018 codebook — HPV_PSCC

Appraisal tool for empirical studies in the FT Included cohort.
Reviews / overviews without primary data: `mmat_category=NA`,
`overall_judgment=NA`.

## Categories (`mmat_category`)

| Code | When |
|---|---|
| `qualitative` | Qualitative designs |
| `rct` | Randomized trials |
| `non_randomized` | Cohort / case-control / non-rand comparative |
| `descriptive` | Prevalence / case series / single-arm descriptive |
| `mixed_methods` | Mixed methods |
| `NA` | Narrative/systematic review, commentary, methods-only |

## Screening (all empirical)

- `screen_clear_question`: yes/no — clear research question
- `screen_data_address_question`: yes/no — collected data address the question  
If either is `no` → do not continue criteria; `overall_judgment=cannot_appraise`.

## Criteria (1–5)

Judgments: `yes` | `no` | `cant_tell`  
Store short rationale in `rationale_*`.

Domain labels follow Hong et al. MMAT 2018 by category (see tool PDF).
We record criteria as `c1`…`c5` with category-specific meaning noted in
`criteria_note` when helpful.

## Overall

`overall_judgment`: `high` | `moderate` | `low` | `cannot_appraise` | `NA`  
Heuristic (empirical only):

- `high`: all answered criteria `yes` (no `no`/`cant_tell`)
- `moderate`: at most one `no`/`cant_tell`
- `low`: two or more `no`/`cant_tell`
- `cannot_appraise`: failed screening or insufficient text

## Columns

record_id, study_label, mmat_category, screen_clear_question,
screen_data_address_question, c1, c2, c3, c4, c5,
rationale_c1, rationale_c2, rationale_c3, rationale_c4, rationale_c5,
overall_judgment, criteria_note, reviewer_id, assessed_at, assessment_note
