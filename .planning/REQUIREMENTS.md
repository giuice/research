# Requirements: Protocolos de Reabilitação Geriátrica

**Defined:** 2026-03-12
**Core Value:** Every protocol must be the most efficient "Protocol #1" for its comorbidity — prioritizing clinical outcomes, patient safety, and reduction of care-related risks, grounded in Level A evidence and international guidelines.

## v1 Requirements

### Protocol Structure

- [x] **STRUC-01**: Each protocol includes diagnostic/inclusion criteria defining exactly which patients qualify — DONE 01-02 (P-01 Section 1, 2026-03-12)
- [x] **STRUC-02**: Each protocol includes contraindications, precautions, and red flags with stopping rules — DONE 01-02 (P-01 Sections 8-9, 2026-03-12)
- [x] **STRUC-03**: Each protocol uses flexible clinical phase structure (2-4 phases) with function-based entry/exit criteria — DONE 01-02 (P-01 Sections 4-7, 2026-03-12)
- [x] **STRUC-04**: Interventions classified by: Therapeutic Modality, Manual Therapy, Kinesiotherapy — DONE 01-02 (P-01 Sections 5.4, 6.4, 7.4, 2026-03-12)
- [x] **STRUC-05**: Shared Foundation Layer document created before any individual protocol (universal battery, progression principle, evidence grading standard, cross-reference index skeleton) — DONE 01-01 (2026-03-12)

### Assessment & Measurement

- [x] **ASMNT-01**: Universal baseline battery (TUG, SPPB, Manual Dynamometry) with age-stratified normative values and MCIDs in every protocol — DONE 01-01 (2026-03-12)
- [x] **ASMNT-02**: Primary outcome indicators per phase with re-evaluation schedule — DONE 01-02 (P-01 Section 12, 2026-03-12)
- [x] **ASMNT-03**: Functional benchmark targets at phase transitions (objective, tool-anchored advancement criteria) — DONE 01-02 (P-01 Sections 5.3, 6.3, 7.3, 2026-03-12)
- [x] **ASMNT-04**: All outcome tools cited in Brazilian Portuguese validated versions (SPPB-BR, WOMAC-BR, MoCA-BR, etc.) — DONE 01-01 (2026-03-12)

### Dosage & Progression

- [x] **DOSE-01**: Two-column dosage format for all exercises: recommended value + acceptable clinical range — DONE 01-01 (2026-03-12)
- [x] **DOSE-02**: "Start low, go slow, but reach the goal" principle embedded across all parameter and progression content — DONE 01-01 (2026-03-12)
- [x] **DOSE-03**: Frailty-stratified dosage tables (Robust / Pre-frail / Frail) in every protocol — DONE 01-01 (2026-03-12)
- [x] **DOSE-04**: Objective progression criteria (within-phase and phase-advancement), never time-based alone — DONE 01-02 (P-01 Sections 5.3, 6.3, 7.3, 2026-03-12)

### Evidence & Safety

- [x] **EVID-01**: Evidence level classification per intervention (Oxford CEBM Level A/B/C with primary citation) — DONE 01-01 (2026-03-12)
- [x] **EVID-02**: Guideline alignment declaration (IASP, AGS, WHO, and condition-specific body) in every protocol — DONE 01-01 (2026-03-12)
- [x] **EVID-03**: Research conducted in English from PubMed + Cochrane + PEDro triad — DONE 01-01 (2026-03-12)
- [x] **SAFE-01**: Pain monitoring with NRS thresholds per phase (IASP-aligned) — DONE 01-01 (2026-03-12)
- [x] **SAFE-02**: Structured red flag table with escalation pathways per protocol — DONE 01-01 (2026-03-12)
- [x] **SAFE-03**: Polypharmacy interaction section per protocol (most common drug classes + exercise implications) — DONE 01-01 (2026-03-12)
- [x] **SAFE-04**: Cardiorespiratory precautions section in every protocol regardless of primary diagnosis — DONE 01-01 (2026-03-12)

### Output

