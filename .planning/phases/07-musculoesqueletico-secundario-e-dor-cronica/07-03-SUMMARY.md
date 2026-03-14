---
phase: 07-musculoesqueletico-secundario-e-dor-cronica
plan: "03"
subsystem: protocols
tags: [ombro-doloroso, impingement, capsulite-adesiva, tendinopatia-manguito, gonalgia, coxalgia, artrose-conservadora, DASH-BR, WOMAC-BR, cross-reference-index, sensibilizacao-central, CSI-BR]

# Dependency graph
requires:
  - phase: 01-fundacao-e-template
    provides: 15-section protocol template (P-01), SHARED-FOUNDATION universal standards
  - phase: 02-modificadores-transversais
    provides: P-04 Seção 5.2 bone-loading constraint table, P-08 Seção 6.3 resistance dosing modifier
  - phase: 03-infraestrutura-de-seguranca-de-quedas
    provides: P-07 Seção 5.2 session fall-risk protocol, P-07 Seção 7.2 balance hierarchy
  - phase: 06-cluster-cardiorrespiratorio
    provides: Universal cardiorespiratory template (SHARED-FOUNDATION Seção 7.4) — Sections 11.1 + 11.2 verbatim
  - plan: 07-01
    provides: P-02, P-09 — lumbar trio differentiation framework; NÃO COBRE structural patterns
  - plan: 07-02
    provides: P-12, P-19 — DLC inespecífica and vertebral fractures cross-reference data
provides:
  - protocols/P-13-SINDROME-OMBRO-DOLOROSO.md — complete protocol for shoulder pain syndrome (SIS/adhesive capsulitis/rotator cuff tendinopathy/mixed)
  - protocols/P-20-GONALGIA-COXALGIA-DEGENERATIVA.md — complete protocol for knee/hip OA in definitive conservative management
  - protocols/SHARED-FOUNDATION.md — Section 8.1 cross-reference index updated with 6 new rows (P-02, P-09, P-12, P-13, P-19, P-20) — 18/20 rows now complete
affects:
  - SHARED-FOUNDATION.md Seção 8.1 (16 rows now populated; P-14 and P-17 remain pending)

# Tech tracking
tech-stack:
  added: []
  patterns:
    - "P-13 mechanism-based differentiation — SIS/capsulite/tendinopatia/mista as structural decision before protocol entry; distinct dosage tables per mechanism"
    - "P-13 CSI-BR >= 40 triggers PNE adjunct + time-contingent progression (minimum 3 weeks Phase 1, 4 weeks Phase 2)"
    - "P-20 permanent Phase 3 — no conventional discharge; quarterly review protocol; formal expectation management as structural component"
    - "P-20 WOMAC-BR primary with explicit KOOS-BR/HOOS-BR caution note (validation not confirmed at same rigor)"
    - "P-20 vs P-01 scope differentiation formalized — 6-dimension table distinguishing conservative definitive from pre-surgical"
    - "SHARED-FOUNDATION 6-row update completes Phase 7 cross-reference integration — Lombalgia-Osteoporose, Ombro-ATQ, Gonalgia-Artrose, Fraturas-Osteoporose pathways documented"

key-files:
  created:
    - protocols/P-13-SINDROME-OMBRO-DOLOROSO.md
    - protocols/P-20-GONALGIA-COXALGIA-DEGENERATIVA.md
  modified:
    - protocols/SHARED-FOUNDATION.md

key-decisions:
  - "P-13 asymptomatic rotator cuff tears in elderly: explicit note that prevalence of complete tears increases with age (10% at 60-70 years → 30% at >80 years); preserved function with asymptomatic complete tear is NOT a surgical indication — patient education mandatory"
  - "P-13 corticosteroid injection (CSI) positioning: NICE NG228 — CSI is a therapeutic window facilitator, not standalone treatment; exercise must follow within 2-3 days; max 3/year"
  - "P-20 Phase 3 is permanent (not a transition to surgery): HEP indefinitely + quarterly review + formal expectation management + community exercise integration"
  - "P-20 rapid decline criterion: WOMAC worsening >20% in 3 months = signal physician to reconsider surgical option (redirect to P-01 pathway)"
  - "P-20 WOMAC-BR confirmed as primary (Oliveira 2022, PMC9673866); KOOS-BR/HOOS-BR as secondary with explicit validation caution note"
  - "SHARED-FOUNDATION status: 18/20 rows complete after Phase 7 — P-14 (Assoalho Pélvico) and P-17 (Neuropatia Periférica) remain pending for Phase 8"

