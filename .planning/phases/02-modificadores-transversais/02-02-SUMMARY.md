---
phase: 02-modificadores-transversais
plan: "02"
subsystem: osteoporosis-protocol
tags: [osteoporose, FRAX, T-score, restricoes-carga-ossea, modificador-transversal, HEP-aderencia, Sinaki-1984]
dependency_graph:
  requires: [protocols/SHARED-FOUNDATION.md, protocols/P-01-OSTEOARTRITE.md, protocols/P-08-SARCOPENIA.md]
  provides: [protocols/P-04-OSTEOPOROSE.md]
  affects: [protocols/SHARED-FOUNDATION.md, all 20 protocols — bone-loading constraint modifier]
tech_stack:
  added: []
  patterns:
    - "WHO T-score + FRAX dual-stratification for 4 fracture risk categories (Baixo/Médio/Alto/Muito Alto)"
    - "Bone-loading constraint table (MODIFICADOR TRANSVERSAL) — 3-axis: espinal/impacto/resistência"
    - "Hip hinge universal precaution technique — mandatory in all phases for all patients"
    - "Cross-protocol reference to P-08 Seção 6.3 for resistance dosing in osteosarcopenia"
    - "Long-term HEP adherence strategies with pictographic instructions and monthly check-in"
    - "8 clinical validity questions template — Section 15 (consistent with P-01 and P-08)"
key_files:
  created:
    - protocols/P-04-OSTEOPOROSE.md
  modified:
    - protocols/SHARED-FOUNDATION.md
decisions:
  - "[02-02]: FRAX + T-score dual-stratification adopted — T-score alone subestima risco (maioria das fraturas ocorre com T-score > -2.5)"
  - "[02-02]: 4 fracture risk categories (Baixo/Médio/Alto/Muito Alto) stratified by T-score + FRAX + fracture history + OWD"
  - "[02-02]: Spinal extension exercises recommended (Nível B, Sinaki 1984) — hip hinge as universal precaution for all categories"
  - "[02-02]: Impacto moderado recomendado (não contraindicado) para Baixo/Médio Risco — UK consensus: 5.8% fractures in exercise vs 9.6% controls"
  - "[02-02]: P-08 Seção 6.3 cross-referenced (not re-derived) for resistance dosing — preserves modifier chain integrity"
  - "[02-02]: Osteosarcopenia: co-tratamento P-04 + P-08 simultâneo com P-04 Seção 5.2 como teto de carga"
metrics:
  duration_minutes: 12
  completed_date: "2026-03-13"
  tasks_completed: 2
  tasks_total: 2
  files_created: 1
  files_modified: 1
  lines_written: 1059
requirements_satisfied: [PROT-03]
---

# Phase 2 Plan 02: P-04 Osteoporose Protocol Summary

**One-liner:** Complete osteoporosis rehabilitation protocol with authoritative cross-protocol bone-loading constraint table (4 risk categories × 3 restriction axes) as the normative reference for all 20 protocols in the series, with cross-reference to P-08 for resistance dosing and long-term HEP adherence strategies.

---

## What Was Built

### Task 1: P-04-OSTEOPOROSE.md (1059 lines)

Created a complete 15-section geriatric rehabilitation protocol for osteoporosis in Brazilian Portuguese, TIDieR/CERT compliant, with:

**Section 1 — Critérios Diagnósticos e de Inclusão:**
- WHO BMD T-score categories (Normal ≥ -1.0; Osteopenia -1.0 to -2.5; Osteoporose ≤ -2.5; Osteoporose Estabelecida = T-score ≤ -2.5 + fratura por fragilidade)
- FRAX Brasil model integration — limiares: fratura maior < 10%/10–20%/> 20%; quadril < 3%/3–10%/> 10%
- Critical note: T-score alone subestima risco — maioria das fraturas ocorre com T-score > -2.5
- Inclusion: T-score ≤ -2.5 OR osteopenia with FRAX above thresholds, age ≥ 60
- Exclusion: metastatic bone disease, acute unstable vertebral fracture (< 6 weeks), Paget active phase

**Section 2 — Avaliação Inicial Mandatória:**
- TUG + SPPB-BR + Dinamometria (inherited SHARED-FOUNDATION)
- Avaliação postural: occiput-to-wall distance (OWD > 5 cm = hipercifose = Muito Alto Risco regardless of T-score)
- Height measurement: loss ≥ 4 cm = suspect vertebral fracture
- FRAX calculation procedure (online tool, Brazil model) with documentation instructions
- Fracture risk category determination table (Seção 2.5)

**Section 5.2 — MODIFICADOR TRANSVERSAL (Bone-Loading Constraint Table):**
- 4 fracture risk categories (Baixo/Médio/Alto/Muito Alto) × 6 restriction columns (flexão espinal / rotação espinal / impacto / carga de resistência / supervisão)
- Labeled as authoritative cross-protocol reference for all P-01 to P-20
- General spinal rule: extension RECOMMENDED (Nível B, Sinaki 1984, PubMed 6487063)
- Hip hinge as universal precaution for ALL patients and ALL categories
- Cross-reference to P-08 Seção 6.3 for resistance dosing in Muito Alto Risco and osteosarcopenia

**Section 10 — Polifarmácia:**
- 6 SHARED-FOUNDATION base classes + 6 osteoporosis-specific: Bifosfonatos (sinergia com exercício), Denosumabe (ONJ awareness), SERMs/Raloxifeno (VTE risk), Romosozumabe/Teriparatida (anabólico + exercise synergy), Corticosteroides crônicos (GICO mechanism), Suplementos Ca/Vitamina D (scope note)
- Sinergia bifosfonato + exercício explicitly documented (BHOF 2022) — motivação de aderência

