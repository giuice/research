# Roadmap: Protocolos de Reabilitação Geriátrica Baseados em Evidências

## Overview

Twenty evidence-based geriatric rehabilitation protocols, delivered sequentially in eight phases ordered by clinical knowledge dependencies. Phase 1 establishes the Shared Foundation Layer and the validated template protocol (P-01 Osteoartrite), locking all structural, assessment, dosage, evidence, safety, and output standards that every subsequent phase inherits. Phases 2–3 build the cross-protocol modifiers (Sarcopenia, Osteoporosis, Falls) that all later protocols reference. Phases 4–8 deliver the remaining 16 protocols in dependency order: high-complexity musculoskeletal, neuromotor, cardiorespiratory, secondary musculoskeletal/chronic pain, and specialized domains.

## Phases

**Phase Numbering:**
- Integer phases (1, 2, 3): Planned milestone work
- Decimal phases (2.1, 2.2): Urgent insertions (marked with INSERTED)

Decimal phases appear between their surrounding integers in numeric order.

- [ ] **Phase 1: Fundação e Template** - Shared Foundation Layer + P-01 Osteoartrite (template protocol establishing all standards)
- [ ] **Phase 2: Modificadores Transversais** - P-08 Sarcopenia e P-04 Osteoporose (cross-protocol dosage and bone-loading modifiers)
- [ ] **Phase 3: Infraestrutura de Segurança de Quedas** - P-07 Quedas e Síndrome Pós-Queda (balance hierarchy and session-level fall risk protocol)
- [ ] **Phase 4: Musculoesquelético Alta Dependência** - P-05 Fratura de Fêmur, P-10 ATJ, P-11 ATQ (post-op and fracture protocols)
- [ ] **Phase 5: Cluster Neuromotor** - P-03 AVC, P-06 Parkinson, P-18 Demência (neurological protocols)
- [ ] **Phase 6: Cluster Cardiorrespiratório** - P-15 DPOC e P-16 Insuficiência Cardíaca (with retroactive cardiorespiratory precautions update)
- [ ] **Phase 7: Musculoesquelético Secundário e Dor Crônica** - P-02, P-09, P-12, P-19 Lombalgia/Coluna + P-13 Ombro e P-20 Gonalgia/Coxalgia
- [ ] **Phase 8: Protocolos Especializados** - P-17 Neuropatia Periférica e P-14 Disfunção do Assoalho Pélvico + Cross-Reference Index finalizado

## Phase Details

### Phase 1: Fundação e Template
**Goal**: The Shared Foundation Layer exists and P-01 Osteoartrite is a clinically complete, validated protocol that serves as the template for all 19 subsequent protocols — locking document structure, assessment standards, dosage format, evidence grading, safety architecture, and Brazilian Portuguese tool citations.
**Depends on**: Nothing (first phase)
**Requirements**: STRUC-01, STRUC-02, STRUC-03, STRUC-04, STRUC-05, ASMNT-01, ASMNT-02, ASMNT-03, ASMNT-04, DOSE-01, DOSE-02, DOSE-03, DOSE-04, EVID-01, EVID-02, EVID-03, SAFE-01, SAFE-02, SAFE-03, SAFE-04, OUT-01, OUT-02, OUT-03, OUT-04, PROT-01
**Success Criteria** (what must be TRUE):
  1. A Shared Foundation Layer document exists defining: universal baseline battery (TUG, SPPB, Manual Dynamometry) with age-stratified normative values and MCIDs, progression principle ("Start low, go slow, but reach the goal"), Oxford CEBM evidence grading standard, and cross-reference index skeleton
  2. P-01 Osteoartrite is a complete TIDieR/CERT-structured document in Brazilian Portuguese with all 8 clinical validity questions answered unambiguously (who qualifies, when to stop, where to start, what to do, how much, how fast, how to measure progress, why these choices)
  3. The two-column dosage format (recommended value + acceptable clinical range) with frailty-stratified tables (Robust / Pre-frail / Frail) is operational and verified in P-01
  4. All outcome tools cited in their Brazilian Portuguese validated versions (SPPB-BR, WOMAC-BR, MoCA-BR, ODI-BR) with validation citations confirmed
  5. P-01 can be handed to a clinician who then knows exactly which patients qualify, what to prescribe, how to progress them, and when to escalate — without needing any other document