- [x] **OUT-01**: Final protocols written in Brazilian Portuguese — DONE 01-02 (P-01 entirely in BP, 2026-03-12)
- [x] **OUT-02**: One structured markdown document per comorbidity (20 total) — P-01 DONE 01-02; 1/20 complete (2026-03-12)
- [x] **OUT-03**: Protocols follow TIDieR/CERT reporting standards — DONE 01-02 (P-01 TIDieR/CERT compliant, 2026-03-12)
- [x] **OUT-04**: Cross-reference index mapping protocol interactions and comorbidity flags — DONE 01-01 (skeleton; to be filled progressively)

### Protocols (sequential, dependency-ordered)

- [x] **PROT-01**: P-01 Osteoartrite / Artrose (joelho, quadril, coluna, mãos) — template protocol — DONE 01-02 (2026-03-12, commits 6bc6ddd, 79fa068)
- [x] **PROT-02**: P-08 Sarcopenia / Fraqueza Generalizada — cross-protocol resistance dosing modifier
- [x] **PROT-03**: P-04 Osteoporose — cross-protocol bone-loading constraint
- [x] **PROT-04**: P-07 Quedas e Síndrome Pós-Queda — balance hierarchy + session fall risk protocol
- [x] **PROT-05**: P-05 Fratura de Fêmur Proximal / Quadril
- [x] **PROT-06**: P-10 Pós-op Artroplastia Total de Joelho (ATJ)
- [x] **PROT-07**: P-11 Pós-op Artroplastia Total de Quadril (ATQ)
- [ ] **PROT-08**: P-03 AVC/AVE (fase crônica, neuroplasticidade)
- [ ] **PROT-09**: P-06 Doença de Parkinson
- [ ] **PROT-10**: P-18 Demência / Alzheimer (leve a moderado)
- [ ] **PROT-11**: P-15 DPOC (reabilitação respiratória)
- [ ] **PROT-12**: P-16 Insuficiência Cardíaca / Cardiopatias
- [ ] **PROT-13**: P-02 Lombalgia Crônica e Estenose de Canal
- [ ] **PROT-14**: P-09 Artrose de Coluna / Espondilose
- [ ] **PROT-15**: P-12 Dor Lombar Crônica Inespecífica
- [ ] **PROT-16**: P-19 Fraturas Vertebrais por Compressão
- [ ] **PROT-17**: P-13 Síndrome do Ombro Doloroso
- [ ] **PROT-18**: P-20 Gonalgia / Coxalgia Degenerativa
- [ ] **PROT-19**: P-17 Neuropatia Periférica (diabética)
- [ ] **PROT-20**: P-14 Disfunção do Assoalho Pélvico

## v2 Requirements

### Enhanced Content

- **V2-01**: Clinical decision tree / flowchart per protocol
- **V2-02**: Quick reference cards (1-page distillation for experienced clinicians)
- **V2-03**: Dosage rationale annotations (inline citations for each parameter choice)
- **V2-04**: Caregiver/family guidance sections (priority: P-06 Parkinson, P-18 Dementia, P-03 Stroke)
- **V2-05**: Home exercise program (HEP) templates with pictographic sheets
- **V2-06**: Intra-session structure templates (warm-up / main / cool-down per phase)
- **V2-07**: Patient education summaries in plain language (Brazilian Portuguese)
- **V2-08**: Adherence and motivation strategies specific to geriatric population

## Out of Scope

| Feature | Reason |
|---------|--------|
| Marketing or hospitality techniques | Purely clinical-therapeutic focus per PROJECT.md |
| Acute hospital care protocols | Different population state, clinical logic, and legal context |
| Surgical technique descriptions | Outside rehab scope; only post-operative rehabilitation |
| Pharmaceutical dosage recommendations | Outside physical therapy scope of practice; medico-legal risk |
| Pediatric or adult non-geriatric content | Population specificity is core to project value |
| Proprietary/trademarked techniques | Evidence-based only; describe mechanisms, not brands |
| Unvalidated or fringe modalities | Violates Level A evidence standard |
| Software/app development | This is a clinical documentation project |

## Traceability

