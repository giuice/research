---
phase: 07-musculoesqueletico-secundario-e-dor-cronica
plan: "02"
subsystem: protocols
tags: [dor-lombar-cronica-inespecifica, PNE, CSI-BR, sensibilizacao-central, fratura-vertebral, osteoporose, P-04-co-gerente, seguranca-maxima, ODI-BR, FES-I-BR]

# Dependency graph
requires:
  - phase: 01-fundacao-e-template
    provides: 15-section protocol template (P-01), SHARED-FOUNDATION universal standards
  - phase: 02-modificadores-transversais
    provides: P-04 Seção 5.2 bone-loading constraint table (governs ALL P-19 exercises), P-08 Seção 6.3 resistance dosing modifier
  - phase: 03-infraestrutura-de-seguranca-de-quedas
    provides: P-07 Seção 5.2 session fall-risk protocol, P-07 Seção 7.2 balance hierarchy (mandatory in P-19 post-fracture)
  - phase: 06-cluster-cardiorrespiratorio
    provides: Universal cardiorespiratory template (SHARED-FOUNDATION Seção 7.4) — Sections 11.1 + 11.2 verbatim
  - phase: 07-musculoesqueletico-secundario-e-dor-cronica
    plan: "01"
    provides: Scope differentiation analysis lumbar trio (P-02/P-09/P-12) embedded in P-02; P-12 anchors its non-structural identity against P-02/P-09
provides:
  - P-12-DOR-LOMBAR-CRONICA-INESPECIFICA.md — complete biopsychosocial protocol with PNE as CENTRAL component; CSI-BR mandatory; time-contingent progression for CSI >= 40
  - P-19-FRATURAS-VERTEBRAIS-COMPRESSAO.md — highest safety-risk protocol; P-04 Seção 5.2 governs all exercises; flexion contraindicated Phases 1-2; cauda equina maximum emergency
affects:
  - SHARED-FOUNDATION.md Seção 8.1 (P-12 and P-19 rows now populated)
  - Any future protocol referencing PNE as central component should follow P-12 model
  - Any future protocol with osteoporosis substrate must cite P-04 Seção 5.2 per P-19 pattern

# Tech tracking
tech-stack:
  added: []
  patterns:
    - "PNE as CENTRAL component in P-12 (4 formal modules 30-40 min each) vs. PNE as ADJUNCT in P-02/P-09/P-19 (2-3 informal sessions) — differentiation established"
    - "CSI-BR MANDATORY at admission in P-12 with full action plan table by score range (0-29/30-39/40-49/>=50) — most rigorous psychosocial assessment in the series"
    - "Time-contingent progression (CSI >= 40): NRS removed as progression criterion; TUG/SPPB/PSFS-BR/Confidence Scale govern advancement"
    - "Movement Confidence Scale (0-10) introduced as progression criterion when NRS is unreliable"
    - "P-04 Seção 5.2 as mandatory TETO (ceiling) for EVERY exercise in P-19 — documented per intervention"
    - "Vertebral flexion CONTRAINDICADA Phases 1-2 in P-19 (Sinaki 1984 PubMed 6487063 — 89% vs. 16% new fracture rate)"
    - "Hip hinge as permanent movement pattern (P-19): taught Session 1, practiced in ALL ADLs, maintained indefinitely post-discharge"
    - "Osteosarcopenia dual ceiling rule: min(P-04 Seção 5.2 teto, P-08 Seção 6.3 teto) governs resistance dosing"
    - "Post-vertebroplasty/kyphoplasty: cement does not change P-04 restrictions; adjacent vertebra risk explicitly documented"

key-files:
  created:
    - protocols/P-12-DOR-LOMBAR-CRONICA-INESPECIFICA.md
    - protocols/P-19-FRATURAS-VERTEBRAIS-COMPRESSAO.md
  modified: []

