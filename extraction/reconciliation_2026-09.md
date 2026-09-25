# Reconciliación de extracción y apreciación — núcleo probatorio (24 fuentes Categoría A)

**Revisión:** HPV_PSCC / SR-HPV-PSCC — *The Immune Microenvironment in Penile SCC* (Manuscript ID 4GARYD).
**Fecha:** 2026-09-06.
**R1 (extracción original):** REV-ALCIDES — extracción asistida por texto, 2026-08-25
(`analysis/HPV_PSCC_synthesis_characteristics_2026-08-25.csv`,
`risk_of_bias/HPV_PSCC_mmat_assessments_2026-08-25.csv`).
**R2 (segunda extracción independiente, ciega):** REV-PAOLA (Paola Britos) — desde PDF completo.
23 fuentes devueltas 2026-09-03; ref 12 (COI) devuelta 2026-09-06 tras segundo pedido.
**Las 24/24 completas.**
(`extraction/exports/2026-08-31__extraccion-R2-britos/returned/HPV_PSCC_extraction_R2_FILLED.csv`,
`…/HPV_PSCC_mmat_R2_FILLED.csv`).

Alcance: las 24 fuentes citadas individualmente en el manuscrito (refs 10–33), que alimentan
Tablas 1, 2 y 4. El resto del corpus (95 estudios) mantiene extracción simple + QC y no entra
en esta reconciliación.

---

## 1. Resumen cuantitativo

**Extracción** — 145 celdas comparables (7 campos × ~21 filas con dato en ambas fuentes):

| | n | % |
|---|---:|---:|
| Acuerdo exacto | 87 | 60 % |
| R2 completa un campo que R1 dejó en `NR`/`NA` (mejora, no conflicto) | 24 | 17 % |
| **Compatibles (acuerdo + relleno de vacío)** | **111** | **77 %** |
| Conflicto real o R2 rebaja a `NR` | 34 | 23 % |

De los 34 «no triviales», la mayoría son **diferencias de convención de codificación resueltas
a favor de R2** (§2) y **8 son correcciones de fondo que sí afectan al manuscrito** (§3).

**MMAT** — 20 filas empíricas apreciadas por ambos (21 previstas − ref 33 reclasificada a NA):

| | acuerdo |
|---|---:|
| Categoría MMAT | 9/20 (45 %) |
| Juicio global | 9/20 (45 %) |

El bajo acuerdo MMAT **no refleja disputa de fondo** sino que la apreciación de R1 fue una
plantilla heurística por categoría (mismos rationales genéricos «sampling/eligibility signals…»
en las 21 filas) que además clasificó mal varios diseños. La de R2 es una apreciación real
criterio por criterio, con rationale específico por dominio — **se adopta la de R2 en bloque**
(cierra también el pedido del Revisor 4 de «justificación por dominio, no etiqueta»).

---

## 2. Diferencias de convención — resueltas a favor de R2 (sin volver al PDF caso por caso)

1. **`time_compartment` = `both` (R2) en vez de `tumor` (R1)** para refs 10, 14, 15, 16, 18, 22,
   23, 24, 30, 31, 32. R1 puso `tumor` por defecto; R2 documenta que estos estudios puntúan PD-L1
   por CPS (células tumorales + linfocitos + macrófagos) y/o cuantifican densidades en compartimento
   tumoral **y** estromal. Convención de R2 adoptada; se anota en Métodos que la mayoría de las
   cohortes con IHC informan ambos compartimentos.
2. **`hpv_method` — R2 reemplaza `NR`/`p16` genérico de R1 por el ensayo real** en 12 fuentes
   (GP5+/6+ PCR, Cobas, LCD-Array, qPCR Hybribio, NGS, clon de p16, etc.). Mejora directa del
   campo que 4 revisores marcaron como faltante. Adoptado.
3. **`hpv_positive_pct` — R2 completa el % HPV+ en 17 fuentes que R1 dejó en `NR`.** Adoptado
   (con las salvedades de denominador que R2 anota en `extraction_note` por estudio).
4. **`country_setting` — R2 completa país + centro(s) en las 21 fuentes empíricas** (R1: `NR` en
   todas). Adoptado.

---

## 3. Conflictos de fondo — resueltos por consenso contra el PDF