**Plans**: 2 plans

Plans:
- [x] 01-01: Shared Foundation Layer — universal battery, progression principle, evidence grading standard, cross-reference index skeleton, Brazilian PT tool validation citations — COMPLETED 2026-03-12 (commit 0add8ff)
- [ ] 01-02: P-01 Osteoartrite — complete protocol research (English) and document authorship (Brazilian Portuguese) following TIDieR/CERT with all structural, assessment, dosage, evidence, and safety requirements

### Phase 2: Modificadores Transversais
**Goal**: P-08 Sarcopenia and P-04 Osteoporose exist as complete reference protocols, providing the resistance dosing modifier table and bone-loading constraint set that all later protocols cross-reference rather than independently derive.
**Depends on**: Phase 1
**Requirements**: PROT-02, PROT-03
**Success Criteria** (what must be TRUE):
  1. P-08 Sarcopenia includes a frailty-stratified resistance training dosage table (referencing EWGSOP2 criteria) that any subsequent protocol can cite as the authoritative geriatric resistance dosing modifier
  2. P-04 Osteoporose includes explicit bone-loading constraint thresholds (impact, compression, torsion limits by BMD category) that govern all fracture, arthroplasty, and vertebral protocols
  3. Both protocols are self-contained, TIDieR/CERT compliant, fully in Brazilian Portuguese, and inherit all Phase 1 template standards without deviation
**Plans**: TBD

Plans:
- [ ] 02-01: P-08 Sarcopenia — research and complete protocol with EWGSOP2-anchored resistance dosing table and polypharmacy interaction section (protein-exercise coordination, dietitian referral pathway)
- [ ] 02-02: P-04 Osteoporose — research and complete protocol with bone-loading constraint set by BMD category, long-term HEP adherence strategies, and cross-reference to P-08 resistance dosing

### Phase 3: Infraestrutura de Segurança de Quedas
**Goal**: P-07 Quedas e Síndrome Pós-Queda exists as a complete reference protocol, delivering the balance intervention hierarchy (static → dynamic → dual-task → perturbation training) and the session-level fall risk protocol that must appear in all subsequent protocols.
**Depends on**: Phase 2
**Requirements**: PROT-04
**Success Criteria** (what must be TRUE):
  1. P-07 includes the balance intervention hierarchy with objective entry criteria for each level, referenced by all neuromotor and frailty protocols in Phases 4–8
  2. The session-level fall risk protocol (pre-session fatigue VAS, orthostatic BP check, gait belt criteria by TUG score, supervised exit protocol) is fully defined in P-07 and formatted as a reusable section template
  3. P-07 is self-contained, TIDieR/CERT compliant, fully in Brazilian Portuguese, and inherits all Phase 1 template standards
**Plans**: TBD

Plans:
- [ ] 03-01: P-07 Quedas e Síndrome Pós-Queda — research and complete protocol with balance hierarchy, kinesiophobia screening (Tampa Scale), session fall risk protocol template, and red flag escalation table

### Phase 4: Musculoesquelético Alta Dependência
**Goal**: P-05 Fratura de Fêmur Proximal, P-10 ATJ, and P-11 ATQ are complete protocols — the three highest-dependency musculoskeletal protocols, requiring all Phase 1–3 outputs (OA template, bone-loading constraints from Osteoporose, fall risk from Quedas, sarcopenia dosing from P-08) to be available before drafting.
**Depends on**: Phase 3
**Requirements**: PROT-05, PROT-06, PROT-07
**Success Criteria** (what must be TRUE):
  1. P-05 specifies frailty assessment (CFS at admission) as mandatory, includes VTE prophylaxis protocol awareness, and addresses post-hip-fracture fall risk with direct references to the P-07 session fall risk protocol
  2. P-10 and P-11 are explicitly differentiated (scope statements prevent overlap), each specifying surgical approach-specific precaution sets (P-11: posterior vs. anterior hip precautions; P-10: compartment syndrome and stiffness prevention) and post-operative weight-bearing progression criteria
  3. All three protocols populate their comorbidity interaction sections from Phase 2–3 reference documents rather than re-deriving shared knowledge
