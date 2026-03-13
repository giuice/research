---
phase: 04-musculoesqueletico-alta-dependencia
plan: "02"
subsystem: arthroplasty-protocols
tags: [ATJ, ATQ, artroplastia-joelho, artroplastia-quadril, sindrome-compartimental, luxacao-protetica, precaucoes-abordagem, modificador-transversal, WOMAC-BR, diferenciacao-de-escopo]
dependency_graph:
  requires: [protocols/SHARED-FOUNDATION.md, protocols/P-04-OSTEOPOROSE.md, protocols/P-08-SARCOPENIA.md, protocols/P-07-QUEDAS.md, protocols/P-05-FRATURA-FEMUR.md, protocols/P-01-OSTEOARTRITE.md]
  provides: [protocols/P-10-ATJ.md, protocols/P-11-ATQ.md]
  affects: [protocols/SHARED-FOUNDATION.md, all Phase 4+ protocols — ATJ/ATQ cross-reference pattern]
tech_stack:
  added: []
  patterns:
    - "Scope differentiation analysis before drafting — each protocol opens with explicit NÃO COBRE block listing what it does not cover and referencing the other protocol"
    - "P-10: compartment syndrome vigilance (5 Ps) as specific red flag with epidural masking warning (PubMed 16498006) — 2+ signs = orthopedic emergency"
    - "P-11: approach-specific precaution subsets (Posterior / Anterior Direto / Anterolateral) — mandatory surgical approach verification before any ROM exercise"
    - "P-11: declared policy on posterior approach precautions — follow surgeon orientation; 2024 meta-analysis evidence (PMC11651519) presented but no auto-relaxation at 6 weeks"
    - "Both protocols: function-based phase progression with temporal minimums (not time-only) — consistent with DOSE-04 and SHARED-FOUNDATION Seção 3"
    - "Both protocols: WOMAC-BR (Oliveira 2022, PMC9673866) as primary functional outcome — pre-existing registry in SHARED-FOUNDATION Seção 6.2"
    - "Both protocols: P-04 Seção 5.2 + P-08 Seção 6.3 + P-07 Seções 5.2/7.2 cited by section number — zero re-derivation of modifier knowledge"
key_files:
  created:
    - protocols/P-10-ATJ.md
    - protocols/P-11-ATQ.md
  modified:
    - protocols/SHARED-FOUNDATION.md
decisions:
  - "[04-02]: Scope differentiation analysis performed before drafting — explicit NÃO COBRE blocks prevent content overlap between P-10 and P-11"
  - "[04-02]: P-11 adopts declared policy on posterior approach precautions — 2024 meta-analysis (PMC11651519) evidence of non-inferiority without restrictions presented; conduta follows surgeon orientation with classical precautions as default in absence of specific instruction"
  - "[04-02]: Precautions in P-11 NOT relaxed automatically at 6 weeks — require documented surgical clearance; Trendelenburg elimination as functional target not gated by time"
  - "[04-02]: WOMAC-BR as primary functional outcome for both P-10 and P-11 — consistent with SHARED-FOUNDATION Seção 6.2 registry; KOOS-BR excluded due to absence of confirmed Brazilian validation"
  - "[04-02]: P-10 lag de quadriceps (quad lag) included as specific ATJ assessment — incapacity to achieve final 15° of active extension against gravity is functional predictor"
  - "[04-02]: P-11 anterolateral approach monitoring: glúteo médio (superior gluteal nerve at risk) — force assessment mandatory at admission, Trendelenburg > 12 weeks = nerve injury red flag"
metrics:
  completed_date: "2026-03-13"
  tasks_completed: 2
  tasks_total: 2
  files_created: 2
  files_modified: 1
  lines_written: 1900
requirements_satisfied: [PROT-06, PROT-07]
---

# Phase 4 Plan 02: P-10 ATJ and P-11 ATQ Summary

**One-liner:** Explicitly differentiated post-arthroplasty rehabilitation protocols — P-10 for TKA (compartment syndrome vigilance, quadriceps lag monitoring, ROM milestones) and P-11 for THA (approach-specific dislocation precautions with 2024 meta-analysis evidence, abductor rehabilitation, Trendelenburg elimination) — both consuming all three cross-protocol modifiers and completing the Phase 4 high-dependency musculoskeletal cluster.

---

## What Was Built

### Task 1: P-10-ATJ.md (922 lines) and P-11-ATQ.md (978 lines)

Created two complete 15-section geriatric rehabilitation protocols in Brazilian Portuguese, TIDieR/CERT compliant, with full scope differentiation analysis performed before drafting.

**Pre-Drafting Differentiation Analysis:**