| Ref | Campo | R1 | R2 | Resolución (contra PDF) | Impacto manuscrito |
|----:|---|---|---|---|---|
| 29 Apolo 2024 | publication_type / N | original_research / 120 | trial / 11 | **R2.** Es el ensayo fase I CaboNivo(Ipi); 120 = canasta multitumoral, 11 = subgrupo de pene (9 evaluables). | Tabla 1: «Observational \| 120» → «Trial (fase I) \| 11». Tabla 4: cat `descriptive` (no `rct`). |
| 30 Borcoman 2025 | N / hpv_stratified | 107 / no | 11 / yes | **R2.** Ensayo canasta fase 2 (PEVO); 107–111 = todo el ensayo, 11 = cohorte de pene. Análisis HPV+ agrupado entre sitios SCC pero estratificado. | Tabla 1: N 107 → 11. Tabla 4: cat `rct` → `descriptive`. |
| 31 Cotait Maluf 2025 (HERCULES) | hpv_stratified / MMAT | no / low | yes / moderate | **R2.** Hay análisis exploratorio por HPV16 (ORR 55,6 % vs 35 %). N=37 concuerda. | Tabla 4: cat `rct`→`descriptive`, juicio `low`→`moderate`. |
| 32 Xu 2026 | N | 17 | 25 | **R2** con nota: 25 = población de seguridad/eficacia declarada en Resumen/§3.1; 17 = subgrupo neoadyuvante-evaluable; 24 = denominador de la Tabla 3. Se registra N=25 y se anota la inconsistencia interna de la fuente. | Tabla 1: N 17 → 25. Tabla 4: cat `rct`→`descriptive`. |
| 33 Gambale 2022 | publication_type / N | trial / 608 | narrative_review / NR | **R2.** *J Immunother Cancer* 2022, «cemiplimab: ongoing and future perspectives» — es un comentario/revisión narrativa, sin cohorte propia de pSCC. El «608» y «clinical trial» de R1 son un error de la extracción asistida. | **Corrección de error existente.** Tabla 1: «Clinical trial \| 608» → «Narrative review \| NR». Tabla 4: `rct/low` → `NA/NA`. Sigue válida como cita contextual (Tablas 2/3, dominio «checkpoints exploratorios»). |
| 25 El Zarif 2023 | hpv_stratified | yes | partial | **R2.** HPV conocido en 49/92 (53 %); el contraste HPV+/− existe pero sobre denominador parcial. | Texto/Tabla 1: matizar a «HPV parcialmente informado». |
| 12 Canete-Portillo 2026 | hpv_stratified / hpv_method | yes / NR | partial / NR | **R2.** El «HPV status» no es molecular: se infiere de la morfología (subtipos HPV-asociados WHO 2022), sin p16/PCR/ISH. Los propios autores lo señalan como limitación. Estudio a nivel de *spot* de TMA (108 pacientes, hasta 528 spots), sin análisis de sobrevida. `country_setting=NR` (los 108 especímenes no tienen origen declarado; posible solapamiento con el archivo paraguayo de Chaux et al. 2013, no confirmado en Métodos). | Tabla 1: método HPV se mantiene «NR»; MMAT `moderate`→`low`. |
| 28 Taghizadeh & Fajkovic 2025 | immunotherapy_setting | neoadjuvant | advanced | **R2.** Toda la evidencia de ICI revisada es en enfermedad avanzada/refractaria; lo neoadyuvante es prospectivo/aspiracional. | Sin impacto en tablas (es revisión). |
| 21 Necchi 2023 | hpv_method | NR | NGS | **R2.** Detección de HPV por secuenciación de nueva generación. | Tabla 1: «NR» → «NGS». |

---

## 3b. Hallazgo colateral — títulos de referencias incorrectos en el manuscrito

Al cotejar los títulos de la lista de Referencias contra los títulos reales de los PDF
(extracción de R2), **17 de las 24 entradas (refs 11–33) tenían el título parafraseado o
inventado**, no el título publicado. Ejemplos: ref 13 figuraba como «Distinct spatial macrophage
and dendritic cell subsets…» cuando el real es «Distinct patterns of myeloid cell infiltration…»;
ref 15 como «Tertiary lymphoid structures and antitumor immunity…» cuando el real es «A B
cell-IgA-epithelial axis enhances antitumor immunity…». Los DOI y revistas eran correctos; la
verificación bibliográfica de la sesión 3 comprobó el mapeo cita↔referencia y los datos
numéricos, pero no los títulos literales.

**Corregidos los 24 títulos** en `r2/hpv-scc-manuscrito.md` con el título exacto de cada PDF.