**Plans**: TBD

Plans:
- [ ] 04-01: P-05 Fratura de Fêmur Proximal — research and complete protocol with frailty-mandatory CFS, VTE awareness, and P-07 fall risk integration
- [ ] 04-02: P-10 ATJ + P-11 ATQ — differentiation analysis first, then both protocols drafted in parallel to enforce structural consistency; approach-specific precaution sets for ATQ

### Phase 5: Cluster Neuromotor
**Goal**: P-03 AVC, P-06 Parkinson, and P-18 Demência are complete protocols, delivering the neuromotor cluster including dual-task training sub-category template and cognitively-adapted instruction approach — drafted in sequence (P-03 first, then P-06, then P-18) to respect neuroplasticity knowledge dependencies within the cluster.
**Depends on**: Phase 4
**Requirements**: PROT-08, PROT-09, PROT-10
**Success Criteria** (what must be TRUE):
  1. P-03 AVC includes neuroplasticity-grounded phase progression, aphasia/apraxia instruction adaptations, and the dual-task training template usable by P-06 and P-18
  2. P-06 Parkinson specifies levodopa timing (session scheduling 45–60 min post-dose), "on/off" state exercise response differentiation, and caregiver training as a formal protocol component
  3. P-18 Demência uses procedural/implicit learning instruction design for all exercises, mandates MMSE or MoCA at baseline with cognitive-stratified instruction complexity, limits HEP to 2–3 exercises with pictographic sheets for MMSE <24, and integrates PAINAD/Abbey Pain Scale alongside self-report
**Plans**: TBD

Plans:
- [ ] 05-01: P-03 AVC — research and complete protocol with neuroplasticity evidence, aphasia/apraxia adaptations, dual-task training template
- [ ] 05-02: P-06 Parkinson + P-18 Demência — research and complete both protocols sequentially; P-06 with levodopa timing specification; P-18 with full cognitive-adaptation design and caregiver training section

### Phase 6: Cluster Cardiorrespiratório
**Goal**: P-15 DPOC and P-16 Insuficiência Cardíaca are complete protocols, and the universal Cardiorespiratory Precautions section template (SpO2 monitoring, pre-session vitals protocol, session suspension criteria) has been retroactively added to all 10 protocols completed in Phases 1–5.
**Depends on**: Phase 5
**Requirements**: PROT-11, PROT-12
**Success Criteria** (what must be TRUE):
  1. P-15 DPOC includes mandatory SpO2 monitoring with exercise start/stop decision cut-offs and the 6MWT as primary outcome tool, referencing ATS/ERS guidelines
  2. P-16 Insuficiência Cardíaca uses RPE-only intensity monitoring (acknowledging beta-blocker HR confound), includes daily weight monitoring with cardiology coordination pathway, and thermoregulatory impairment guidance
  3. All 10 previously completed protocols (Phases 1–5) have received the universal Cardiorespiratory Precautions section, verified and documented as a retroactive update pass
**Plans**: TBD

Plans:
- [ ] 06-01: P-15 DPOC + P-16 Insuficiência Cardíaca — research and complete both protocols sequentially; draft universal Cardiorespiratory Precautions section template from P-15 work
- [ ] 06-02: Retroactive Cardiorespiratory Precautions update — add universal section to all 10 Phase 1–5 protocols; verify consistency and document the update pass

