---
phase: 02-modificadores-transversais
plan: "01"
subsystem: sarcopenia-protocol
tags: [sarcopenia, EWGSOP2, exercicio-resistido, modificador-transversal, polifarmacia, proteina-exercicio]
dependency_graph:
  requires: [protocols/SHARED-FOUNDATION.md, protocols/P-01-OSTEOARTRITE.md]
  provides: [protocols/P-08-SARCOPENIA.md]
  affects: [protocols/SHARED-FOUNDATION.md, all 20 protocols — resistance dosing modifier]
tech_stack:
  added: []
  patterns:
    - "EWGSOP2 FACS 4-step diagnostic algorithm (Find-Assess-Confirm-Severity)"
    - "Frailty-stratified resistance dosing modifier table (MODIFICADOR TRANSVERSAL)"
    - "Protein-exercise coordination subsection with 5-criterion dietitian referral pathway"
    - "11-class polypharmacy table (6 base + 5 sarcopenia-specific)"
    - "8 clinical validity questions template — Section 15 (replicating P-01 pattern)"
key_files:
  created:
    - protocols/P-08-SARCOPENIA.md
  modified:
    - protocols/SHARED-FOUNDATION.md
decisions:
  - "[02-01]: EWGSOP2 (2018) confirmed as operative standard — GLIS 2024 is conceptual only; no numerical cutoffs published as of 2026-03-13"
  - "[02-01]: Fried Frailty Phenotype used as dosage stratifier (not EWGSOP2 severity) — consistency with SHARED-FOUNDATION and all 20 protocols"
  - "[02-01]: Sarcopenia Grave + Frágil interaction rule: 20% additional load reduction on Frágil tier baseline"
  - "[02-01]: 11 polypharmacy classes (6 base + statins, aromatase inhibitors, loop diuretics, chronic corticosteroids extended detail, SSRIs)"
  - "[02-01]: Protein-exercise coordination classified as Nivel A (CEBM 1) — PROT-AGE + PMC12288929"
metrics:
  duration_minutes: 8
  completed_date: "2026-03-13"
  tasks_completed: 2
  tasks_total: 2
  files_created: 1
  files_modified: 1
  lines_written: 929
requirements_satisfied: [PROT-02]
---

# Phase 2 Plan 01: P-08 Sarcopenia Protocol Summary

**One-liner:** Complete sarcopenia rehabilitation protocol with EWGSOP2 FACS diagnostic algorithm and frailty-stratified resistance dosing modifier table as authoritative cross-protocol reference for all 20 protocols in the series.

---

## What Was Built

### Task 1: P-08-SARCOPENIA.md (929 lines)

Created a complete 15-section geriatric rehabilitation protocol for sarcopenia in Brazilian Portuguese, TIDieR/CERT compliant, with:

**Section 1 — Critérios Diagnósticos e de Inclusão:**
- EWGSOP2 FACS 4-step algorithm rendered as markdown flow diagram
- SARC-F 5-item screening questionnaire with scoring table
- Cutoffs: grip < 27 kg (M) / < 16 kg (F); ASM/h² < 7.0/5.5 kg/m² (DEXA/BIA); gait < 0.8 m/s / SPPB ≤ 8 / TUG > 20 for severity
- GLIS 2024 correctly positioned as contextual only — no operational cutoffs

**Section 6.3 — MODIFICADOR TRANSVERSAL:**
- Frailty-stratified resistance dosing table (Robusto/Pré-frágil/Frágil)
- Parameters: Robusto 65% 1RM; Pré-frágil 50% 1RM; Frágil 35% 1RM
- Sarcopenia Grave + Frágil rule: 20% additional load reduction
- Labeled as authoritative cross-protocol reference for all P-01 to P-20

**Section 10 — Polifarmácia:**
- 11 drug classes: 6 SHARED-FOUNDATION base + statins, aromatase inhibitors, loop diuretics, chronic corticosteroids (extended), SSRIs
- Statins: miotoxicidade confirmed causal association (PMC11503558)
- Subsection 10.3: Protein-exercise coordination with 5-criterion dietitian referral pathway (Nivel A evidence)

**Section 15 — 8 Questões de Validade Clínica:**
- All 8 questions answered with section cross-references
- Replicates P-01 template for series consistency