| Dimension | P-10 (ATJ) | P-11 (ATQ) |
|-----------|-----------|-----------|
| Joint | Joelho (knee) | Quadril (hip) |
| Primary risk | Rigidez + síndrome compartimental + lag de quadríceps | Luxação protética (abordagem-dependente) + déficit de abdutores |
| Specific assessment | ROM joelho (flexão/extensão) + lag de quadríceps | Abordagem cirúrgica + força de abdução + Trendelenburg |
| Specific red flag | Síndrome compartimental (5 Ps + mascaramento epidural) | Luxação (dor aguda + rotação interna + discrepância + incapacidade) |
| Section 5 key feature | Crioterapia + ativação de quadríceps + mobilização patelar | Precauções por abordagem (3 subseções) + ativação de abdutores |
| Outcome | WOMAC-BR + ROM joelho + lag de quadríceps | WOMAC-BR + força abdução + Trendelenburg |

**P-10 ATJ — Key Architectural Features:**

**Section 1 — Critérios Diagnósticos e de Inclusão:**
- OA grau III-IV + indicação cirúrgica + estado pós-op
- Scope block: cobre ATJ primária; NÃO cobre ATQ (P-11), fratura periprotética, revisão de ATJ
- Inclusion: age ≥ 60, post-primary TKA, admitted to rehabilitation

**Section 2 — Avaliação Inicial Mandatória:**
- TUG + SPPB-BR + Dinamometria (inherited SHARED-FOUNDATION)
- ROM ativo de joelho: flexão (meta ≥ 90° por 6 semanas / ≥ 120° por 12 semanas) + extensão (meta 0°)
- Lag de quadríceps: incapacidade de extensão ativa dos últimos 15° contra gravidade
- BBS-BR + FES-I-BR (pós-artroplastia fall risk)
- WOMAC-BR (Oliveira 2022, PMC9673866) — primary functional outcome

**Section 9 — Bandeiras Vermelhas (P-10 Specific):**
- 5 Ps de síndrome compartimental: Pain (dorsiflexão passiva de tornozelo), Pressure, Pallor, Paresthesia, Paralysis
- Alert: bloqueio epidural pode mascarar sinal de dor — monitorar os outros 4 Ps mesmo sem dor relatada (PubMed 16498006: 5 de 7 casos com atraso diagnóstico)
- Rule: 2+ sinais = suspender + ortopedia de urgência IMEDIATAMENTE
- Artrofibrose: flexão < 70° aos 6 semanas = encaminhar ortopedia

**P-11 ATQ — Key Architectural Features:**

**Section 1 — Critérios Diagnósticos e de Inclusão:**
- Coxartrose terminal + indicação cirúrgica + estado pós-op
- Scope block: cobre ATQ primária; NÃO cobre ATJ (P-10), hemiartroplastia por fratura (P-05), fratura periprotética, revisão de ATQ
- Mandatory: document surgical approach BEFORE starting rehabilitation

**Section 2 — Avaliação Inicial Mandatória:**
- TUG + SPPB-BR + Dinamometria (inherited SHARED-FOUNDATION)
- ROM ativo de quadril: flexão, extensão, abdução, rotação — per approach restrictions
- Força de abdução (dinamometria ou MMT) + Sinal de Trendelenburg + Discrepância de comprimento
- BBS-BR + FES-I-BR + WOMAC-BR

**Section 5 — Fase 1 — Precauções de Luxação por Abordagem:**

Three explicitly differentiated subsections:

*Abordagem Posterior:*
- Classical precautions (flexion > 90°, adduction, internal rotation) + 2024 meta-analysis evidence (PMC11651519: 1,215 patients, no significant difference in dislocation rate with/without precautions)
- Declared policy: follow surgeon orientation; maintain classical precautions as default in absence of specific instruction; do NOT auto-relax at 6 weeks

*Abordagem Anterior Direta:*
- Avoid extension beyond neutral, excessive external rotation, prone sleeping
- Lower posterior dislocation risk documented; functional benefit (less ROM restriction) noted

*Abordagem Anterolateral:*
- Minimal precautions; monitor abductor deficit (superior gluteal nerve at risk)
- Mandatory force assessment at admission; Trendelenburg > 12 weeks = possible nerve injury

**Section 9 — Bandeiras Vermelhas (P-11 Specific):**
- Luxação protética: dor aguda + rotação interna involuntária + discrepância + incapacidade de carga → EMERGÊNCIA; imobilizar na posição encontrada, NÃO tentar reduzir
- Fratura periprotética: dor súbita em coxa + impossibilidade de carga → urgência
- Trendelenburg > 12 semanas: possível lesão de nervo glúteo superior → EMG/VCN