### Phase 7: Musculoesquelético Secundário e Dor Crônica
**Goal**: Six secondary musculoskeletal and chronic pain protocols (P-02, P-09, P-12, P-19, P-13, P-20) are complete, with high-overlap pairs (P-02/P-12, P-09/P-02 derivative, P-20/P-01 derivative) explicitly differentiated before drafting begins, and the cross-protocol comorbidity flags and cross-reference index substantively populated.
**Depends on**: Phase 6
**Requirements**: PROT-13, PROT-14, PROT-15, PROT-16, PROT-17, PROT-18
**Success Criteria** (what must be TRUE):
  1. P-02 Lombalgia Crônica e Estenose de Canal and P-12 Dor Lombar Crônica Inespecífica each have explicit scope statements differentiating their patient populations, diagnostic criteria, and management approaches — with no substantive content duplication between them
  2. All six protocols include Pain Neuroscience Education (PNE) components and central sensitization screening (CSI) where clinically indicated, with time-contingent progression and psychosocial flags
  3. The cross-reference index reflects all 16 protocols now complete and documents known comorbidity interaction pathways (e.g., Lombalgia ↔ Osteoporose, Ombro ↔ ATQ, Gonalgia ↔ Artrose)
**Plans**: TBD

Plans:
- [ ] 07-01: P-02/P-12 differentiation analysis + P-02 Lombalgia Crônica + P-09 Espondilose — differentiation first, then protocols in dependency order
- [ ] 07-02: P-12 Dor Lombar Inespecífica + P-19 Fraturas Vertebrais — complete with PNE components and osteoporosis cross-reference
- [ ] 07-03: P-13 Síndrome do Ombro Doloroso + P-20 Gonalgia/Coxalgia Degenerativa — complete both; update cross-reference index to reflect all 16 protocols

### Phase 8: Protocolos Especializados
**Goal**: P-17 Neuropatia Periférica Diabética and P-14 Disfunção do Assoalho Pélvico are complete, the Cross-Reference Index is finalized covering all 20 protocols, and the corpus is clinically coherent as a complete reference system.
**Depends on**: Phase 7
**Requirements**: PROT-19, PROT-20
**Success Criteria** (what must be TRUE):
  1. P-17 Neuropatia Periférica includes mandatory pre-session glucose check protocol, sensory-loss-adapted balance exercises referencing the P-07 fall risk hierarchy, and a sensory re-education progression hierarchy appropriate for the neuropathic population
  2. P-14 Disfunção do Assoalho Pélvico distinguishes hyper vs. hypo tone through functional assessment as the mandatory first step before any exercise type selection, with ICIQ-SF cited in its Brazilian Portuguese validated version
  3. The Cross-Reference Index covers all 20 protocols — mapping comorbidity interaction pathways, shared assessment tools, cross-protocol dosage modifiers (sarcopenia, osteoporosis, falls), and high-overlap protocol differentiation — forming a usable navigation system for multi-morbid patient management
**Plans**: TBD

Plans:
- [ ] 08-01: P-17 Neuropatia Periférica Diabética — research and complete protocol with glucose monitoring, sensory-loss balance adaptation, and sensory re-education hierarchy
- [ ] 08-02: P-14 Disfunção do Assoalho Pélvico — research and complete protocol with hyper/hypo tone differentiation and ICIQ-SF-BR validation
- [ ] 08-03: Cross-Reference Index finalization — complete all 20-protocol interaction matrix, comorbidity flags, and shared tool mapping

## Progress

**Execution Order:**
Phases execute in strict sequential order: 1 → 2 → 3 → 4 → 5 → 6 → 7 → 8

| Phase | Plans Complete | Status | Completed |
|-------|----------------|--------|-----------|
| 1. Fundação e Template | 1/2 | In progress | 01-01 done 2026-03-12 |
| 2. Modificadores Transversais | 0/2 | Not started | - |
| 3. Infraestrutura de Segurança de Quedas | 0/1 | Not started | - |
| 4. Musculoesquelético Alta Dependência | 0/2 | Not started | - |
| 5. Cluster Neuromotor | 0/2 | Not started | - |
| 6. Cluster Cardiorrespiratório | 0/2 | Not started | - |
| 7. Musculoesquelético Secundário e Dor Crônica | 0/3 | Not started | - |
| 8. Protocolos Especializados | 0/3 | Not started | - |