**Section 15 — 8 Questões de Validade Clínica:**
- All 8 questions answered with section cross-references
- Replicates P-01 and P-08 template for series consistency

### Task 2: SHARED-FOUNDATION.md — P-04 Row

Updated Section 8.1 cross-reference matrix:
- 9 comorbidity interactions: P-08, P-01, P-05, P-07, P-09, P-10, P-11, P-16, P-19
- Shared modifier: bone-loading constraint table reference with category descriptions
- Specific precautions: FRAX + T-score dual stratification; acute vertebral pain = suspend immediately; osteosarcopenia co-treatment rule

---

## Verification Results

All 12 verification criteria from the plan confirmed:

| # | Criterion | Status |
|---|-----------|--------|
| 1 | P-04-OSTEOPOROSE.md exists with ≥ 15 sections | PASS — 15 sections |
| 2 | MODIFICADOR TRANSVERSAL label present | PASS — 2 occurrences (Seção 5.2) |
| 3 | Constraint table covers 3 axes: espinal/impacto/resistência | PASS — 6 occurrences of axis headers |
| 4 | FRAX referenced alongside T-score in constraint stratification | PASS — 48 total references |
| 5 | P-08 cross-referenced for resistance dosing in kinesiotherapy section | PASS — 4 explicit mentions in dosage context |
| 6 | Sinaki 1984 (PubMed 6487063) cited for spinal extension evidence | PASS — 7 occurrences |
| 7 | Long-term HEP adherence strategies included | PASS — 18 occurrences (HEP + aderência) |
| 8 | All exercises have two-column dosage tables with 3 frailty rows | PASS — 12 table header occurrences |
| 9 | Section 15 answers all 8 clinical validity questions | PASS — Q1 through Q8 |
| 10 | SHARED-FOUNDATION.md Section 8.1 P-04 row populated | PASS — bea4c3d |
| 11 | P-08 and P-04 mutually cross-referenced and consistent | PASS — P-08 in P-04: 10 refs; P-04 in P-08: 4 refs |
| 12 | Entire document in Brazilian Portuguese | PASS |

Automated term-count verification: 139 matches (threshold: 35 — exceeded 4× over).

---

## Commits

| Task | Commit | Message |
|------|--------|---------|
| 1 | bdbc3c6 | feat(02-02): create P-04-OSTEOPOROSE.md — complete 15-section geriatric rehabilitation protocol |
| 2 | bea4c3d | feat(02-02): update SHARED-FOUNDATION cross-reference index with P-04 row |

---

## Deviations from Plan

None — plan executed exactly as written.

The plan specified the MODIFICADOR TRANSVERSAL in Seção 5 (Fase 1 Cinesioterapia) — placed precisely in Seção 5.2 as a prominent labeled blockquote with the full 4-category × 3-axis constraint table. The hip hinge was included as a universal precaution for all categories as specified. P-08 cross-reference was included in both the constraint table (Muito Alto Risco cell) and the resistance dosing section of Fase 2 Cinesioterapia (Seção 6.3.1). All 6 osteoporosis-specific polypharmacy classes from the plan specification were included plus all 6 SHARED-FOUNDATION base classes.

---

## Key Decisions

1. **FRAX + T-score dual stratification:** T-score alone is insufficient — the majority of hip and vertebral fractures occur in patients with T-score in the osteopenia range (> -2.5). FRAX integrates clinical risk factors (age, fracture history, corticosteroid use, etc.) and provides the full fracture probability picture. Both metrics are required in the constraint table.

2. **OWD > 5 cm as Muito Alto Risco trigger:** Occiput-to-wall distance is an accessible clinical proxy for vertebral compression fracture. Added as an alternative pathway to Muito Alto Risco classification alongside T-score + vertebral fracture history — provides a way to identify high-risk patients even when recent DXA is unavailable.

3. **Hip hinge as universal precaution:** Applied to ALL categories (not just Alto/Muito Alto Risco) because the biomechanical principle (spinal neutrality during loading) is protective regardless of fracture risk level. Introduced in Fase 1 before any resistance exercise.

4. **Exercise + bifosfonato sinergia as motivational tool:** BHOF/NOF 2022 confirms the synergistic effect. Explicitly documented in polypharmacy section as a communication point for the clinician — communicating this synergy to the patient is a direct aderência strategy.

5. **P-08 cross-reference (not re-derivation) for resistance dosing:** Consistent with the modifier chain architecture — P-04 sets the ceiling (fracture risk restrictions); P-08 sets the floor and parameters (frailty-stratified dosing). For osteosarcopenia patients, both apply simultaneously with P-04 taking precedence for the ceiling.

---

## Self-Check

**Files created/modified:**
- `C:/Projects/research/protocols/P-04-OSTEOPOROSE.md` — FOUND (1059 lines, created 2026-03-13)
- `C:/Projects/research/protocols/SHARED-FOUNDATION.md` — FOUND (P-04 row populated, 4 references)

**Commits:**
- `bdbc3c6` — FOUND (feat(02-02): create P-04-OSTEOPOROSE.md)
- `bea4c3d` — FOUND (feat(02-02): update SHARED-FOUNDATION cross-reference index with P-04 row)

## Self-Check: PASSED
