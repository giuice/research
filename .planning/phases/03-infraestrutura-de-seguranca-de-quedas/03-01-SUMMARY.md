---
phase: 03-infraestrutura-de-seguranca-de-quedas
plan: "01"
subsystem: falls-prevention-protocol
tags: [quedas, sindrome-pos-queda, hierarquia-de-equilibrio, protocolo-de-sessao, FES-I-BR, BBS-BR, TSK-11-BR, infraestrutura-de-seguranca, modificador-transversal]
dependency_graph:
  requires: [protocols/SHARED-FOUNDATION.md, protocols/P-08-SARCOPENIA.md, protocols/P-04-OSTEOPOROSE.md]
  provides: [protocols/P-07-QUEDAS.md]
  affects: [protocols/SHARED-FOUNDATION.md, all neuromotor and frailty protocols Phases 4-8 — balance hierarchy + session safety reference]
tech_stack:
  added: []
  patterns:
    - "4-level balance intervention hierarchy (static/dynamic/dual-task/perturbation) with TUG/SPPB/BBS entry and exit criteria — normative reference for Phases 4-8"
    - "Session-level fall risk protocol with 4 operational elements: VAS fatigue, orthostatic BP check, TUG-anchored gait belt, supervised exit — reusable template"
    - "Post-fall syndrome full triad: medo de cair (FES-I-BR ≥ 23) + restricao de atividade + perda funcional progressiva"
    - "FES-I-BR (Camargos 2010) cutoffs ≥23/≥31 for sporadic/recurrent fall history"
    - "Perturbation-based training (PBT) eligible for frail patients with harness + pre-test safeguards — not excluded categorically"
    - "INFRAESTRUTURA DE SEGURANÇA label pattern for cross-protocol modifier blocks (consistent with MODIFICADOR TRANSVERSAL in P-04)"
    - "Modifier chain: P-04 bone ceiling (priority 1) → P-08 resistance params (priority 2) → P-07 balance progression + session safety (normative, Phases 4-8)"
key_files:
  created:
    - protocols/P-07-QUEDAS.md
  modified:
    - protocols/SHARED-FOUNDATION.md
decisions:
  - "[03-01]: INFRAESTRUTURA DE SEGURANÇA label pattern adopted for both P-07 modifier sections — consistent with MODIFICADOR TRANSVERSAL pattern from P-04 but differentiated by function (safety infrastructure vs. constraint table)"
  - "[03-01]: Balance hierarchy 4-level table with objective TUG/SPPB/BBS entry/exit criteria — normative reference for all neuromotor/frailty protocols (P-03, P-05, P-06, P-08, P-10, P-11, P-18)"
  - "[03-01]: PBT eligible for frail patients WITH safeguards (harness + pre-test) — PMC10587291 feasibility confirms 61% frail participants, zero adverse events"
  - "[03-01]: Post-fall syndrome defined as full triad (fear + activity restriction + progressive functional loss) — not synonymous with fear of falling"
  - "[03-01]: STOPPFall escalation threshold: ≥4 psicoactive medications OR benzodiazepine + opioid + anti-hypertensive combination"
metrics:
  duration_minutes: 10
  completed_date: "2026-03-13"
  tasks_completed: 2
  tasks_total: 2
  files_created: 1
  files_modified: 1
  lines_written: 990
requirements_satisfied: [PROT-04]
---

# Phase 3 Plan 01: P-07 Quedas e Sindrome Pos-Queda Summary

**One-liner:** Complete falls prevention and post-fall syndrome rehabilitation protocol with dual cross-protocol infrastructure role: 4-level balance intervention hierarchy with objective TUG/SPPB/BBS entry criteria (normative reference for Phases 4-8) and session-level fall risk protocol with 4 operational safety elements (reusable template for all fall-risk patient protocols).

---

## What Was Built

### Task 1: P-07-QUEDAS.md (990 lines)

Created a complete 15-section geriatric rehabilitation protocol for falls and post-fall syndrome in Brazilian Portuguese, TIDieR/CERT compliant, with:

**Section 1 — Criterios Diagnosticos e de Inclusao:**
- WHO fall definition (involuntary event resulting in resting on ground or lower level)
- Post-fall syndrome defined as FULL TRIAD: medo de cair (FES-I-BR ≥ 23) + restricao de atividade (avoidance behavior) + perda funcional progressiva (TUG deterioration, SPPB decline) — NOT just "fear of falling"
- 6 inclusion criteria: ≥ 1 fall in 12 months, TUG > 13.5 sec, SPPB ≤ 9, FES-I-BR ≥ 23, BBS-BR < 45, self-reported fear
- 5 exclusion criteria with justification and clinical action

