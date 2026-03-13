---
phase: 05-cluster-neuromotor
plan: "01"
subsystem: protocols
tags: [AVC, neuromotor, neuroplasticity, dual-task, aphasia, stroke, chronic]
dependency_graph:
  requires: []
  provides:
    - "protocols/P-03-AVC.md — complete chronic stroke rehabilitation protocol"
    - "TEMPLATE CLUSTER NEUROMOTOR — dual-task template referenced by P-06 and P-18"
    - "Aphasia/apraxia instruction adaptation subsystem — reusable across neuromotor cluster"
    - "SHARED-FOUNDATION.md P-03 row — cross-reference index entry"
  affects:
    - "P-06 (Parkinson) — TEMPLATE CLUSTER NEUROMOTOR via P-03 Seção 7.2"
    - "P-18 (Demência) — TEMPLATE CLUSTER NEUROMOTOR + aphasia adaptations via P-03 Seção 5.3"
    - "SHARED-FOUNDATION.md — Section 8.1 updated with P-03 row"
tech_stack:
  added: []
  patterns:
    - "Neuroplasticity-grounded phase progression (Kleim & Jones 2008 PMID 18230848)"
    - "TEMPLATE CLUSTER NEUROMOTOR — 4-level dual-task progressive difficulty table"
    - "Aphasia/apraxia instruction adaptation — 5-mode hierarchy (demonstration → verbal)"
    - "PAINAD-BR for non-verbal pain assessment in severe aphasia"
key_files:
  created:
    - protocols/P-03-AVC.md
  modified:
    - protocols/SHARED-FOUNDATION.md
decisions:
  - "[P-03]: AVC fase crônica escopo exclusivo (> 6 meses) — NÃO COBRE agudo/subagudo para evitar sobreposição com neurorreabilitação especializada"
  - "[P-03]: BBS-BR >= 40 + TUG < 20 como critérios de entrada para TEMPLATE CLUSTER NEUROMOTOR — fundamentados em segurança (risco de queda documentado fora desses limiares)"
  - "[P-03]: PAINAD-BR (PubMed 25993063) como instrumento primário quando NRS é inválida por afasia grave — único instrumento comportamental de dor validado em português brasileiro"
  - "[P-03]: Kleim & Jones (PMID 18230848) classificados como Nível C (mecanismo neurobiológico, não ECR) — valor reside na fundamentação teórica da progressão, não em evidência de intervenção"
  - "[P-03]: mCIMT (modified CIMT) adotado para geriatria — 3 horas/dia ao invés de 6 horas; 4 semanas semi-intensivas ao invés de 2 semanas intensivas"
  - "[P-03]: BWSTT (body-weight support treadmill) posicionado como opção adjuvante, não primeira linha — alinhado com VA/DoD 2024 (neither for nor against)"
metrics:
  duration_minutes: 8
  completed_date: "2026-03-13"
  tasks_completed: 2
  files_created: 1
  files_modified: 1
---

# Phase 5 Plan 01: AVC Fase Crônica — P-03-AVC.md Summary

**One-liner:** Protocolo completo de AVC crônico com fundação neuroplástica Kleim-Jones, template de dupla tarefa reutilizável (TEMPLATE CLUSTER NEUROMOTOR), subsistema de adaptação de instrução para afasia/apraxia e PAINAD-BR para avaliação de dor não-verbal.

---

## What Was Built

**P-03-AVC.md** (1147 lines, 15 sections, TIDieR/CERT compliant, Brazilian Portuguese):

