# Protocolo operativo — HPV_PSCC

**Título:** The Immune Microenvironment in Penile Squamous Cell Carcinoma:
Distinctions Between HPV-Driven and HPV-Independent Pathways

**Tipo de revisión:** Integrativa
**Idioma del manuscrito:** Inglés
**Marco utilizado:** PICO
**Fecha de búsqueda:** 2026-08-13
**review_id:** `SR-HPV-PSCC` · **review_slug:** `HPV_PSCC`
**Registro externo (OSF/PROSPERO):** No registrado. PROSPERO no aplica a
revisiones integrativas. Se ofreció al usuario la opción de registrar el
protocolo en OSF; queda pendiente para una futura sesión si el usuario lo
solicita. `protocol_ref: pending` en `review.yaml`.

## Origen del expediente

Esta revisión rehace, con cribado doble independiente desde el inicio, el
corpus de evidencia que sustentó el manuscrito original de pSCC/TIME
(expediente 4GARYD en el histórico editorial), tras la crítica de revisor
único recibida en el peer review de ese manuscrito. El corpus se construyó en
REDACTOR (`manuscritos/hpv-scc/r1/`) mediante búsqueda estructurada en dos
canales bibliográficos más un canal adicional de literatura ya citada por el
usuario, y se transfiere aquí como RIS intermedio ya deduplicado para que el
cribado título/abstract lo hagan dos revisores humanos independientes.

## Pregunta de revisión

En pacientes con carcinoma escamocelular de pene (pSCC), ¿cómo difiere la
composición del microambiente inmune tumoral (TIME) — incluyendo infiltrado
de linfocitos T CD8+, expresión de PD-L1, Tregs, macrófagos asociados a tumor
(TAM) y otros checkpoints inmunes — entre los tumores HPV-driven y
HPV-independent, y qué implicancias tiene esta distinción para el pronóstico
y la respuesta a inmunoterapia?

## PICO

- **P (Población):** Pacientes con carcinoma escamocelular de pene (pSCC).
- **I/C (Intervención/Concepto):** Composición del microambiente inmune
  tumoral (TIME), estratificada por estado HPV (driven vs. independent).
- **C (Comparador/Contexto):** HPV-positivo vs. HPV-negativo/independiente.
- **O (Desenlaces):** Composición inmune (CD8/TIL, PD-L1, Tregs, TAM,
  checkpoints), respuesta a inmunoterapia, pronóstico.

## Ecuaciones de búsqueda

### Canal A — Europe PMC

1. `(TITLE:"penile" OR ABSTRACT:"penile") AND (TITLE:"squamous" OR ABSTRACT:"squamous cell carcinoma") AND ("human papillomavirus" OR HPV) AND ("tumor immune microenvironment" OR "tumor microenvironment" OR "immune infiltrate" OR "immune microenvironment")`
2. `(TITLE:"penile" OR ABSTRACT:"penile") AND (TITLE:"squamous" OR ABSTRACT:"squamous cell carcinoma") AND ("PD-L1" OR "tumor-infiltrating lymphocytes" OR TIL OR CD8 OR "regulatory T cells" OR Treg OR "tumor-associated macrophages" OR TAM OR TIGIT OR "immune checkpoint")`
3. `(TITLE:"penile" OR ABSTRACT:"penile") AND (TITLE:"squamous" OR ABSTRACT:"squamous cell carcinoma") AND (immunotherapy OR "checkpoint inhibitor" OR "immune checkpoint blockade" OR pembrolizumab OR nivolumab OR atezolizumab OR PERICLES OR HERCULES)`

### Canal B — MEDLINE

