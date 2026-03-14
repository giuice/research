---
phase: 08-protocolos-especializados
plan: "02"
subsystem: clinical-protocols
tags: [disfuncao-assoalho-pelvico, DAP, PFMT, down-training, hipertonico, hipotonico, ICIQ-SF-BR, Modified-Oxford, PERFECT, geriatria, fisioterapia-pelvica, incontinencia-urinaria]

# Dependency graph
requires:
  - phase: 01-fundacao-e-template
    provides: "15-section protocol structure, Fried frailty stratification, SHARED-FOUNDATION universal standards"
  - phase: 02-modificadores-transversais
    provides: "P-04 bone load modifier (Section 5.2), P-08 resistance dosing modifier (Section 6.3)"
  - phase: 03-infraestrutura-de-seguranca-de-quedas
    provides: "P-07 fall risk session protocol (Section 5.2) and balance hierarchy (Section 7.2)"
  - phase: 06-cluster-cardiorrespiratorio
    provides: "Universal Section 11 cardiorespiratory template (SHARED-FOUNDATION 7.4)"
  - phase: 08-protocolos-especializados
    provides: "P-17 structure and 08-RESEARCH.md content for P-14"

provides:
  - "P-14-DISFUNCAO-ASSOALHO-PELVICO.md: complete 721-line 15-section protocol for pelvic floor dysfunction in elderly women"
  - "Passo 0 Estrutural: mandatory hypertonic vs. hypotonic classification framework before any exercise selection"
  - "Down-training therapeutic track for hypertonic pelvic floor (diaphragmatic breathing, relaxation, inhibition biofeedback, myofascial release)"
  - "PFMT/up-training therapeutic track for hypotonic pelvic floor (progressive Kegel, activation biofeedback, electrostimulation, The Knack)"
  - "ICIQ-SF-BR (PMID 15243675) as primary outcome instrument with MCID note"
  - "Cross-protocol chain: P-07 (fall risk) → P-08 (pelvic sarcopenia) → P-04 (osteoporosis load)"
  - "ABRAFISM 2025 + ICS/IUGA 2010 terminology throughout"

affects:
  - "SHARED-FOUNDATION.md Seção 8.1 (two pending rows: P-14 and P-17 to be added in Phase 8 Plan 03 if applicable)"
  - "Phase 08 Plan 03 (cross-reference index finalization)"

# Tech tracking
tech-stack:
  added: []
  patterns:
    - "Bifurcated therapeutic protocol: single protocol with diametrically opposed treatment tracks by subtype (first in corpus)"
    - "Passo 0 Estrutural as mandatory classification gate before any exercise prescription"
    - "Frailty-stratified two-column dosage tables (Robusto/Pré-frágil/Frágil) applied to perineal exercise parameters"
    - "MCID with explicit confidence notation: '(estimativa baseada na literatura; MCID geriátrico BR não publicado)'"
    - "Contraindication explicitly embedded in dosage table via CONTRAINDICAÇÃO ABSOLUTA callout"

key-files:
  created:
    - protocols/P-14-DISFUNCAO-ASSOALHO-PELVICO.md
  modified: []

key-decisions:
  - "Passo 0 Estrutural (mandatory tônus classification: hipertônico vs. hipotônico vs. misto) positioned as structural Step 0 in Section 1.4 — before any exercise selection — to prevent iatrogenic error of prescribing PFMT to hypertonic pelvic floor"
  - "Kegel (PFMT) explicitly labeled CONTRAINDICAÇÃO ABSOLUTA in Fase 1 for hypertonic subtypes — embedded directly in the dosage section to prevent clinical error at point of care"
  - "ICIQ-SF-BR MCID ≥ 3 points documented with MEDIUM confidence note: '(estimativa baseada na literatura; MCID geriátrico BR não publicado)' — honoring 08-RESEARCH.md uncertainty"
  - "Fase 3 declared PERMANENTE for P-14 — DAP in elderly women is chronic; discharge implies transition to autonomous HEP with quarterly review, not cessation of treatment"
  - "Oxford ≤ 2 (pelvic sarcopenia) triggers passive electrostimulation BEFORE active PFMT — insufficient voluntary recruitment makes active PFMT ineffective"
  - "MMSE < 18 declared absolute contraindication for active PFMT — electrostimulation passiva as primary alternative"
  - "FES-I-BR ≥ 23 activates P-07 Section 5.2 — urge incontinence to bathroom = fall mechanism requiring formal fall prevention protocol"
  - "ABRAFISM 2025 (PMC11847513) adopted as primary Portuguese-language terminology reference for hypertônico/hipotônico — eliminates ambiguity in interprofessional communication"

patterns-established:
  - "Bifurcated protocol with subtype-determined track: applicable to future conditions where treatment approach inverts by subtype"
  - "Mandatory classification step (Passo 0) before exercise: template for protocols where wrong-subtype prescription causes harm"