**Verificación completa contra PubMed (2026-09-07)** — Scite (`bibliography`) devolvió 502 y
`search_literature` devolvió resultados corruptos (química/oceanografía), así que se usó el
conector PubMed (fallback aprobado). Los 24 DOI resuelven a PMID; los 24 títulos coinciden 1:1
con PubMed. **Añadidos volumen(issue):páginas verificados** a las 24 entradas:

| Ref | Antes | PubMed |
|----:|---|---|
| 11 | Cancers 2020;12:1796 | 12(7):1796 |
| 12 | Int J Surg Pathol 2026 (sin vol) | 34(1):73-79 — PubMed [DP]=2025 pero vol 34 = año 2026; se mantiene 2026, **único punto ambiguo, verificar** |
| 14 | Cancers 2026;18:257 | 18(2):257 |
| 15 | Nat Commun 2025 | 17(1):624 (5.º autor corregido Zhang Y→Zhang P) |
| 16 | BMC Urol 2024 | 24(1):165 |
| 17 | J Urol 2015 | 193(4):1245-51 (Heideman DAM→DA) |
| 18 | Clin Transl Oncol 2022 | 24(2):331-341 |
| 20 | JNCCN 2026 | 24(8):e267025 |
| 21 | JAMA Netw Open 2023 | 6(12):e2348002 |
| 22 | Am J Clin Pathol 2024 | 161(1):49-59 |
| 23 | Pathology 2023 | 55(5):637-649 |
| 25 | J Natl Cancer Inst 2023 | 115(12):1605-1615 |
| 26 | Virchows Arch 2025 | 487(3):687-699 |
| 27 | Cancer 2024 | 130(9):1650-1662 |
| 28 | Cancers 2025;17:883 | 17(5):883 |
| 29 | J Clin Oncol 2024 | 42(25):3033-3046 |
| 30 | Nat Cancer 2025 | 6(8):1370-1383 |
| 31 | JAMA Oncol 2025 | 11(11):1314-1320 |
| 32 | Front Immunol 2026 | 17:1731920 |
| 33 | J Immunother Cancer 2022 | 10(1):e003540 — PubMed la clasifica **Editorial**, coherente con «revisión narrativa/perspectiva» de R2 |

Primeros autores de las 24: coinciden con PubMed. Coautores 2–6 verificados donde PubMed devolvió
la lista completa (refs 15, 20, 24, 30, 31, 32); en el resto PubMed solo devuelve el primer autor
+ conteo y las listas existentes son plausibles y consistentes con el conteo.

## 4. MMAT — adopción de la apreciación de R2

Se adopta íntegra la apreciación de R2 (categoría + c1–c5 + rationale por dominio + juicio global).
Cambios respecto de la tabla actual del manuscrito (Tabla 4):

| Ref | Cat. actual | Cat. R2 | Juicio actual | Juicio R2 |
|----:|---|---|---|---|
| 10 Ottenhof 2018 | descriptive | non_randomized | moderate | moderate |
| 11 Chu 2020 | descriptive | non_randomized | low | low |
| 12 Canete-Portillo 2026 | descriptive | **non_randomized** | moderate | **low** |
| 13 Rafael 2021 | non_randomized | non_randomized | low | low |
| 14 Fazili 2026 | non_randomized | non_randomized | moderate | **low** |
| 15 Tao 2025 | non_randomized | non_randomized | low | low |
| 16 Tang 2024 | descriptive | **non_randomized** | moderate | **low** |
| 17 Djajadiningrat 2015 | non_randomized | non_randomized | moderate | **low** |
| 18 Müller 2022 | descriptive | **non_randomized** | moderate | **low** |
| 21 Necchi 2023 | non_randomized | non_randomized | low | low |
| 22 Lobo 2024 | descriptive | **non_randomized** | moderate | moderate |
| 23 Hrudka 2023 | non_randomized | non_randomized | low | **moderate** |
| 24 Tan 2025 | descriptive | **non_randomized** | moderate | **low** |
| 25 El Zarif 2023 | descriptive | **non_randomized** | moderate | **low** |
| 26 Stenzel 2025 | non_randomized | non_randomized | moderate | **low** |
| 27 Wei 2024 | non_randomized | non_randomized | low | low |
| 29 Apolo 2024 | descriptive | descriptive | moderate | **low** |
| 30 Borcoman 2025 | rct | **descriptive** | low | low |
| 31 Cotait Maluf 2025 | rct | **descriptive** | low | **moderate** |
| 32 Xu 2026 | rct | **descriptive** | low | low |
| 33 Gambale 2022 | rct | **NA (revisión narrativa)** | low | **NA** |