1. `("penile squamous cell carcinoma"[tiab] OR "penile cancer"[tiab] OR "penile carcinoma"[tiab]) AND ("human papillomavirus"[tiab] OR HPV[tiab]) AND ("tumor immune microenvironment"[tiab] OR "tumor microenvironment"[tiab] OR "immune infiltrate"[tiab] OR "immune microenvironment"[tiab])`
2. `("penile squamous cell carcinoma"[tiab] OR "penile cancer"[tiab]) AND ("PD-L1"[tiab] OR "tumor-infiltrating lymphocytes"[tiab] OR TIL[tiab] OR CD8[tiab] OR "regulatory T cells"[tiab] OR Treg[tiab] OR "tumor-associated macrophages"[tiab] OR TAM[tiab] OR TIGIT[tiab] OR "immune checkpoint"[tiab])`
3. `("penile squamous cell carcinoma"[tiab] OR "penile cancer"[tiab]) AND (immunotherapy[tiab] OR "checkpoint inhibitor"[tiab] OR "immune checkpoint blockade"[tiab] OR pembrolizumab[tiab] OR nivolumab[tiab] OR atezolizumab[tiab] OR PERICLES[tiab] OR HERCULES[tiab])`

### Canal C — fuente adicional ("identificados por otros métodos")

RIS de Paperpile depositado por el usuario (`Paperpile - HPV_PENILE - 13
ago.ris`), 27 registros = bibliografía citada en el manuscrito R0 original
(4GARYD). Detalle de clasificación conservado en REDACTOR
(`manuscritos/hpv-scc/r1/ris-previo-triage.md`, fuera de este repo, solo
lectura).

### División de responsabilidad de fuentes (Paso 0-C)

No aplica — solo conectores disponibles en la sesión de búsqueda (Europe PMC
vía Canal A, MEDLINE vía Canal B). Bases sin conector (Embase, Cochrane
CENTRAL, PsycINFO, LILACS, Web of Science, SciELO) no se ejecutaron; si el
usuario decide ampliar cobertura, deberán ejecutarse aparte y sus resultados
incorporarse como fuente adicional declarada en este expediente.

## Contabilidad PRISMA (n reales)

| Etapa | n |
|---|---|
| Canal A (Europe PMC) — búsqueda 1 | 71 |
| Canal A (Europe PMC) — búsqueda 2 | 178 |
| Canal A (Europe PMC) — búsqueda 3 | 188 |
| Canal A — subtotal bruto | 437 |
| Canal A — únicos (dedup interno por PMID/epmcId) | 240 |
| Canal B (MEDLINE) — búsqueda 1 | 31 |
| Canal B (MEDLINE) — búsqueda 2 | 137 |
| Canal B (MEDLINE) — búsqueda 3 | 139 |
| Canal B — subtotal bruto | 307 |
| Canal B — únicos (dedup interno por PMID) | 202 |
| Canal C (RIS previo, elegibles tras excluir 4 citas metodológicas) | 23 |
| Combinado A+B+C antes de deduplicación cruzada | 472* |
| **Tras deduplicación por DOI/PMID y reglas de sustitución/exclusión** | **318** |

\* 240 (A únicos) + 202 (B únicos) + 23 (C elegibles), sin restar aún
duplicados cruzados A∩B/A∩C/B∩C.

- **n_canal_a** (Europe PMC, interno): 437 brutos / 240 únicos tras dedup
  interno.
- **n_canal_b_medline:** 307 brutos / 202 únicos tras dedup interno.
- **n_combinado_antes_deduplicación** (A únicos + B únicos, antes de cruzar
  A×B): 442.
- **n_tras_deduplicación_doi:** 318 (corpus final único, tras cruzar A×B por
  PMID/DOI y fusionar Canal C).
- **Canal C declarado aparte** (PRISMA "identificados por otros métodos", no
  como línea de base de datos): 23 candidatos elegibles; 21 coincidieron por
  DOI con registros ya presentes en A/B (dedup cruzado), 2 se incorporaron
  como únicos nuevos (Ribera-Cortada 2021 SR, Cao 2021 — DOIs no capturados
  por las ecuaciones de A/B).
- **Corpus ingresado a SQLite (este expediente):** 318 registros (verificado
  en intake, ver `logs/workflow-log.md`).

Referencia metodológica: `modulos/scite-protocolo.md` §5.1 (repo REDACTOR).