requirements-completed: [PROT-20]

# Metrics
duration: 6min
completed: 2026-03-14
---

# Phase 8 Plan 02: P-14 Disfunção do Assoalho Pélvico Summary

**P-14 pelvic floor dysfunction protocol with mandatory hypertonic/hypotonic classification (Passo 0 Estrutural) gating divergent down-training vs. PFMT therapeutic tracks, ICIQ-SF-BR (PMID 15243675) as primary outcome, and explicit Kegel contraindication for hypertonic subtype**

## Performance

- **Duration:** 6 min
- **Started:** 2026-03-14T11:47:49Z
- **Completed:** 2026-03-14T11:53:00Z
- **Tasks:** 2 (Research + Authorship executed as unified task — research content fed directly into document)
- **Files modified:** 1

## Accomplishments

- Created 721-line complete 15-section protocol P-14 in Brazilian Portuguese per TIDieR/CERT standards
- Passo 0 Estrutural with full classification framework table (palpation, Oxford, PERFECT, symptoms, trigger points) — hypertonic vs. hypotonic vs. mixed, each routing to distinct therapeutic track
- Down-training Phase 1 (5b) with explicit CONTRAINDICAÇÃO ABSOLUTA callout for Kegel in hypertonic; up-training Phase 1 (5a) with frailty-stratified Kegel dosage; sequential Phase 1 (5c) for mixed
- ICIQ-SF-BR cited with PMID 15243675 (Tamanini 2004) + PERFECT Scheme + Modified Oxford + FES-I-BR + PFDI-20-BR (Arouca 2016) + EVA dor pélvica as assessment battery
- Cross-protocol modifier chain: P-07 (fall risk when FES-I ≥ 23) → P-08 (pelvic sarcopenia when Oxford ≤ 2) → P-04 (osteoporosis load precautions)
- Universal Section 11 cardiorespiratory template verbatim from SHARED-FOUNDATION 7.4 including Valsalva-specific warning for DAP patients
- All 8 clinical validity questions answered with actionable non-response algorithm (Q8)

## Task Commits

1. **Task 1+2: Research and Authorship P-14** - `e538f72` (feat) — Tasks 1 and 2 executed as unified research-to-document workflow per plan design

## Files Created/Modified

- `C:/Projects/research/protocols/P-14-DISFUNCAO-ASSOALHO-PELVICO.md` — Complete 721-line protocol for pelvic floor dysfunction: 15 sections, bifurcated therapeutic tracks, frailty-stratified dosage tables, NÃO COBRE block, universal Section 11, 8 clinical validity questions

## Decisions Made

- **Passo 0 Estrutural**: Positioned prominently in Section 1.4 with classification table (5 assessment parameters × 3 subtypes) and routing checkboxes ([ ] Hipertônico / [ ] Hipotônico / [ ] Misto) — clinician uses checklist format before any prescription
- **CONTRAINDICAÇÃO ABSOLUTA Kegel in hypertonic**: Embedded as blockquote callout directly within the Fase 1 Via Hipertônico dosage section (5b) — not hidden in text but at point of prescription decision
- **MCID ≥ 3 with MEDIUM confidence note**: Documented per 08-RESEARCH.md: "(estimativa baseada na literatura; MCID geriátrico BR não publicado)" — honest evidence annotation
- **Fase 3 is PERMANENT**: Explicitly stated as "Nota IMPORTANTE" — prevents clinicians from discharging patients when they reach Fase 3 (common error in DAP management in elderly)
- **Oxford ≤ 2 = electrostimulation first**: Codified as rule in Section 2.3 geriatric adaptations — pelvic sarcopenia mechanism explained
- **ABRAFISM 2025 + ICS/IUGA 2010**: Dual-standard terminology table in Section 1.1 maps terms to Portuguese-Brazilian clinical practice

## Deviations from Plan

None — plan executed exactly as written. Research (Task 1) and authorship (Task 2) executed as unified workflow with research findings feeding directly into the protocol document, as intended by the plan design.

## Issues Encountered

None.

## User Setup Required

None — no external service configuration required.

## Next Phase Readiness

- P-14 complete — PROT-20 requirement fulfilled
- Both P-17 (08-01) and P-14 (08-02) now complete
- Remaining: SHARED-FOUNDATION Seção 8.1 needs P-14 and P-17 rows added (OUT-04 requirement) — this is Phase 08 Plan 03 if it exists, or can be addressed in a follow-up plan
- All cross-protocol links confirmed: P-07 Seção 5.2, P-08 Seção 6.3, P-04 Seção 5.2 referenced correctly

---
*Phase: 08-protocolos-especializados*
*Completed: 2026-03-14*
