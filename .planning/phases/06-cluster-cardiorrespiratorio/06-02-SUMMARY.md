---
phase: 06-cluster-cardiorrespiratorio
plan: "02"
subsystem: clinical-protocols
tags: [cardiorespiratory-precautions, universal-template, retroactive-update, section-11, safety-floor]

# Dependency graph
requires:
  - phase: 06-cluster-cardiorrespiratorio
    plan: "01"
    provides: "Universal Section 11 template from P-15 DPOC + SHARED-FOUNDATION Seção 7.4"
provides:
  - "Universal Cardiorespiratory Precautions section (11.1 + 11.2) in all 10 Phase 1-5 protocols"
  - "Condition-specific Section 11.4 in each of the 10 updated protocols"
  - "SHARED-FOUNDATION Section 7.4.5 documenting the retroactive pass with dated record"
  - "Consistent safety floor: any clinician opening any of 12 protocols finds identical pre-session protocol"
affects:
  - 07-cluster-ortopedia
  - all future phases (Phases 7-8 must include template at creation time)

# Tech tracking
tech-stack:
  added: []
  patterns:
    - "Universal Section 11 template: 11.1 (pre-session table) + 11.2 (stop criteria table) VERBATIM across all protocols; 11.3 (comorbidity adaptations) + 11.4 (protocol-specific) vary"
    - "Retroactive update pass pattern: document with dated record in SHARED-FOUNDATION when applying corpus-wide changes"
    - "Future protocol creation instruction: Phases 7-8 must include universal template at creation, not via retroactive pass"

key-files:
  created: []
  modified:
    - protocols/P-01-OSTEOARTRITE.md
    - protocols/P-03-AVC.md
    - protocols/P-04-OSTEOPOROSE.md
    - protocols/P-05-FRATURA-FEMUR.md
    - protocols/P-06-PARKINSON.md
    - protocols/P-07-QUEDAS.md
    - protocols/P-08-SARCOPENIA.md
    - protocols/P-10-ATJ.md
    - protocols/P-11-ATQ.md
    - protocols/P-18-DEMENCIA.md
    - protocols/SHARED-FOUNDATION.md

key-decisions:
  - "Universal template subsections 11.1 and 11.2 applied VERBATIM from P-15 DPOC — no threshold variations across protocols"
  - "Existing 11.3 content (ICC/DPOC adaptations) preserved and updated with P-15/P-16 cross-references; renamed to 11.3 Adaptações por Comorbidade"
  - "New 11.4 Especificidades added to each protocol with condition-specific content from plan specification"
  - "SHARED-FOUNDATION Section 7.4.5 documents the pass with per-protocol status table (ATUALIZADO/ORIGINAL) and canonical threshold reference"
  - "Phases 7-8 protocols instructed to include template at creation time — no future retroactive pass needed"

requirements-completed: [PROT-11, PROT-12]

# Metrics
duration: 20min
completed: 2026-03-13
---

# Phase 6 Plan 02: Retroactive Cardiorespiratory Precautions Update Summary

**Universal Cardiorespiratory Precautions template (PA >180/110, FC >120, SpO2 <90%, Borg >=5) applied retroactively to all 10 Phase 1-5 protocols with condition-specific Section 11.4 for each, creating a consistent safety floor across the 12-protocol cardiorespiratory cluster**

## Performance

- **Duration:** 20 min
- **Started:** 2026-03-13T22:12:29Z
- **Completed:** 2026-03-13T22:32:00Z
- **Tasks:** 2/2
- **Files modified:** 11 (10 protocols + SHARED-FOUNDATION)

## Accomplishments

- All 10 Phase 1-5 protocols now have identical Section 11.1 (Protocolo de Avaliação Pré-Sessão) and 11.2 (Indicadores de Parada Imediata) with universal thresholds
- Each protocol received a condition-specific Section 11.4 preserving and expanding its unique cardiorespiratory content (OA, AVC, Osteoporose, Fratura Fêmur, Parkinson, Quedas, Sarcopenia, ATJ, ATQ, Demência)
- SHARED-FOUNDATION Section 7.4.5 documents the retroactive update pass with dated record, per-protocol status (ATUALIZADO/ORIGINAL), canonical threshold reference table, and instruction for Phases 7-8
- Phase 6 Success Criterion 3 fulfilled: all 12 protocol files present the same pre-session safety protocol regardless of primary diagnosis