### Reglas de deduplicación y sustitución aplicadas antes del conteo final

1. **Exclusión del autopreprint:** Chaux A., "The Immune Microenvironment in
   Penile Squamous Cell Carcinoma...", Preprints.org, DOI
   10.20944/preprints202604.0995.v1 (epmcId PPR1177582) — excluido del
   corpus de cribado por ser la revisión misma, no una fuente de evidencia
   (decisión del usuario, 2026-08-13).
2. **Sustitución preprint → publicado:**
   - PPR954027 (medRxiv 10.1101/2024.12.11.24318871) → sustituido por PMID
     40905728 (DOI 10.1177/10668969251361176, *Int J Surg Pathol* 2025).
   - PPR965148 (medRxiv 10.1101/2025.01.11.25320379) → sustituido por PMID
     40938921 (DOI 10.1177/10668969251362475, *Int J Surg Pathol* 2025).
   - PPR954030 ("Machine Learning Analysis of PD-L1 and CD8...", DOI
     10.1101/2024.12.11.24318853) — se buscó explícitamente una versión
     publicada del mismo grupo (Cañete-Portillo/Chaux) en Europe PMC el
     2026-08-13; **no se encontró**. Se mantiene el preprint en el corpus,
     marcado como pendiente de verificación editorial (es el único registro
     del corpus sin DOI resuelto de forma estándar, ver
     `archive/intake_2026-08-13/derived/intake_summary.md`).

## Criterios de elegibilidad

### Inclusión

- Estudios (cualquier diseño: experimental, observacional, serie/reporte de
  caso, ensayo clínico, revisión) que reporten composición del
  microambiente inmune tumoral (TIME) y/o estado HPV en pacientes humanos
  con carcinoma escamocelular de pene (pSCC), incluyendo al menos uno de:
  infiltrado linfocitario (CD8/TIL), PD-L1, Tregs, TAM, otros checkpoints
  inmunes, respuesta a inmunoterapia o correlación con pronóstico.
- Estudios en inglés o español, sin restricción de fecha de publicación.
- Revisiones sistemáticas, narrativas y meta-análisis relevantes se incluyen
  como candidatos para contextualización, sujetos a cribado.

### Exclusión

- **Estudios en especies no humanas.** El corpus incluye 6 estudios de pSCC
  **equino** (modelo animal; Porcellato et al. 2020, 2021; Armando et al.
  2021; Bacci et al. 2025; Miglinci et al. 2023; da Silva et al. 2022) —
  **se marcan como candidatos a exclusión por especie, no se eliminan
  silenciosamente del RIS**; la decisión final de exclusión queda en manos
  del cribado humano en REVISOR (R1/R2 deben aplicar el mismo criterio
  explícitamente, no asumir exclusión automática).
- Estudios sin relación con pSCC (p. ej. cáncer de próstata, cáncer oral
  HPV-asociado usado solo como contexto) — a cribar caso por caso.
- Las 4 citas metodológicas del RIS previo (Page 2021 PRISMA, Sterne 2016
  ROBINS-I, Sterne 2019 RoB2, Whittemore 2005) ya se excluyeron del corpus
  de cribado antes de la importación — van directo a la sección de Métodos
  del nuevo manuscrito, no son candidatas a inclusión/exclusión en este
  expediente.
- El autopreprint de Chaux A. (Preprints.org) — ya excluido antes de la
  importación, ver reglas de deduplicación arriba.

## Herramienta de appraisal

**MMAT v.2018** (Mixed Methods Appraisal Tool), dado que el corpus mixto
incluye estudios cuantitativos observacionales (la mayoría), un ensayo
clínico (PERICLES, HERCULES), series/reportes de caso y revisiones. Si tras
el cribado a texto completo el subconjunto incluido resulta predominantemente
de un solo diseño, considerar aplicar además la checklist JBI específica del
diseño (ver `conocimientos/revisor-integrativo-sesion1.md` §FASE 2.6 en
REDACTOR) como complemento del MMAT para ese subgrupo.