**Both Protocols — Shared Features:**

- Function-based phase progression with temporal minimums (not time-only)
- Two-column dosage tables with 3 frailty rows (Robusto/Pré-frágil/Frágil) in all phase sections
- Section 13 (Rastreabilidade) populated by cross-reference — zero re-derivation:
  - P-04 Seção 5.2 (bone-loading constraints — when T-score ≤ -2.5)
  - P-08 Seção 6.3 (resistance dosing — in sarcopenia)
  - P-07 Seções 5.2 and 7.2 (session protocol + balance hierarchy — all Fase 1 patients)
- All 8 clinical validity questions answered in Section 15
- Section 10: anticoagulant TEV awareness with scope-of-practice declaration (physiotherapy does NOT prescribe anticoagulants)
- STOPPFall referenced for polypharmacy screening

### Task 2: SHARED-FOUNDATION.md — P-10 and P-11 Rows

Updated Section 8.1 cross-reference matrix with:

**P-10 row:**
- 8 comorbidity interactions: P-01, P-04, P-08, P-07, P-05, P-11, P-06, P-18
- Specific precautions: compartment syndrome 5 Ps (PubMed 16498006); ROM targets; quadriceps lag
- Scope note: ATJ only — differentiated from P-11 (ATQ)

**P-11 row:**
- 8 comorbidity interactions: P-01, P-04, P-08, P-07, P-05, P-10, P-06, P-18
- Specific precautions: approach-specific dislocation precautions (PMC11651519); abductor deficit; limb length discrepancy
- Scope note: ATQ only — differentiated from P-10 (ATJ) and P-05 (hemiartroplastia)

---

## Commits

| Task | Commit | Message |
|------|--------|---------|
| 1 | f204aa7 | feat(04-02): create P-10-ATJ.md and P-11-ATQ.md — complete post-arthroplasty rehabilitation protocols |
| 2 | 23965be | feat(04-02): update SHARED-FOUNDATION cross-reference index with P-10 and P-11 rows |

---

## Deviations from Plan

None — plan executed as written. All 15 verification criteria satisfied.

The differentiation analysis (Step 0) was performed as a conceptual step before drafting, as planned. The approach-specific precaution subsets for P-11 (3 subsections: Posterior, Anterior Direta, Anterolateral) match exactly the Code Examples from the research document. The compartment syndrome 5 Ps format in P-10 matches the Code Example from the research document. All anti-patterns from the research document were avoided.

---

## Self-Check

**Files created/modified:**
- `protocols/P-10-ATJ.md` — FOUND (922 lines, 15 sections)
- `protocols/P-11-ATQ.md` — FOUND (978 lines, 15 sections)
- `protocols/SHARED-FOUNDATION.md` — FOUND (P-10 row: 8 interactions; P-11 row: 8 interactions)

**Commits:**
- `f204aa7` — FOUND
- `23965be` — FOUND

**Verification criteria (plan checklist — all 15 passed):**
1. P-10-ATJ.md ≥ 15 sections + ≥ 900 lines — PASS (922 lines, 15 sections)
2. P-11-ATQ.md ≥ 15 sections + ≥ 900 lines — PASS (978 lines, 15 sections)
3. Scope statements referencing each other — PASS (both have NÃO COBRE blocks with P-11/P-10 references)
4. P-10 Section 9: compartment syndrome + PubMed 16498006 — PASS (4 occurrences of 16498006)
5. P-11 approach-specific precautions with PMC11651519 — PASS (3 occurrences of PMC11651519)
6. P-11 surgeon verification instruction before ROM exercises — PASS (mandatory instruction in Seção 5.2 header)
7. Both: P-04 Seção 5.2 in Section 13 — PASS (P-10: 12 refs; P-11: 13 refs)
8. Both: P-08 Seção 6.3 in Section 13 — PASS (P-10: 9 refs; P-11: 9 refs)
9. Both: P-07 Seções 5.2 and 7.2 in Section 13 — PASS (P-07 appears 22 times in each)
10. Function-based phase progression — PASS (all exit criteria use functional measures + temporal minimums)
11. WOMAC-BR (Oliveira 2022, PMC9673866) as primary outcome — PASS (11 refs P-10; 12 refs P-11)
12. Two-column dosage tables with 3 frailty rows — PASS (all phase exercise tables present)
13. Section 15 — 8 clinical validity questions — PASS (Q1–Q8 in both)
14. SHARED-FOUNDATION P-10 and P-11 rows with ≥ 8 comorbidity interactions — PASS (8 each)
15. Both documents entirely in Brazilian Portuguese — PASS

## Self-Check: PASSED
