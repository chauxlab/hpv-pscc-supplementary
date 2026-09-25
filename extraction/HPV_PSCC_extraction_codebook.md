# Extraction codebook — HPV_PSCC

Wide-form CSV, one row per FT Included `record_id` (n=121).
English values/notes. `NR` = not reported; `NA` = not applicable.

Review: *The Immune Microenvironment in Penile Squamous Cell Carcinoma:
Distinctions Between HPV-Driven and HPV-Independent Pathways*
(`integrative_review`, `SR-HPV-PSCC`)

## Core rules

1. Numeric fields: plain numbers (no units/% symbols in numeric columns;
   percents go in `*_pct` fields as numbers 0–100).
2. `publication_type`: `original_research` | `narrative_review` |
   `systematic_review` | `meta_analysis` | `case_report` | `case_series` |
   `trial` | `other`.
3. `relation_type`: `primary_report` | `review` | `case_report` |
   `secondary_analysis`.
4. `study_design`: free text (e.g. `retrospective cohort`, `RCT`,
   `narrative review`).
5. `hpv_stratified`: `yes` | `no` | `partial` | `NR`.
6. `time_markers`: comma-separated controlled tokens from:
   `PD-L1`, `PD-1`, `CD8`, `TIL`, `FOXP3`, `Treg`, `TAM`, `CD68`, `CD163`,
   `CTLA-4`, `TIGIT`, `LAG-3`, `TIM-3`, `IDO1`, `HLA`, `TLS`, `NLR`,
   `IL-12`, `other_checkpoint`, `other_immune`.
7. `clinical_focus`: comma-ok from:
   `TIME_composition` | `HPV_pathway` | `immunotherapy_response` |
   `prognosis` | `overview`.
8. `extraction_status`: `complete` | `partial` | `pending` | `needs_review`.
9. `needs_review`: `yes` | `no`.

## Minimum for `complete`

- `study_label`, `publication_type`, `study_design`, `population_description`,
  `clinical_focus`,
- and **at least one** of:
  `key_finding_time`, `key_finding_hpv`, `key_finding_prognosis`,
  `key_finding_immunotherapy`, or (reviews) substantive `other_key_outcomes`.

## Integrative notes

- Narrative/systematic reviews **in scope** for contextualization;
  set `n_patients=NR`.
- Stratify synthesis by HPV status (when reported) and by marker/domain,
  not by pooling heterogeneous assays.
- Appraisal: **MMAT v.2018** for empirical studies; reviews → MMAT `NA`.

## Column dictionary

| Column | Meaning |
|---|---|
| record_id | Canonical ID |
| study_label | AuthorYear |
| relation_type | Report role |
| publication_type | Controlled vocab |
| study_design | Free text |
| country_setting | Countries / centres |
| funding | Funder |
| conflicts_of_interest | COI |
| n_patients | Analytic N |
| population_description | Brief population |
| hpv_stratified | Controlled |
| hpv_method | p16 / PCR / ISH / NR |
| hpv_positive_pct | % HPV+ if reported |
| time_markers | Token list |
| time_compartment | tumor / stroma / both / NR |
| immunotherapy_agent | Agents or NR |
| immunotherapy_setting | advanced / neoadjuvant / NR / NA |
| clinical_focus | Controlled |
| primary_aim_as_stated | Aim |
| key_finding_time | TIME composition finding |
| key_finding_hpv | HPV± immune distinction |
| key_finding_prognosis | Prognostic association |
| key_finding_immunotherapy | IT response / trials |
| limitations_as_stated | Limitations |
| other_key_outcomes | Other / review synthesis |
| extractor_id | Extractor |
| extraction_status | Controlled |
| extraction_note | Caveats |
| needs_review | yes/no |