patterns-established:
  - "Pattern: Mechanism-Based Protocol Entry — P-13 differentiates SIS/capsulite/tendinopatia BEFORE prescribing; inversão terapêutica at mechanism level (isometric first for tendinopathy; grade I-II mobilization first for capsulitis Stage I; scapular stabilization first for SIS)"
  - "Pattern: Permanent Maintenance Protocol — P-20 Fase 3 has no exit; quarterly review cycle; expectation management as formal structural component (not a note)"
  - "Pattern: Cross-Reference Completion — SHARED-FOUNDATION now reflects all Phase 7 protocols with documented interaction pathways including therapeutic inversions (P-02 flexion vs. P-09 extension)"

requirements-completed: [PROT-17, PROT-18]

# Metrics
duration: 16min
completed: 2026-03-14
---

# Phase 07 Plan 03: P-13 Síndrome do Ombro Doloroso + P-20 Gonalgia/Coxalgia Degenerativa + SHARED-FOUNDATION Cross-Reference Update

**Mechanism-based ombro protocol (SIS/capsulite/tendinopatia), permanent-maintenance conservative OA protocol (P-20 with quarterly review), and SHARED-FOUNDATION cross-reference index updated with 6 new Phase 7 rows completing 18/20 protocols**

## Performance

- **Duration:** 16 min
- **Started:** 2026-03-14T10:49:46Z
- **Completed:** 2026-03-14T11:05:45Z
- **Tasks:** 2/2
- **Files created:** 2
- **Files modified:** 1

## Accomplishments

- P-13 created: 15 sections; mechanism-based differentiation (SIS / capsulite adesiva por estágio / tendinopatia de manguito / apresentação mista); DASH-BR primary outcome (Orfale 2005, PubMed 15821858) with MCID 10-14 pts; SPADI-BR alternative (Martins 2010, PubMed 20802993); CSI-BR >= 40 triggers PNE adjunct + time-contingent progression; cardiac origin exclusion for left shoulder (before any SIS diagnosis); frailty-stratified dosage tables per mechanism; universal Section 11 template; NÃO COBRE block (OA glenoumeral → P-01; cervical radiculopathy → P-09; post-arthroplasty shoulder; pseudoparalysis)
- P-20 created: 15 sections; explicit 6-dimension population differentiation from P-01 (conservative definitive vs. pre-surgical); Phase 3 is PERMANENT maintenance (no conventional discharge); WOMAC-BR primary (Oliveira 2022, PMC9673866) with KOOS-BR/HOOS-BR caution note; quarterly review protocol (Section 7.2); formal expectation management (Section 7.3, 6 structural topics); permanent AVD adaptations (Section 7.4); rapid-decline criterion triggers P-01 reconsideration; P-08 mandatory in ALL patients; universal Section 11 template; NÃO COBRE block (P-01 if surgical decision open, P-10, P-11, P-05)
- SHARED-FOUNDATION Section 8.1 updated: 6 new rows added (P-02, P-09, P-12, P-13, P-19, P-20); status updated to 18/20 complete; all key interaction pathways from Phase 7 success criteria documented (Lombalgia-Osteoporose, Ombro-ATQ, Gonalgia-Artrose, Fraturas-Osteoporose)

## Task Commits

Each task was committed atomically:

1. **Task 1: P-13 Sindrome do Ombro Doloroso + P-20 Gonalgia/Coxalgia Degenerativa** - `8a44d53` (feat)
2. **Task 2: SHARED-FOUNDATION Cross-Reference Index Update** - `8d878eb` (feat)