key-decisions:
  - "PNE as CENTRAL component in P-12: 4 formal structured modules (30-40 min each) with specific content per module — contrasts with PNE ADJUNCT in all other protocols in the series"
  - "CSI-BR >= 40 in P-12: time-contingent progression is the MANDATORY protocol (not optional) — NRS has no role as a progression criterion when sensibilização central is significant"
  - "Opioids in P-12 (Section 10.2): SPACE Trial (Krebs JAMA 2018) documented as Nível A evidence that opioids are not superior to non-opioids for DLC functional outcomes; opioid-induced hyperalgesia explicitly noted for CSI >= 40 patients"
  - "P-19: all patients in Phases 1-2 are classified as MUITO ALTO RISCO by default — no staging required; fracture = automatic classification"
  - "P-04 Seção 5.2 governs P-19 from the first line of the protocol — documented as structural requirement, not optional cross-reference"
  - "Vertebroplasty/kyphoplasty does not change P-04 restrictions — cement stabilizes the treated vertebra but adjacent vertebrae remain at elevated fracture risk (load transfer effect)"
  - "Neurological assessment mandatory at EACH SESSION in P-19 (quick cauda equina screen: sphincter control + perineal sensation) — not only at admission"

patterns-established:
  - "Pattern: PNE Central vs. Adjunct — P-12 establishes the model for PNE as primary intervention (4 modules); P-02/P-09/P-19 use PNE as adjunct (2-3 sessions)"
  - "Pattern: Teto P-04 per Exercise — P-19 establishes the model for documenting P-04 bone-loading ceiling for each exercise in a dosage table column"
  - "Pattern: Mandatory Psychosocial Assessment Battery — P-12 establishes CSI-BR + HADS-BR + PCS-BR as mandatory (not optional) at admission; contrasts with P-02/P-09 where CSI is conditional"

requirements-completed: [PROT-15, PROT-16]

# Metrics
duration: 20min
completed: 2026-03-14
---

# Phase 07 Plan 02: P-12 Dor Lombar Crônica Inespecífica + P-19 Fraturas Vertebrais por Compressão Summary

**P-12 (biopsychosocial protocol with PNE as central component, CSI-BR mandatory, time-contingent progression, opioid alert) and P-19 (highest safety-risk protocol, P-04 Section 5.2 as mandatory bone-loading constraint in all phases, vertebral flexion contraindicated Phases 1-2, cauda equina as maximum emergency)**

## Performance

- **Duration:** 20 min
- **Started:** 2026-03-14T10:24:59Z
- **Completed:** 2026-03-14T10:44:59Z
- **Tasks:** 2/2
- **Files created:** 2

## Accomplishments

- P-12 created: 752 lines; 15 sections; IASP Chronic Primary Pain (ICD-11 MG30.0) as diagnostic anchor; NAO COBRE block for P-02/P-09/P-19; CSI-BR MANDATORY with full action plan table (4 ranges: 0-29/30-39/40-49/>=50); PNE as CENTRAL component with 4 formal structured modules (30-40 min each); time-contingent progression for CSI >= 40; yellow flags section (HADS-BR, PCS-BR, fear-avoidance, social factors) with psychological referral pathway; opioid special section (Section 10.2) with SPACE Trial evidence and hyperalgesia paradox; Movement Confidence Scale; universal Section 11.1/11.2 verbatim; frailty-stratified dosage tables
- P-19 created: 759 lines; 15 sections; NAO COBRE block for P-04/P-02/P-09; P-04 Section 5.2 referenced as mandatory bone-loading constraint in ALL phases (45 P-04 refs, 30 Seção 5.2 refs); "Teto P-04" column in all dosage tables; vertebral flexion CONTRAINDICADA Phases 1-2 (Sinaki 1984 PubMed 6487063 — 89% vs. 16% new fracture rate); cauda equina as maximum emergency (SAMU 192 + NÃO MOBILIZAR); hip hinge as mandatory permanent pattern; FES-I-BR mandatory; neurological assessment per session (quick cauda equina screen); vertebroplasty/kyphoplasty section; osteosarcopenia dual ceiling rule (P-04 × P-08); P-07 Sections 5.2+7.2 mandatory; universal Section 11.1/11.2 verbatim; frailty-stratified dosage tables

## Task Commits

Each task was committed atomically:

1. **Task 1: P-12 Dor Lombar Cronica Inespecifica** — `abb6a29` (feat)
2. **Task 2: P-19 Fraturas Vertebrais por Compressao** — `759332a` (feat)

**Plan metadata:** *(docs commit — this summary)*

## Files Created

