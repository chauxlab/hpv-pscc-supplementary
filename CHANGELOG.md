# Changelog

## 2026-10-27 — Corrections made at proof stage (Manuscript 4GARYD)

Production review of the galley proofs showed that four included studies co-authored by A.C. appeared in File S2, while only one (reference 12) had been appraised independently. The following was done and is reflected in the proofs approved by both authors.

### Independent extraction and appraisal (P.B. alone) of three further studies
File S2 entries 10 (Canete-Portillo et al., Int J Surg Pathol 2026, doi:10.1177/10668969251362475), 11 (Canete-Portillo et al., medRxiv 2024, doi:10.1101/2024.12.11.24318853) and 14 (Chaux and Canete-Portillo, Surg Pathol Clin 2025, doi:10.1016/j.path.2024.12.001) were extracted and appraised from the full text by P.B., blinded to the earlier single-reviewer records.

- Entry 10: N = 23, HPV stratification partial (morphology only), MMAT non-randomized, low.
- Entry 11: N = 108 (spots are the unit of analysis), HPV not assessed, MMAT non-randomized, low.
- Entry 14: narrative review, MMAT not applicable.
- Entries 9 to 11 derive from the same parent tissue-microarray cohort (108 patients, 528 spots).

Independent records: `extraction/HPV_PSCC_extraction_independent_PB_entries10-11-14_2026-10-27.csv` and `risk_of_bias/HPV_PSCC_mmat_independent_PB_entries10-11_2026-10-27.csv`. The corresponding rows in the full-corpus files were replaced by these records.

### Four rows recoded after reading the full text
Four rows had been coded as randomized trials in the single-reviewer pre-fill. Details in `extraction/corrections_2026-10-27_four_rows.csv`.

| Study | Was | Now |
|---|---|---|
| Alencar 2022 | RCT, N = 30 | Narrative review, MMAT not applicable |
| Lloyd 2024 | Clinical trial, N = 125, HPV yes | One-page comment (PubMed type Comment), MMAT not applicable. The PDF previously archived under this record was another article (Buonerba 2017). |
| Necchi 2022 | Clinical trial | Retrospective genomic profiling study (descriptive), N = 230 penile, MMAT descriptive, low |
| Rouvinov 2023 | RCT, N = 18 | Retrospective observational case series (4 eligible, 3 evaluable), MMAT descriptive, low |

The MMAT category of Gambale 2022, Borcoman 2025, Cotait Maluf 2025 and Xu 2026 in the single-reviewer file was aligned with the dual-reconciled appraisal (Gambale: not applicable; the other three: descriptive).

### Figures that changed as a result (121 reports / 119 unique studies)
- Publication types (121 reports): original research 83, case reports 12, narrative reviews or commentaries 13, trials 4, meta-analyses 4, systematic reviews 4, case series 1 (previously 85/12/9/6/4/4/1). Apolo 2024 is recorded as a phase I trial; Gambale 2022 as a narrative review/perspective.
- HPV stratification: 76/121 reports (yes 74; partial 2), i.e. 75/119 unique studies (previously 80/121 in the manuscript text).
- MMAT overall rating, 119 unique studies: low 81, moderate 18, not applicable 20 (previously low 84, moderate 19, not applicable 18).
- Table S4 appraisal source: dual 21, P.B. alone 3, single reviewer 95.

### Files updated
`manuscript/hpv-scc-supplementary-table-s4.csv` and `.md`, `manuscript/hpv-scc-supplementary-prisma-checklist.md`, `manuscript/hpv-scc-supplementary-included-studies.md` (entry 11 note), `manuscript/hpv-scc-manuscrito.md` (counts, HPV figure, shared-cohort sentence in Limitations), `extraction/HPV_PSCC_extraction_wide_2026-08-25.csv`, `risk_of_bias/HPV_PSCC_mmat_singlereviewer_full_corpus.csv`, `README.md`.

The wording changes made by the journal during production (title, affiliations, abbreviations, statement on the use of artificial intelligence, conflict-of-interest text) are not mirrored in `manuscript/`; the published article is the reference text. The dual-reconciled files for the 24 Category A sources are unchanged.