**Plan metadata:** *(docs commit — this summary)*

## Files Created

- `protocols/P-13-SINDROME-OMBRO-DOLOROSO.md` — 719 lines; 15 sections; mechanism-based differentiation (SIS/capsulite/tendinopatia/mista) as structural entry decision; DASH-BR primary outcome; CSI-BR >= 40 protocol (PNE adjunct + time-contingent); goniometric ROM assessment; frailty-stratified dosage tables per mechanism; cardiac exclusion for left shoulder; asymptomatic rotator cuff tears prevalence note; corticosteroid injection (CSI) as therapeutic window facilitator; NÃO COBRE block; universal Section 11.1/11.2 verbatim
- `protocols/P-20-GONALGIA-COXALGIA-DEGENERATIVA.md` — 659 lines; 15 sections; explicit P-20 vs. P-01 differentiation table (6 dimensions); Phase 3 PERMANENT maintenance with quarterly review protocol; WOMAC-BR primary with KOOS/HOOS caution note; formal expectation management component; permanent AVD adaptations; rapid-decline criterion (WOMAC >20% in 3 months = reconsider surgical option); P-08 mandatory for ALL patients; NÃO COBRE block; universal Section 11.1/11.2 verbatim

## Files Modified

- `protocols/SHARED-FOUNDATION.md` — Section 8.1 status updated (18/20 rows complete); 6 rows filled: P-02 (flexion bias + cauda equina chain), P-09 (extension recommended + P-04 gate + therapeutic inversion), P-12 (PNE as CENTRAL + opioid risk), P-13 (cardiac exclusion + CSI + asymptomatic tears), P-19 (P-04 co-manager + flexion contraindicated + hip hinge permanent), P-20 (permanent Phase 3 + P-08 mandatory + P-01 decline trigger)

## Decisions Made

- **P-13 asymptomatic rotator cuff tears:** Explicit clinical note on prevalence with age (10% at 60-70 → 30% at >80 years); preserved function = no surgical indication; patient education on degenerative nature is mandatory in Phase 1 for tendinopathy subtype
- **P-13 CSI positioning:** NICE NG228 frames CSI as therapeutic window facilitator — retake exercise within 2-3 days; max 3 injections/year; not standalone treatment
- **P-20 Phase 3 is permanent:** No conventional discharge in P-20 — quarterly review cycle replaces episodic treatment; formal expectation management is structural (not a note); community exercise integration as sustainability mechanism
- **P-20 WOMAC-BR confirmed primary:** Oliveira 2022 (PMC9673866) as validation source; KOOS-BR/HOOS-BR secondary with explicit validation caution note documented
- **P-20 rapid decline criterion:** WOMAC worsening >20% in 3 months OR conservative failure >12 months = signal physician to reconsider surgical pathway (return to P-01)
- **SHARED-FOUNDATION Phase 7 complete:** 18/20 rows filled after this plan; P-14 (Assoalho Pélvico) and P-17 (Neuropatia Periférica) remain pending for Phase 8

## Deviations from Plan

None — plan executed exactly as written. Both protocols created with all required content elements. SHARED-FOUNDATION updated with all 6 rows including all key interaction pathways specified in the plan success criteria.

## Issues Encountered

None.

## User Setup Required

None — no external service configuration required.

## Next Phase Readiness

- Phase 7 complete: All 6 protocols (P-02, P-09, P-12, P-13, P-19, P-20) created and integrated into SHARED-FOUNDATION cross-reference system
- 16 of 20 protocols now complete across all phases
- SHARED-FOUNDATION cross-reference index: 18/20 rows filled (P-14, P-17 pending Phase 8)
- Phase 8 will create P-14 (Disfunção do Assoalho Pélvico) and P-17 (Neuropatia Periférica Diabética) to complete the full set of 20 protocols

---
*Phase: 07-musculoesqueletico-secundario-e-dor-cronica*
*Completed: 2026-03-14*