- `protocols/P-12-DOR-LOMBAR-CRONICA-INESPECIFICA.md` — 752 lines; 15 sections; IASP Chronic Primary Pain anchor; NAO COBRE (P-02/P-09/P-19); CSI-BR mandatory + full action plan table; PNE CENTRAL (4 modules 30-40 min each); time-contingent progression; yellow flags + HADS-BR mandatory; opioid special section (Section 10.2); Movement Confidence Scale; universal Section 11.1/11.2 verbatim
- `protocols/P-19-FRATURAS-VERTEBRAIS-COMPRESSAO.md` — 759 lines; 15 sections; NAO COBRE (P-04/P-02/P-09); P-04 Seção 5.2 mandatory in ALL phases (Teto P-04 per exercise); flexion CONTRAINDICADA Phases 1-2; cauda equina maximum emergency; hip hinge permanent; FES-I-BR mandatory; neurological assessment per session; vertebroplasty section; osteosarcopenia dual ceiling; universal Section 11.1/11.2 verbatim

## Decisions Made

- **PNE differentiation:** P-12 = PNE CENTRAL (4 formal modules 30-40 min; catastrofização, sensibilização central, graded exposure as primary targets); P-19 = PNE ADJUNCT (2 sessions, structural dor contextualização)
- **CSI-BR >= 40 mandatory action:** Time-contingent progression is NOT optional when CSI-BR >= 40 — it is the mandatory protocol with NRS removed as progression criterion; Movement Confidence Scale substitutes NRS
- **Opioids in DLC inespecífica:** SPACE Trial (Krebs JAMA 2018) documented as Nível A — opioids not superior to non-opioids for functional outcomes at 12 months; opioid-induced hyperalgesia explicitly documented for CSI >= 40 patients; prescribing clinician communication documented as fisioterapeuta responsibility
- **P-19 automatic Muito Alto Risco classification:** Any confirmed vertebral compression fracture = automatic Muito Alto Risco in P-04 Section 5.2 for Phases 1-2 — no FRAX/T-score calculation required for initial classification
- **Vertebroplasty/kyphoplasty:** Cement does not change P-04 bone-loading restrictions; adjacent vertebrae at elevated risk (load transfer) — P-04 restrictions maintained at Muito Alto Risco even post-procedure
- **Neurological screen per session:** Cauda equina quick screen (sphincter control + perineal sensation) made mandatory at each session in P-19, not only at admission — this is the highest-consequence emergency in the protocol

## Deviations from Plan

None — plan executed exactly as written. Both protocols created with all mandatory requirements:
- P-12: IASP Chronic Primary Pain anchor, CSI-BR mandatory with action table, PNE central with 4 structured modules, time-contingent progression, HADS-BR mandatory, opioid special section, yellow flags, 750+ lines, 15 sections
- P-19: P-04 Section 5.2 as mandatory bone-loading constraint in all phases, Teto P-04 per exercise, flexion contraindicated Phases 1-2 (Sinaki 1984), cauda equina in red flags, FES-I-BR mandatory, hip hinge permanent, 750+ lines, 15 sections

## Issues Encountered

None.

## User Setup Required

None — no external service configuration required.

## Next Phase Readiness

- Lumbar trio (P-02/P-09/P-12) is now complete — three differentiated protocols with zero content overlap in defining characteristics
- P-19 established the "Teto P-04 per exercise" pattern that may be reused in any future protocol with high osteoporosis burden
- Phase 7 Plan 02 complete; SHARED-FOUNDATION Seção 8.1 rows for P-12 and P-19 populated in each protocol's Section 13
- Next: Phase 7 Plan 03 (P-13 Síndrome do Ombro Doloroso, P-20 Gonalgia/Coxalgia Degenerativa) per ROADMAP

## Self-Check: PASSED

- protocols/P-12-DOR-LOMBAR-CRONICA-INESPECIFICA.md — FOUND
- protocols/P-19-FRATURAS-VERTEBRAIS-COMPRESSAO.md — FOUND
- .planning/phases/07-musculoesqueletico-secundario-e-dor-cronica/07-02-SUMMARY.md — FOUND
- Commit abb6a29 (P-12) — FOUND
- Commit 759332a (P-19) — FOUND

---

*Phase: 07-musculoesqueletico-secundario-e-dor-cronica*
*Completed: 2026-03-14*