## Task Commits

1. **Task 1: Audit and apply universal template to 10 protocols** - `4548420` (feat)
2. **Task 2: Document retroactive update pass in SHARED-FOUNDATION** - `d5e05a4` (feat)

## Files Created/Modified

- `protocols/P-01-OSTEOARTRITE.md` — Section 11 updated: universal 11.1 + 11.2 + 11.4 (cardiovascular risk in sedentary elderly + AINEs impact)
- `protocols/P-03-AVC.md` — Section 11 updated: universal 11.1 + 11.2 + 11.4 (FA monitoring + anticoagulation + autonomic dysfunction + new neurological deficit indicator)
- `protocols/P-04-OSTEOPOROSE.md` — Section 11 updated: universal 11.1 + 11.2 + 11.4 (Valsalva + bisphosphonate orthostatic hypotension + corticosteroids)
- `protocols/P-05-FRATURA-FEMUR.md` — Section 11 updated: universal 11.1 + 11.2 + 11.4 (TEV table + anemia + orthostatic hypotension protocol) + placeholder removed
- `protocols/P-06-PARKINSON.md` — Section 11 updated: universal 11.1 + 11.2 + 11.4 (autonomic dysfunction + respiratory compromise in advanced DP + levodopa-BP fluctuations)
- `protocols/P-07-QUEDAS.md` — Section 11 updated: universal 11.1 + 11.2 + 11.4 (orthostatic hypotension as fall risk + PBT monitoring + STOPPFall cardiovascular medications) + placeholder removed
- `protocols/P-08-SARCOPENIA.md` — Section 11 updated: universal 11.1 + 11.2 + 11.4 (HIRT cardiovascular screening contraindications + Valsalva in osteosarcopenia)
- `protocols/P-10-ATJ.md` — Section 11 updated: universal 11.1 + 11.2 + 11.4 (TEV post-ATJ with tourniquet + orthostatic hypotension protocol)
- `protocols/P-11-ATQ.md` — Section 11 updated: universal 11.1 + 11.2 + 11.4 (TEV post-ATQ + surgical cardiovascular risk + orthostatic hypotension)
- `protocols/P-18-DEMENCIA.md` — Section 11 updated: universal 11.1 + 11.2 + 11.4 (limited symptom reporting capacity + behavioral substitutes table + caregiver instruction)
- `protocols/SHARED-FOUNDATION.md` — Section 7.4.5 added with retroactive pass documentation

## Decisions Made

- Universal template subsections 11.1 and 11.2 applied VERBATIM from P-15 DPOC — consistent with plan requirement; no threshold variations across protocols
- Existing 11.3 content (generic ICC/DPOC adaptations) was preserved and renamed to "Adaptações por Comorbidade Cardiorrespiratória Coexistente" with added P-15/P-16 cross-references
- New condition-specific Section 11.4 added to each protocol drawing from plan specification for each condition
- P-07 QUEDAS placeholder note "Atualização cardiorrespiratória retroativa planejada para Fase 6" removed (fulfilled)
- P-05 FRATURA-FEMUR placeholder "Placeholder para Fase 6" removed (fulfilled)
- SHARED-FOUNDATION Section 7.4.5 uses ATUALIZADO/ORIGINAL status labels for clear audit trail

## Deviations from Plan

None - plan executed exactly as written.

## Issues Encountered

None.

## User Setup Required

None - no external service configuration required.

## Next Phase Readiness

- Phase 6 is now complete: P-15 (DPOC) + P-16 (IC) created in Plan 06-01; all 10 prior protocols updated with universal template in Plan 06-02
- Phase 7 (Cluster Ortopédico) can begin. New protocols created in Phase 7+ must include the universal cardiorespiratory template at creation time per SHARED-FOUNDATION Section 7.4.5
- P-02/P-12 differentiation analysis is mandatory before any drafting in Phase 7 (per STATE.md decision)

---
*Phase: 06-cluster-cardiorrespiratorio*
*Completed: 2026-03-13*