Distribución MMAT del núcleo probatorio tras R2 (24 fuentes):
**moderate 4 (Ottenhof 10, Lobo 22, Hrudka 23, Cotait Maluf 31), low 16, NA 4 (refs 19, 20, 28 y 33).**
→ refuerza la lectura del manuscrito de que la evidencia primaria es mayoritariamente de baja
calidad metodológica.

---

## 5. Ref 12 (Canete-Portillo 2026, `REC-HPVPSCC-000252`) — RESUELTA

R2 la devolvió en blanco en la primera vuelta. **Decisión del usuario (2026-09-06):** volver a
Britos con un paquete de una sola fila (`extraction/exports/2026-09-06__ref12-britos/`). Britos
devolvió la fila completa el **2026-09-06** — extracción `complete` + MMAT `non_randomized / low`
con rationale por dominio, verificadas:

- **Extracción:** estudio translacional transversal sobre TMA (4 TMAs, 528 spots de 108
  pacientes); N analítico = 108 (pero casi todo el análisis es a nivel de *spot*); PD-L1/FOXP3/CD8
  en compartimento tumoral y estromal; **sin análisis de sobrevida ni inmunoterapia**.
  `hpv_stratified = partial`, `hpv_method = NR` (HPV inferido por morfología WHO 2022, no molecular).
  `country_setting = NR` — R2 anota el posible solapamiento con el archivo paraguayo de Chaux et al.
  2013 (no confirmado en Métodos).
- **MMAT `low`:** c3 `no` (FOXP3 cuantificado en solo 80/528 spots, atrición no explicada),
  c4 `no` (sin modelo multivariable; sin ajuste por *clustering* intra-paciente de múltiples spots).
- **COI:** el propio estudio no declara financiamiento ni conflictos; el conflicto es de nivel
  meta-revisión (Chaux coautor) y la extracción/apreciación las hizo R2 sin ese conflicto —
  **exactamente lo que pidió el Revisor 2.**

Cambios al manuscrito: Tabla 1 MMAT `moderate`→`low`; Tabla 4 `descriptive/moderate` →
`non_randomized/low`.

---

## 6. Propagación al manuscrito — HECHA (2026-09-06)

Aplicado en `REDACTOR/manuscritos/hpv-scc/r2/`:

1. ✅ **Tabla 1** reescrita (diseño según categorías de apreciación; N analítico = subgrupo de
   pene en los ensayos canasta; método HPV verbatim; hallazgo clave de R2; MMAT de R2) + pie nuevo.
2. ✅ **Tabla 4** regenerada con R2 (cohortes comparativas → `non_randomized`; ensayos de brazo
   único → `descriptive`; ref 33 → `NA`) + pie nuevo.
3. ✅ **Tabla 3** — ref 33 pasa a soporte contextual en la fila de ICI (n 6→5); fila de
   «checkpoints exploratorios» de ref 33 → refs 11,24.
4. ✅ **Métodos** «Data extraction and critical appraisal» — dos revisores independientes para
   las 24, reconciliación por consenso; resto single-reviewer + QC.
5. ✅ **Resultados** — HPV stratification 80/121 (yes 76; partial 4); MMAT whole-corpus
   recalculado (low 84, moderate 19, NA 18); «Quality appraisal» reescrito.
6. ✅ **Limitations** — párrafo de extracción acotado al corpus secundario; frase de Tabla 4
   reescrita; cláusula de COI ref 12.
7. ✅ **Referencias** — 24 títulos corregidos (§3b).
8. ✅ **Carta de respuesta** — Revisor 2 Partes 1/3, Revisor 4 Parte 3/6, guía editorial, tabla
   de alcance y «Comentarios pendientes»: clúster D → «resuelto para el núcleo probatorio».

9. ✅ **Verificación bibliográfica final contra PubMed** — 24 títulos + volumen(issue):páginas
   añadidos y verificados (§3b). `.docx` de `r2/` regenerados (los 3).

**Pendiente (revisión humana):** (a) confirmar el año de la ref 12 (2025 vs 2026 — ambigüedad
epub/issue); (b) revisión humana del manuscrito y la carta; (c) reenvío de 4GARYD y cierre.