- **Section 1:** Temporal scope declaration (> 6 meses, fase crônica exclusivamente) with full NÃO COBRE block
- **Section 2:** Complete assessment battery — 9 instruments including BBS-BR, FES-I-BR, MoCA-BR, Ashworth Modificada, FMA-MMII, avaliação de afasia e apraxia
- **Sections 4–7:** Three-phase structure with neuroplasticity principle declarations per phase, function-based transition criteria (never time-only), two-column dosage tables × 3 frailty rows
- **Section 5.3:** Aphasia/Apraxia Instruction Adaptation Subsystem — 4 patient profiles (A–D), 5-mode instruction hierarchy (physical demonstration as primary), hand-over-hand guidance, visual feedback, single-keyword verbal reduction
- **Section 7.2:** TEMPLATE CLUSTER NEUROMOTOR — formal reusable dual-task training template with: Cochrane-level evidence (PMC12261537, 30 RCTs), BBS-BR ≥ 40 + TUG < 20 entry criteria, 4-level DT table (DT-1 to DT-4), dosage table with 3 frailty rows, aphasia adaptation (verbal → visual task substitution)
- **Section 8.2:** PAINAD-BR (PubMed 25993063) — 5-domain behavioral pain table with action thresholds (0–2 continue, 3–5 reduce 25%, ≥ 6 suspend)
- **Section 13:** Full cross-protocol modifier chain — P-07 Seção 5.2, P-07 Seção 7.2, P-08 Seção 6.3, P-04 Seção 5.2 — all with priority ordering
- **Section 15:** All 8 clinical validity questions answered

**SHARED-FOUNDATION.md Section 8.1** updated with complete P-03 row (11 protocol interactions, key features, scope note, assessment instruments, primary guidelines, safety alerts).

---

## Commits

| Task | Name | Commit | Files |
|------|------|--------|-------|
| 1 | Create P-03-AVC.md | bccfa72 | protocols/P-03-AVC.md (created, 1147 lines) |
| 2 | Update SHARED-FOUNDATION P-03 row | a8cc0c1 | protocols/SHARED-FOUNDATION.md (modified) |

---

## Decisions Made

1. **Scope**: AVC fase crônica (> 6 meses) is the exclusive scope. Acute/subacute AVC are redirected to specialized neurorehabiliation — prevents content overlap and scope confusion.

2. **TEMPLATE entry criteria**: BBS-BR ≥ 40 + TUG < 20 + 2 sessions without balance events. These thresholds are evidence-based safety gates: literature documents increased fall risk during dual-task training below BBS-BR 40.

3. **PAINAD-BR**: Positioned as primary (not secondary) instrument when aphasia makes NRS unreliable. NRS is inherently verbal — applying it to patients who cannot reliably quantify pain is a measurement error, not a limitation.

4. **Kleim & Jones evidence classification**: Classified as Level C (mechanistic, not RCT). The value is theoretical coherence for phase progression — individual interventions maintain their own evidence annotations independently.

5. **mCIMT for geriatric population**: Standard CIMT (6h/day, 2 weeks) is physiologically unsuitable for frail elderly. mCIMT (3h/day, 4 weeks) preserves efficacy while accommodating frailty and safety constraints.

6. **BWSTT positioning**: VA/DoD 2024 "neither for nor against" — this is an honest evidence annotation. BWSTT is positioned as adjuvant option, not first-line, to avoid over-prescribing a resource-intensive intervention without strong directional evidence.

---

## Deviations from Plan

None — plan executed exactly as written.

---

## Cluster Assets Created

Three reusable assets established in P-03 for the neuromotor cluster (P-06 Parkinson, P-18 Demência):

1. **TEMPLATE CLUSTER NEUROMOTOR** (P-03 Seção 7.2) — P-06 and P-18 reference by name, never re-derive
2. **Aphasia/Apraxia Instruction Subsystem** (P-03 Seção 5.3) — P-18 (Demência) will reference for cognitively impaired patients
3. **Neuroplasticity theoretical foundation** (P-03 Seção 4.2) — contextual reference for all three neuromotor protocols

---

## Self-Check: PASSED

| Item | Status |
|------|--------|
| protocols/P-03-AVC.md | FOUND (1147 lines) |
| protocols/SHARED-FOUNDATION.md (modified) | FOUND |
| .planning/phases/05-cluster-neuromotor/05-01-SUMMARY.md | FOUND |
| Commit bccfa72 (Task 1) | FOUND |
| Commit a8cc0c1 (Task 2) | FOUND |