**Section 2 — Avaliacao Inicial Mandatoria:**
- TUG + SPPB-BR + Dinamometria Manual (inherited SHARED-FOUNDATION)
- BBS-BR (Miyamoto 2004, PubMed 15334208): 14 items, 0-56 pts; fall risk cutoff < 45; MCID 3.3 pts (Donoghue 2009; Brazilian-specific MCID annotated as unconfirmed)
- FES-I-BR (Camargos 2010, PubMed 20730369): 16 items, 16-64 pts; cutoffs ≥ 23/≥ 31; Cronbach α = 0.93; ICC inter = 0.91; MCID 3 pts (clinical estimate, annotated)
- TSK-11-BR (Salvador 2020, PMC7990729): 11 items, 11-44 pts; Cronbach α = 0.77; ICC = 0.85; cutoff > 37 with population annotation (chronic pain origin — verify in geriatric falls)
- Combined FES-I-BR + TSK-11-BR decision table with 5 clinical action profiles

**Section 5.2 — INFRAESTRUTURA DE SEGURANCA — PROTOCOLO DE RISCO DE QUEDA POR SESSAO:**
- Labeled as reusable template with verbatim citation format for Phases 4-8
- Element 1: VAS fadiga pre-sessao (≤4 proceed / 5-7 reduce 30% no perturbation / ≥8 defer) — annotated as clinical consensus
- Element 2: Orthostatic BP check (supine 5 min → stand 1 + 3 min; systolic ≥20 OR diastolic ≥10 mmHg threshold; cites PMC10024337)
- Element 3: TUG-anchored gait belt criteria table (≤10 optional / 10.1-13.5 recommended / 13.6-20 mandatory+therapist / >20 mandatory+parallel bars)
- Element 4: Supervised exit protocol (5 min seated cooldown, dizziness check, assisted stand, 2 min standing wait, non-release criteria, mandatory documentation)

**Section 7.2 — INFRAESTRUTURA DE SEGURANCA — HIERARQUIA DE INTERVENCAO DE EQUILIBRIO:**
- Labeled as normative cross-protocol reference naming downstream protocols P-03, P-05, P-06, P-08, P-10, P-11, P-18 with citation format
- 4-level table: Estatico / Dinamico / Dupla Tarefa / Perturbacao
- Each level: TUG/SPPB/BBS numerical entry criteria, exit criteria, typical dosage, frailty note
- Frailty override: Fragil (Fried ≥ 3) always starts Level 1 regardless of TUG
- Frail patients eligible for Level 4 (perturbation) WITH safeguards — not excluded

**Section 15 — As 8 Questoes de Validade Clinica:**
- All 8 questions answered with section cross-references (Q1-Q8)
- Q8 explains evidence rationale for each key architectural choice

### Task 2: SHARED-FOUNDATION.md — P-07 Row

Updated Section 8.1 cross-reference matrix:
- 10 comorbidity interactions: P-08, P-04, P-01, P-05, P-06, P-03, P-10, P-11, P-18, P-17
- Both cross-protocol modifiers documented with citation formats
- Modifier chain priority documented: P-04 (priority 1) → P-08 (priority 2) → P-07 (normative, Phases 4-8)
- Specific precautions: triad assessment, FES-I-BR ≥ 31 escalation, STOPPFall criteria

---

## Verification Results

All 14 verification criteria from the plan confirmed:

| # | Criterion | Status |
|---|-----------|--------|
| 1 | P-07-QUEDAS.md exists with ≥ 15 sections and ≥ 900 lines | PASS — 15 sections, 990 lines |
| 2 | INFRAESTRUTURA DE SEGURANÇA label present for both modifier sections | PASS — 4 occurrences (2 for each modifier block) |
| 3 | Balance hierarchy table has 4 levels with numerical entry criteria | PASS — 4 levels, each with TUG/SPPB/BBS values |
| 4 | Session fall risk protocol has 4 operational elements in decision-table format | PASS — 4 elements with thresholds |
| 5 | FES-I-BR with Camargos 2010 (PubMed 20730369), cutoffs ≥23 and ≥31 | PASS — 4 PubMed occurrences, both cutoffs |
| 6 | BBS-BR with Miyamoto 2004 (PubMed 15334208), fall risk cutoff < 45 | PASS — 3 PubMed occurrences |
| 7 | TSK-11-BR with Salvador 2020 (PMC7990729), cutoff > 37 with annotation | PASS — 2 PMC occurrences + annotation |
| 8 | Post-fall syndrome defined as triad | PASS — 4 occurrences of triad definition |
| 9 | Two-column dosage tables with 3 frailty rows | PASS — 6 tables (one per intervention phase) |
| 10 | Section 15 answers all 8 clinical validity questions | PASS — Q1 through Q8 |
| 11 | SHARED-FOUNDATION.md P-07 row ≥ 10 comorbidity interactions | PASS — 10 interactions |
| 12 | Entire document in Brazilian Portuguese | PASS — 76+ Portuguese clinical terms confirmed |
| 13 | Perturbation training includes frail patients with safeguards | PASS — 8 occurrences (arnês, 61%, frágil elegível) |
| 14 | Cross-protocol modifier labels name downstream protocols and citation format | PASS — 2 occurrences naming P-03, P-05, P-06, P-08, P-10, P-11, P-18 |