| Requirement | Phase | Phase Name | Status |
|-------------|-------|------------|--------|
| STRUC-01 | Phase 1 | Fundação e Template | Done — 01-02 |
| STRUC-02 | Phase 1 | Fundação e Template | Done — 01-02 |
| STRUC-03 | Phase 1 | Fundação e Template | Done — 01-02 |
| STRUC-04 | Phase 1 | Fundação e Template | Done — 01-02 |
| STRUC-05 | Phase 1 | Fundação e Template | Done — 01-01 |
| ASMNT-01 | Phase 1 | Fundação e Template | Done — 01-01 |
| ASMNT-02 | Phase 1 | Fundação e Template | Done — 01-02 |
| ASMNT-03 | Phase 1 | Fundação e Template | Done — 01-02 |
| ASMNT-04 | Phase 1 | Fundação e Template | Done — 01-01 |
| DOSE-01 | Phase 1 | Fundação e Template | Done — 01-01 |
| DOSE-02 | Phase 1 | Fundação e Template | Done — 01-01 |
| DOSE-03 | Phase 1 | Fundação e Template | Done — 01-01 |
| DOSE-04 | Phase 1 | Fundação e Template | Done — 01-02 |
| EVID-01 | Phase 1 | Fundação e Template | Done — 01-01 |
| EVID-02 | Phase 1 | Fundação e Template | Done — 01-01 |
| EVID-03 | Phase 1 | Fundação e Template | Done — 01-01 |
| SAFE-01 | Phase 1 | Fundação e Template | Done — 01-01 |
| SAFE-02 | Phase 1 | Fundação e Template | Done — 01-01 |
| SAFE-03 | Phase 1 | Fundação e Template | Done — 01-01 |
| SAFE-04 | Phase 1 | Fundação e Template | Done — 01-01 |
| OUT-01 | Phase 1 | Fundação e Template | Done — 01-02 |
| OUT-02 | Phase 1 | Fundação e Template | Done — 01-02 (1/20 protocols) |
| OUT-03 | Phase 1 | Fundação e Template | Done — 01-02 |
| OUT-04 | Phase 1 | Fundação e Template | Done — 01-01 (skeleton); 01-02 (P-01 row) |
| PROT-01 | Phase 1 | Fundação e Template | Done — 01-02 |
| PROT-02 | Phase 2 | Modificadores Transversais | Done — 02 (2026-03-12) |
| PROT-03 | Phase 2 | Modificadores Transversais | Done — 02 (2026-03-12) |
| PROT-04 | Phase 3 | Infraestrutura de Segurança de Quedas | Done — 03 (2026-03-12) |
| PROT-05 | Phase 4 | Musculoesquelético Alta Dependência | Done — 04-01 (2026-03-13) |
| PROT-06 | Phase 4 | Musculoesquelético Alta Dependência | Done — 04-02 (2026-03-13) |
| PROT-07 | Phase 4 | Musculoesquelético Alta Dependência | Done — 04-02 (2026-03-13) |
| PROT-08 | Phase 5 | Cluster Neuromotor | Pending |
| PROT-09 | Phase 5 | Cluster Neuromotor | Pending |
| PROT-10 | Phase 5 | Cluster Neuromotor | Pending |
| PROT-11 | Phase 6 | Cluster Cardiorrespiratório | Pending |
| PROT-12 | Phase 6 | Cluster Cardiorrespiratório | Pending |
| PROT-13 | Phase 7 | Musculoesquelético Secundário e Dor Crônica | Pending |
| PROT-14 | Phase 7 | Musculoesquelético Secundário e Dor Crônica | Pending |
| PROT-15 | Phase 7 | Musculoesquelético Secundário e Dor Crônica | Pending |
| PROT-16 | Phase 7 | Musculoesquelético Secundário e Dor Crônica | Pending |
| PROT-17 | Phase 7 | Musculoesquelético Secundário e Dor Crônica | Pending |
| PROT-18 | Phase 7 | Musculoesquelético Secundário e Dor Crônica | Pending |
| PROT-19 | Phase 8 | Protocolos Especializados | Pending |
| PROT-20 | Phase 8 | Protocolos Especializados | Pending |

**Coverage:**
- v1 requirements: 44 total
- Mapped to phases: 44
- Unmapped: 0

---
*Requirements defined: 2026-03-12*
*Last updated: 2026-03-13 after phase 04 completion*