### Task 2: SHARED-FOUNDATION.md — P-08 Row

Updated Section 8.1 cross-reference matrix:
- Comorbidity interactions: P-04, P-01, P-05, P-07, P-10, P-11
- Shared modifier: resistance dosing table reference with summary parameters
- Specific precautions: EWGSOP2 severity classification rule and dietitian referral criteria

---

## Verification Results

All 10 verification criteria from the plan confirmed:

| # | Criterion | Status |
|---|-----------|--------|
| 1 | P-08-SARCOPENIA.md exists with ≥ 15 sections | PASS — 15 sections |
| 2 | EWGSOP2 FACS algorithm with 4 steps and operational cutoffs | PASS — Section 1.1 |
| 3 | Frailty-stratified resistance dosing modifier table labeled MODIFICADOR TRANSVERSAL | PASS — Section 6.3 |
| 4 | Protein-exercise coordination with dietitian referral pathway | PASS — Section 10.3 |
| 5 | Polypharmacy section has ≥ 9 drug class entries | PASS — 11 classes |
| 6 | All exercises have two-column dosage tables with 3 frailty rows | PASS — all phases |
| 7 | Section 15 answers all 8 clinical validity questions | PASS — Q1 through Q8 |
| 8 | SHARED-FOUNDATION.md Section 8.1 P-08 row populated | PASS — b129017 |
| 9 | Entire document in Brazilian Portuguese | PASS |
| 10 | Oxford CEBM evidence annotations on all interventions | PASS — Nivel A/B/C on each |

Automated verification: 102 term matches (threshold: 40); grep -c threshold test passed.

---

## Commits

| Task | Commit | Message |
|------|--------|---------|
| 1 | 8e45436 | feat(02-01): create P-08-SARCOPENIA.md — complete 15-section geriatric rehabilitation protocol |
| 2 | b129017 | feat(02-01): update SHARED-FOUNDATION cross-reference index with P-08 row |

---

## Deviations from Plan

None — plan executed exactly as written.

The plan specified the MODIFICADOR TRANSVERSAL in the Cinesioterapia subsection of Phase 2 (Seção 6.3) — placed exactly there. Drug class count ≥ 9 achieved as 11 (plan permitted additional entries). Protein-exercise coordination section placed in Section 10.3 with exactly the 5-criterion referral pathway specified in the research template.

---

## Key Decisions

1. **EWGSOP2 as operative standard:** GLIS 2024 explicitly acknowledged as conceptual only — no numerical cutoffs. Note embedded in P-08 header and Section 3. Consistent with STATE.md active blocker documentation.

2. **Fried Frailty Phenotype (not EWGSOP2 severity) as dosage stratifier:** Critical architectural decision — sarcopenia severity (Provável/Confirmada/Grave) maps to clinical context WITHIN each frailty tier, not to independent dosage rows. This maintains cross-protocol consistency with SHARED-FOUNDATION.

3. **Sarcopenia Grave + Frágil interaction rule (20% additional reduction):** Derived from research template; explicitly annotated on the MODIFICADOR TRANSVERSAL table. Provides safety margin for the most vulnerable patients.

4. **11 polypharmacy classes:** 6 base + 5 sarcopenia-specific (statins with causal evidence from PMC11503558; aromatase inhibitors for post-menopausal women; loop diuretics via hypokalemia mechanism; chronic corticosteroids with extended detail; SSRIs in chronic use). Corticosteroids appear in both base (general) and extended (fiber type II-specific miopatia) sections — counted as 11 distinct entries.

5. **Protein-exercise coordination as Nivel A:** PROT-AGE (2013) and PMC12288929 (2025) both provide Level 1 CEBM evidence for combined protein+RT synergy — elevated from B to A.

---

## Self-Check

**Files created/modified:**
- `C:/Projects/research/protocols/P-08-SARCOPENIA.md` — FOUND (929 lines, created 2026-03-13)
- `C:/Projects/research/protocols/SHARED-FOUNDATION.md` — FOUND (P-08 row populated, 2 references)

**Commits:**
- `8e45436` — FOUND (feat(02-01): create P-08-SARCOPENIA.md)
- `b129017` — FOUND (feat(02-01): update SHARED-FOUNDATION cross-reference index with P-08 row)

## Self-Check: PASSED