Automated term counts: FES-I-BR: 43; BBS-BR: 17; TSK-11-BR: 13; Camargos: 5; Miyamoto: 5; Salvador: 2; PubMed: 24; Secao/Seção: 49.

---

## Commits

| Task | Commit | Message |
|------|--------|---------|
| 1 | 6d94af4 | feat(03-01): create P-07-QUEDAS.md — complete 15-section geriatric rehabilitation protocol |
| 2 | ea25a9c | feat(03-01): update SHARED-FOUNDATION cross-reference index with P-07 row |

---

## Deviations from Plan

None — plan executed exactly as written.

The plan specified the session fall risk protocol in Fase 1 (Section 5) — placed precisely in Section 5.2 as a labeled INFRAESTRUTURA DE SEGURANÇA blockquote with all 4 elements. The balance hierarchy was placed in Fase 3 (Section 7) as Section 7.2 with the INFRAESTRUTURA DE SEGURANÇA label naming downstream protocols. Both citation formats were implemented as specified. The STOPPFall reference was included in Section 10 (Polypharmacy) with the O'Mahony 2021 citation. All required annotations were included: VAS fatigue thresholds (clinical consensus), TSK-11-BR cutoff population note, BBS-BR MCID annotation, and manual perturbation alternative annotation.

---

## Key Decisions

1. **INFRAESTRUTURA DE SEGURANÇA label pattern:** Adopted the same blockquote modifier label pattern established by MODIFICADOR TRANSVERSAL in P-04, but named distinctly as INFRAESTRUTURA DE SEGURANÇA to reflect the safety infrastructure function (not a constraint table). Two separate labeled blocks — one for the session protocol (Section 5.2) and one for the balance hierarchy (Section 7.2).

2. **Frail patients eligible for PBT (perturbation training):** PMC10587291 feasibility pilot included 61% frail participants without adverse events when arnês + pre-test protocol was applied. Excluding frail patients from PBT would be unsupported by evidence and would deny them the most effective fall rate reduction intervention (23% reduction per meta-analysis). The plan explicitly required inclusion with safeguards — implemented with full safety protocol specification.

3. **TSK-11-BR population annotation:** The cutoff > 37 was derived from chronic pain populations, not geriatric falls. This annotation was made explicit in Section 2.4 per plan instructions. This is honest evidence annotation consistent with the series standard.

4. **BBS-BR as primary balance outcome (not Escala de Tinetti):** Deliberate exclusion of Tinetti scale per plan anti-patterns. BBS-BR has the validated Brazilian version with published cutoffs (< 45 for fall risk) and provides the objective anchor for the balance hierarchy table — which is the structural reason it was chosen.

5. **STOPPFall escalation threshold operationalized:** ≥ 4 psicoactive medications OR combination benzodiazepine + opioid + anti-hypertensive. This makes the referral recommendation actionable rather than generic.

---

## Self-Check

**Files created/modified:**
- `C:/Projects/research/protocols/P-07-QUEDAS.md` — FOUND (990 lines, created 2026-03-13)
- `C:/Projects/research/protocols/SHARED-FOUNDATION.md` — FOUND (P-07 row populated, 10 interactions)
- `C:/Projects/research/.planning/phases/03-infraestrutura-de-seguranca-de-quedas/03-01-SUMMARY.md` — FOUND

**Commits:**
- `6d94af4` — FOUND (feat(03-01): create P-07-QUEDAS.md)
- `ea25a9c` — FOUND (feat(03-01): update SHARED-FOUNDATION cross-reference index with P-07 row)

## Self-Check: PASSED
