---
phase: 04-musculoesqueletico-alta-dependencia
plan: "01"
subsystem: hip-fracture-protocol
tags: [fratura-femur, CFS, TEV, mobilizacao-precoce, modificador-transversal, equilibrio, P-07-comodificador]
dependency_graph:
  requires: [protocols/SHARED-FOUNDATION.md, protocols/P-04-OSTEOPOROSE.md, protocols/P-08-SARCOPENIA.md, protocols/P-07-QUEDAS.md, protocols/P-01-OSTEOARTRITE.md]
  provides: [protocols/P-05-FRATURA-FEMUR.md]
  affects: [protocols/SHARED-FOUNDATION.md, all Phase 4+ protocols — CFS+TEV+fall-risk integration pattern]
tech_stack:
  added: []
  patterns:
    - "CFS (Clinical Frailty Scale) mandatory at admission with mortality prediction (PubMed 33215137) — CFS 1-3 Robusto, 4-5 Pre-fragil, 6-7 Fragil, 8 paliativo conjunto, 9 fora do escopo"
    - "TEV awareness section declaring physiotherapy scope of practice — no anticoagulant prescription"
    - "First protocol to consume ALL three cross-protocol modifiers simultaneously (P-04 bone-loading, P-08 resistance dosing, P-07 balance/session safety)"
    - "FES-I-BR >= 23 triggers mandatory P-07 co-modifier activation for post-fracture fall prevention"
    - "Two-column dosage tables with 3 frailty rows in all phase sections"
    - "Function-based phase progression with temporal safety minimums (not time-only)"
key_files:
  created:
    - protocols/P-05-FRATURA-FEMUR.md
  modified:
    - protocols/SHARED-FOUNDATION.md
decisions:
  - "[04-01]: CFS mandatório na admissão de P-05 — superioridade discriminativa vs ASA e idade para mortalidade pós-fratura (PubMed 33215137)"
  - "[04-01]: TEV awareness section declara escopo de prática (não prescreve anticoagulante) — tabela de implicações por agente (LMWH, DOACs, aspirina, warfarina)"
  - "[04-01]: P-07 como comodificador obrigatório sempre (risco intrínseco de queda pós-fratura) — FES-I-BR >= 23 ativa hierarquia de equilíbrio como componente estrutural"
  - "[04-01]: Cargas de Fase 2 ligeiramente abaixo de P-08 Seção 6.3 baseline (50% vs 65% 1RM para Robusto) para acomodar fragilidade pós-fratura"
  - "[04-01]: WBAT como padrão quando cirurgicamente liberado — P-05 não especifica carga por tipo de implante sem orientação cirúrgica"
metrics:
  completed_date: "2026-03-13"
  tasks_completed: 2
  tasks_total: 2
  files_created: 1
  files_modified: 1
  lines_written: 905
requirements_satisfied: [PROT-05]
---

# Phase 4 Plan 01: P-05 Fratura de Fêmur Proximal Summary

**One-liner:** Complete proximal femur fracture rehabilitation protocol with CFS mandatory at admission, TEV awareness within physiotherapy scope, and first protocol to consume all three cross-protocol modifiers (P-04 bone-loading, P-08 resistance dosing, P-07 balance/session safety) — establishing the integration pattern for P-10 and P-11.

---

## What Was Built

### Task 1: P-05-FRATURA-FEMUR.md (905 lines)

Created a complete 15-section geriatric rehabilitation protocol for proximal femur fracture in Brazilian Portuguese, TIDieR/CERT compliant, with:

**Section 1 — Critérios Diagnósticos e de Inclusão:**
- Fracture classification: intracapsular (subcapital, transcervical) vs extracapsular (intertrocantérica, subtrocantérica)
- Surgical fixation types with clinical implications for weight-bearing
- Inclusion: age >= 60, post-surgical fixation, CFS <= 8
- Exclusion: pathological fracture, periprosthetic, polytrauma, CFS 9
- Scope declaration distinguishing P-05 from P-11 (elective THA)

**Section 2 — Avaliação Inicial Mandatória:**
- TUG + SPPB-BR + Dinamometria (inherited SHARED-FOUNDATION)
- CFS (Rockwood 2005) MANDATORY at admission with mortality data and CFS-to-frailty tier mapping
- BBS-BR (Miyamoto 2004) mandatory — high fall risk population
- FES-I-BR (Camargos 2010) mandatory — post-fracture fear of falling screening
- MoCA-BR for delirium/dementia screening (35-65% incidence post-hip-fracture)
- Weight-bearing status documentation protocol

**Section 5 — Fase 1 (Aguda/Protegida):**
- Mobilization < 48h post-op (AAOS 2021) with day-by-day protocol
- WBAT as default when surgically cleared
- Bed exercises, transfers, gait training with dosage tables
- Static balance (P-07 Seção 7.2 Level 1)
- Session safety protocol (P-07 Seção 5.2)

**Section 10.3 — TEV Awareness:**
- Scope of practice declaration — no anticoagulant prescription
- Anticoagulant implication table (LMWH, DOACs, Aspirina, Warfarina)
- Early mobilization as mechanical VTE prophylaxis

**Section 13 — Rastreabilidade:**
- P-04 Seção 5.2 cited for bone-loading (always applicable)
- P-08 Seção 6.3 cited for resistance dosing (Phase 2+)
- P-07 Seções 5.2 and 7.2 cited as mandatory co-modifier
- FES-I-BR >= 23 activation flag for P-07

### Task 2: SHARED-FOUNDATION.md — P-05 Row

Updated Section 8.1 with P-05 row: 8 comorbidity interactions, CFS admission requirement, three modifier references, TEV awareness scope.

---

## Commits

| Task | Commit | Message |
|------|--------|---------|
| 1 | 0bc4cfd | feat(04-01): create P-05-FRATURA-FEMUR.md — complete 15-section geriatric rehabilitation protocol |
| 2 | 4b970c6 | feat(04-01): update SHARED-FOUNDATION cross-reference index with P-05 row |

---

## Deviations from Plan

None — plan executed as written. All 14 verification criteria satisfied.

---

## Self-Check

**Files created/modified:**
- `protocols/P-05-FRATURA-FEMUR.md` — FOUND (905 lines)
- `protocols/SHARED-FOUNDATION.md` — FOUND (P-05 row populated, 8 interactions)

**Commits:**
- `0bc4cfd` — FOUND
- `4b970c6` — FOUND

## Self-Check: PASSED