## Scope de búsqueda contextual (Sesión 2 — REDACTOR)

No sujeta a los criterios de elegibilidad de este protocolo; se declara aquí
solo como referencia para cuando el corpus incluido pase a redacción.

- **Términos:** Epidemiología y carga de enfermedad del pSCC (incidencia,
  prevalencia regional, factores de riesgo); guías clínicas vigentes EAU
  (European Association of Urology) y ASCO/NCCN para manejo de cáncer de
  pene, incluyendo recomendaciones sobre inmunoterapia.
- **Período:** Últimos 10 años (2016–2026).
- **Propósito declarable:** Búsqueda complementaria para fundamentar
  Introducción y Discusión, no sujeta a los criterios de elegibilidad del
  protocolo de esta revisión integrativa.

## Nota — coautoría del usuario en el corpus (conflicto de interés potencial)

Los siguientes registros del corpus tienen coautoría del usuario (Chaux A.)
y deben tenerse en cuenta durante el cribado independiente (posible riesgo
de sesgo de autoría; ambos revisores lo consideran, no solo REV-PAOLA):

| PMID / DOI | Título | Nota |
|---|---|---|
| PMID 27663086 | Immune-checkpoint status in penile squamous cell carcinoma: a North American cohort | Cocks, Netto, Chaux et al. |
| PMID 39890300 | Molecular Pathology and Biomarkers of Penile Squamous Cell Carcinoma: Implications for Classification and Management | Coautoría Chaux (revisión) |
| PMID 40905728 | Interplay of PD-L1, FOXP3, and CD8 in the Immune Microenvironment of Penile Squamous Cell Carcinoma | Cañete-Portillo, Cubilla, Netto, Chaux — versión publicada, sustituye preprint PPR954027 |
| PMID 40938921 | Characterization of CD8+ and FOXP3+ T-Cell Ratios in Tumor and Stromal Compartments of Penile Squamous Cell Carcinoma | Cañete-Portillo, Cubilla, Netto, Chaux — versión publicada, sustituye preprint PPR965148 |
| DOI 10.1101/2024.12.11.24318853 (preprint, sin PMID) | Machine Learning Analysis of PD-L1 and CD8 Expression Patterns in Penile Squamous Cell Carcinoma | Cañete-Portillo, Chaux et al. — preprint medRxiv sin versión publicada verificada al 2026-08-13; pendiente de verificación editorial |

## Hallazgo adicional respecto al triage previo

El ensayo **HERCULES** (LACOG 0218, pembrolizumab + quimioterapia basada en
platino), cuya ausencia se había señalado como brecha en el triage previo,
**sí apareció** en los resultados de Canal A/B de esta sesión: PMID
40965911 (ensayo principal, *JAMA Oncol* 2025, DOI
10.1001/jamaoncol.2025.3266), más un comentario "Re:" asociado y una revisión
que lo discute. Queda incorporado al corpus.

## Revisores asignados

- **R1:** Alcides Chaux (`REV-ALCIDES`)
- **R2:** Andrea Paola Britos Gómez (`REV-PAOLA`)
- IDs reutilizados del sistema (ya existentes desde `ctDNA_GU`), no
  reasignados ni recreados.
- Cribado título/abstract: **doble e independiente desde el inicio** (a
  diferencia del expediente original del manuscrito 4GARYD, que tuvo
  revisor único).

## Archivo RIS intermedio

- Nombre: `cribado-pscc-time-2026-08.ris`
- Ubicación en este expediente: `searches/ris/cribado-pscc-time-2026-08.ris`
- Total de registros: 318 (todos con campo AB completo; 16 registros llevan
  el placeholder `[Resumen no disponible]` porque el artículo original
  —cartas, comentarios "Re:", reportes breves— no tiene abstract
  estructurado en PubMed/Europe PMC).

## Estado

Protocolo cerrado para intake. Cribado título/abstract (R1/R2) pendiente de
inicio — ver `logs/workflow-log.md` y `logs/decision-log.md`.
