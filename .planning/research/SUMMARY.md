# Project Research Summary

**Project:** Protocolos de Reabilitação Geriátrica Baseados em Evidências
**Domain:** Clinical Protocol Documentation — Geriatric Physical Therapy (20 Comorbidities)
**Researched:** 2026-03-12
**Confidence:** MEDIUM (training knowledge, cutoff August 2025; web verification unavailable)

---

## Executive Summary

This project is a clinical protocol corpus — 20 individually complete, evidence-based rehabilitation documents for geriatric patients, organized around a standardized internal structure and a shared dependency graph. It is not a software project; the "architecture" is document architecture and a knowledge organization system. The correct mental model is a structured reference system where earlier protocols generate reusable knowledge blocks (templates, assessment standards, progression rules) consumed by later protocols. Expert organizations building similar corpora (WHO, APTA, NICE) uniformly ground them in TIDieR/CERT reporting standards, ICF outcome domains, and Oxford CEBM evidence grading — all of which are well-established and should be adopted here from Protocol 1 onward.

The recommended approach is to front-load foundation protocols in a strict dependency order: Osteoarthritis first (widest evidence base, establishes the template), then Sarcopenia (modifies resistance dosing in every subsequent protocol), then Osteoporosis (governs all fracture and arthroplasty protocols), then Falls Syndrome (balance intervention hierarchy used by all neuromotor protocols). This sequencing is not stylistic — it is determined by clinical knowledge dependencies, and deviating from it means later protocols must re-derive shared knowledge or produce inconsistencies. The three-layer progression architecture ("Start low, go slow, but reach the goal" operationalized as entry threshold + two-column dosing parameter block + objective phase exit criteria) should be established in Protocol 1 and applied uniformly across all 20.

The critical risks in this project are geriatric-specific and well-documented: applying adult dosage without age and frailty stratification is the most dangerous failure mode, followed by ignoring polypharmacy interactions with exercise physiology, and treating frailty as binary rather than a spectrum. These are not edge cases — they describe the majority of patients in the target population. Structural risks include template drift across 20 protocols (requires strict enforcement from Protocol 1), high-overlap protocol pairs (P-02/P-12 Lombalgia, P-10/P-11 arthroplasty) that need explicit differentiation before drafting, and outcome tools requiring Brazilian Portuguese-validated versions rather than generic translations.

---

## Key Findings

### Recommended Stack

This project's "stack" is a set of authoritative clinical and methodological resources, not software. The evidence infrastructure requires PubMed and Cochrane Library as co-primary evidence databases, supplemented by PEDro for physiotherapy-specific trials. Brazilian and Latin American context is covered by LILACS and BVS/Biblioteca Virtual em Saúde. Evidence grading should use Oxford CEBM (1a–5 scale, maps to Level A–E) as the primary system with GRADE (High/Moderate/Low/Very Low) reported alongside any Cochrane or WHO citation — these two systems are complementary, not alternatives.

All 20 protocols must use TUG, SPPB, and Manual Dynamometry as universal baseline assessment tools (non-negotiable, mandatory per PROJECT.md and confirmed by EWGSOP2 sarcopenia criteria, which directly reference all three). Frailty staging uses Fried Phenotype + Clinical Frailty Scale in combination (community and hospital coverage respectively). The protocol reporting standard is TIDieR, extended by CERT for all exercise interventions. AGREE II governs the document quality standard if any protocol targets academic publication. The ICF framework structures all outcome measurement by domain: Body Functions/Structures, Activities, Participation.

**Core resources:**

- **PubMed + Cochrane Library:** Co-primary evidence databases — comprehensive coverage, gold standard for Level A evidence search
- **PEDro:** Specialist rehabilitation database — indexes only RCTs and systematic reviews; includes PEDro scale quality scores per record
- **LILACS + BVS:** Brazilian/Latin American clinical literature — bridges international evidence to local context
- **IASP + AGS + WHO ICOPE:** Tier 1 guideline bodies (explicitly mandated by PROJECT.md) — authoritative on pain, geriatric care, and functional decline respectively
- **Oxford CEBM + GRADE:** Evidence grading — CEBM for study-level classification; GRADE for body-of-evidence certainty ratings in Cochrane/WHO citations
- **EWGSOP2:** Sarcopenia diagnostic criteria — links directly to mandatory TUG, SPPB, dynamometry baseline tools
- **TIDieR + CERT:** Protocol reporting standards — ensures reproducibility; CERT adds 16 exercise-specific items absent from basic FITT tables
- **ICF (WHO):** Outcome framework — organizes outcomes by Body Functions, Activities, Participation; maps to the 3-phase clinical structure
- **ACSM FITT-VP (Older Adults):** Exercise dosage framework — provides "start low, go slow" geriatric intensity anchors; validates protocol design philosophy

### Expected Features

See `.planning/research/FEATURES.md` for the full dependency tree. Summary:

**Must have (table stakes — absence makes protocol clinically invalid):**
- Diagnostic and inclusion criteria — the entry gate; clinicians must know exactly who qualifies
- Contraindications, precautions, and red flags — patient safety baseline; legal and ethical minimum
- Universal baseline assessments (TUG, SPPB, Manual Dynamometry) with age-stratified normative values and MCIDs
- Clinical phase structure with function-based (not time-based) entry and exit criteria
- Prescriptive exercise parameters in two-column format: recommended value + acceptable clinical range
- Progression criteria (within-phase and phase-advancement), objective and measurable
- Intervention classification by modality: Therapeutic Modality / Manual Therapy / Kinesiotherapy
- Primary outcome indicators per phase with re-evaluation schedule
- Evidence level classification per intervention (Level A/B/C with primary citation)
- Guideline alignment declaration (IASP, AGS, WHO, or condition-specific equivalent)
- "Start low, go slow, but reach the goal" principle embedded across all parameter and progression content

**Should have (differentiators — elevate protocol quality and safety):**
- Pain monitoring integration with NRS thresholds per phase (IASP alignment; high safety value)
- Structured red flag table with escalation pathways — maps warning signs to specific responses
- Functional benchmark targets at phase transitions — objective, tool-anchored advancement criteria
- Intra-session structure template (warm-up / main / cool-down with phase-specific intensity)
- Home exercise program (HEP) template with adherence structure (not just exercise list)
- Polypharmacy interaction section per protocol (most common drug classes + exercise implications)
- Cardiorespiratory precautions section in every protocol regardless of primary diagnosis

**Defer to later protocols or v2:**
- Cross-protocol comorbidity flags — cannot be built until 3+ protocols exist
- Clinical decision tree / flowchart — requires phase structure finalized; build after 2-3 protocols
- Quick reference cards — build after template is stable across 2-3 protocols
- Caregiver guidance sections — prioritize for P-06 (Parkinson), P-18 (Dementia), P-03 (Stroke); not needed for OA template
- Dosage rationale annotations — high overhead; add selectively for contested or non-obvious parameters

**Clinical validity threshold:** A protocol is complete only when it answers all 8 questions without ambiguity: who is it for, when do we stop, where do we start, what do we do, how much, how fast, how do we know it's working, why these choices.

### Architecture Approach

The corpus is organized as a shared foundation layer plus 20 individually self-contained protocol documents, grouped into five clinical clusters: Musculoskeletal (11 protocols), Neuromotor/Functional Decline (5 protocols), Cardiorespiratory (2 protocols), Metabolic/Neuropathic (2 protocols), and Pelvic/Axial (2 protocols). Each protocol must be independently usable by a clinician treating a single-condition patient — cross-references add depth but are not required reading. The critical architectural decision is that phase exit criteria are always objective and function-based (never time-based alone), the universal baseline battery is supplemented but never replaced within individual protocols, and comorbidity notes reference rather than duplicate shared knowledge.

**Major components:**

1. **Shared Foundation Layer** — Universal baseline assessment battery, progression principle specification, evidence grading standard, comorbidity interaction reference table. Defined once; changes propagate to all 20 protocols. Created before any individual protocol is drafted.
2. **Individual Protocol Documents (P-01 to P-20)** — 8-section TIDieR/CERT-structured clinical documents. Each is self-contained. Phase count varies by condition (2-4). The atomic decision-making unit is the Phase Block (entry criteria + two-column dosing + progression rules + exit criteria).
3. **Cross-Reference Index** — Maps which protocols interact, which tools are shared, which conditions modify others. Maintained as standalone appendix. Critical for multi-morbid patients (80%+ of geriatric rehabilitation caseload).

### Critical Pitfalls

See `.planning/research/PITFALLS.md` for the full 16-pitfall registry with phase-by-phase warning tables. Top 5:

1. **Age-agnostic dosage prescription** — Copying adult RCT headline dosages to geriatric protocols without age/frailty adjustment. Prevention: trace every dosage to source study population (mean age, frailty status); use RPE (Borg 11-13 Acute, 13-15 Subacute, 15-17 max Advanced) alongside absolute cutoffs; cross-reference ACSM Older Adult guidelines for every parameter.

2. **Frailty treated as binary** — Protocols without frailty stratification are unauditable and clinically dangerous for the actual population range. Prevention: mandate Fried Phenotype or CFS alongside TUG/SPPB/Dynamometry at baseline; provide frailty-stratified dosage columns (Robust / Pre-frail / Frail); tie phase-advancement criteria to frailty score.

3. **Polypharmacy interactions ignored** — Beta-blockers invalidate HR-based intensity monitoring; antihypertensives + diuretics create orthostatic hypotension risk; anticoagulants require documented fall-event protocol. Prevention: include Polypharmacy Interaction section in every protocol; mandate pre/post-session BP check; reference AGS Beers Criteria 2023.

4. **Exercise-induced falls during the protocol itself** — Balance and gait training operates at stability limits; post-exercise fatigue window (2-4 hours post-session) is rarely addressed. Prevention: session-level fall risk protocol including pre-session fatigue VAS, orthostatic BP check, gait belt criteria by TUG score, supervised exit protocol.

5. **Cognitive barriers to protocol compliance** — MCI and early dementia are prevalent in 75+ populations; RCTs exclude MMSE <24 patients, then practitioners apply findings to the excluded population. Prevention: mandate MMSE or MoCA at baseline; stratify instruction complexity by cognitive score; for MMSE <24, limit HEP to 2-3 exercises max with pictographic sheets; use PAINAD/Abbey Pain Scale alongside self-report for moderate-to-severe dementia.

---

## Implications for Roadmap

Build order is driven by clinical knowledge dependencies, not convenience. The dependency graph is explicit in ARCHITECTURE.md and confirmed by FEATURES.md feature dependency tree. Deviating from this order means later protocols must re-derive shared knowledge or will contain inconsistencies that require retroactive revision.

### Phase 1: Shared Foundation and Template Protocol (P-01 Osteoarthritis)

**Rationale:** Before any individual protocol is drafted, the shared foundation layer must exist. Without it, each of the 20 protocols will independently re-derive the same baseline assessment rationale, progression principle, and evidence standards — creating inconsistency and maintenance overhead across 20 documents. Osteoarthritis is the correct first protocol because it has the broadest, most mature evidence base, and the clinical logic it establishes (kinesiotherapy progressions, manual therapy framework, WOMAC usage, joint-loading principles) is directly consumed by 6+ later protocols.

**Delivers:** Shared Foundation Layer document + P-01 as the validated template for all subsequent protocols. By the end of this phase, the two-column dosing format, TIDieR/CERT document structure, evidence grading conventions, Brazilian Portuguese tool versions, and MCID anchors are all established and tested.

**Addresses (from FEATURES.md):** All 11 table-stakes features must be present in P-01. Pain monitoring integration (NRS thresholds per phase) and structured red flag table are worth including at this stage despite being differentiators — they are high safety value and medium effort, and establishing them in the template costs little once the structure is designed.

**Avoids (from PITFALLS.md):** Age-agnostic dosage (establish geriatric-specific ranges from first protocol), frailty binary treatment (design stratified dosage columns in the template), outcome measures without MCIDs (document all MCIDs in P-01 template), Brazilian Portuguese tool version confusion (verify SPPB-BR, WOMAC-BR, MoCA-BR citations in P-01).

**Research flag:** Needs deeper per-condition literature research during planning. OARSI 2024 update status should be verified (in-progress as of late 2024). Central sensitization screening (PCS, CSI) should be included from the start given the chronic pain pitfall.

### Phase 2: Sarcopenia and Osteoporosis — Cross-Protocol Modifiers

**Rationale:** P-08 (Sarcopenia) and P-04 (Osteoporosis) are not standalone protocols in terms of downstream influence — they are system-level modifiers. Sarcopenia criteria (EWGSOP2) affect resistance training dosing in all 20 protocols. Osteoporosis bone stress thresholds govern all fracture, arthroplasty, and vertebral protocols. These must be defined before any of the protocols they modify can be drafted with confidence.

**Delivers:** P-08 and P-04 as reference documents. After this phase, the author has a sarcopenia dosing table and bone-loading constraint set that all later protocols can cross-reference rather than derive.

**Addresses (from FEATURES.md):** Cross-protocol comorbidity flags become first usable here (3 protocols now exist). Polypharmacy interaction section is especially important for P-08 (protein-exercise coordination, dietitian referral pathway).

**Avoids (from PITFALLS.md):** Adult dosage applied to sarcopenic patients (P-08 directly solves this), impact loading without BMD data (P-04 defines this boundary), HEP adherence for long-term bone remodeling (P-04 requires behavioral adherence strategies).

**Research flag:** EWGSOP3 revision status should be confirmed (discussed in literature; current standard is EWGSOP2). Resistance training dosage ranges for sarcopenia should be verified against current Cochrane reviews.

### Phase 3: Falls Syndrome — Cross-Cutting Safety Infrastructure

**Rationale:** P-07 (Quedas / Síndrome Pós-Queda) establishes the balance intervention hierarchy (static → dynamic → dual-task → perturbation training) and fall risk stratification tools referenced by all neuromotor and frailty protocols. This phase logically follows Sarcopenia and Osteoporosis because fall risk stratification is meaningless without the muscle strength and bone quality frameworks already defined.

**Delivers:** P-07 as the balance/falls reference document. Also: the session-level fall risk protocol (pre-session fatigue VAS, orthostatic BP check, gait belt criteria, post-session supervised exit) that must appear as a section in all subsequent protocols.

**Addresses (from FEATURES.md):** Structured red flag table with escalation pathways is mandatory here. Kinesiophobia screening (Tampa Scale) should be included given the fear-of-movement dynamic in falls population.

**Avoids (from PITFALLS.md):** Exercise-induced falls during the protocol (Pitfall 4 — this protocol directly operationalizes the prevention strategy), exercise-induced fall post-session window (must appear in session structure).

**Research flag:** Standard patterns (Cochrane review by Sherrington on exercise and falls prevention is well-established). Minimal additional research needed beyond verifying current systematic review landscape.

### Phase 4: High-Dependency Musculoskeletal Protocols (P-05, P-10, P-11)

**Rationale:** Proximal Femur Fracture (P-05), Total Knee Arthroplasty (P-10), and Total Hip Arthroplasty (P-11) all depend on P-01 (OA), P-04 (Osteoporosis), P-07 (Falls), and P-08 (Sarcopenia) — all now available. The arthroplasty pair (P-10, P-11) are architecturally twinned and should be drafted together to enforce consistency.

**Delivers:** Three high-complexity musculoskeletal protocols with full comorbidity interaction sections populated from Phase 2-3 reference documents.

**Avoids (from PITFALLS.md):** DVT/PE risk window in post-op protocols (must include VTE prophylaxis protocol awareness); hip precaution specification by surgical approach (posterior vs. anterior — must coordinate with surgeon); frailty underestimation in hip fracture (CFS at admission is mandatory); exercise-induced falls during rehabilitation.

**Research flag:** Phase 4 needs deeper research during planning. Post-arthroplasty weight-bearing progression criteria, surgical approach-specific precaution sets, and cardiac comorbidity interaction are protocol-specific research needs. ATJ and ATQ may need 4 phases (Pós-operatório Imediato is clinically distinct).

### Phase 5: Neuromotor Cluster (P-03, P-06, P-18)

**Rationale:** Stroke (P-03), Parkinson's (P-06), and Dementia (P-18) all depend on the Falls framework (P-07) and the neuroplasticity principles established in P-03. P-06 depends on P-03; P-18 depends on both. Draft in sequence within this phase.

**Delivers:** Three neurological protocols. This phase also delivers the dual-task training sub-category template (motor + cognitive simultaneously) and the procedural/implicit learning instruction approach for cognitively impaired patients.

**Avoids (from PITFALLS.md):** Cognitive barriers to compliance (Pitfall 5 — Dementia is the primary case; design all exercises as procedural, mandate caregiver training, use PAINAD/Abbey alongside self-report); levodopa timing specification in P-06 (schedule sessions 45-60 min post-dose); aphasia/apraxia instruction adaptations in P-03.

**Research flag:** Needs deeper research during planning. Neuroplasticity windows in chronic stroke, Parkinson's-specific exercise response during "on" vs. "off" states, and dementia-adapted instruction design are specialized domains with active research. Caregiver training as a formal protocol component needs specific evidence sourcing.

### Phase 6: Cardiorespiratory Cluster (P-15, P-16)

**Rationale:** DPOC and Heart Failure are relatively standalone from the musculoskeletal protocols but generate a cardiac precautions block that must flow back and be added to all previously completed protocols. Draft P-15 first (establishes exercise intensity/monitoring framework), then P-16 (extends it with cardiac-specific constraints).

**Delivers:** Two cardiorespiratory protocols. Also delivers: the universal Cardiorespiratory Precautions section template (mandatory SpO2 monitoring, pre-session vitals protocol, session suspension criteria) that retroactively supplements all 10 prior protocols.

**Avoids (from PITFALLS.md):** SpO2 monitoring absent in DPOC (Pitfall 10 — mandatory in this protocol and referenced universally); beta-blocker confound in Heart Failure (RPE-only intensity; daily weight monitoring with cardiology coordination); thermoregulatory impairment guidance.

**Research flag:** ATS/ERS 2023 Pulmonary Rehabilitation Statement final publication status should be confirmed. ESC Heart Failure Guidelines 2021/2023 cardiac rehab position should be verified.

### Phase 7: Secondary Musculoskeletal and Chronic Pain Protocols (P-02, P-09, P-12, P-19, P-13, P-20)

**Rationale:** These protocols depend heavily on P-01, P-04, and the Cardiorespiratory precautions block. The high-overlap pairs (P-02/P-12 Lombalgia; P-09 Spondylosis as P-02 derivative; P-20 Gonalgia/Coxalgia as P-01 derivative) must be explicitly differentiated before drafting begins. Merging without differentiation is the primary structural risk in this phase.

**Delivers:** Six secondary musculoskeletal and chronic pain protocols. This phase also matures the cross-protocol comorbidity flags and cross-reference index (now 16 protocols exist).

**Avoids (from PITFALLS.md):** Protocol isolation — by this point the comorbidity interaction cross-reference matrix should be fully populated; central sensitization treated biomechanically (Pitfalls 9 — chronic pain protocols P-02, P-12 must include PNE component, time-contingent progression, CSI screening); merging high-overlap protocols without differentiation (Pitfall S6 — explicit differentiation required before drafting P-12 vs. P-02).

**Research flag:** P-02 and P-12 explicitly need differentiation research. If the clinical management difference is only pathological classification, P-12 may be a section within P-02.

### Phase 8: Specialized Protocols (P-17, P-14, P-08 variant if needed)

**Rationale:** Peripheral Neuropathy (P-17) and Pelvic Floor (P-14) are relatively standalone with specialized domain knowledge requirements. P-17 depends on P-07 (falls — neuropathy is a major falls risk factor) and P-08 (sarcopenia context). P-14 depends on P-12 (core overlap).

**Delivers:** Final two specialized protocols. Completion of the Cross-Reference Index and comorbidity interaction matrix.

**Avoids (from PITFALLS.md):** Hypoglycemia during exercise in P-17 (pre-session glucose check mandatory); proprioceptive deficit depth underestimated (sensory-loss-adapted balance exercises); pelvic floor overactivity vs. underactivity conflation in P-14 (functional assessment must distinguish hyper vs. hypo tone before exercise type selection); sex-specific differentiation in P-14 and P-19.

**Research flag:** Pelvic floor is a specialized domain; ICIQ-SF validation for Brazilian Portuguese should be confirmed. Neuropathy sensory re-education hierarchy may need 4 phases (distinct early sensory phase).

---

### Phase Ordering Rationale

- **Foundation-first is mandatory:** The Shared Foundation Layer and P-01 template must exist before any subsequent protocol, because all 20 share the same baseline assessment battery, evidence grading convention, progression architecture, and document structure. Retroactive template enforcement across 20 documents is high-cost.
- **Dependency graph drives sequence:** P-08 (Sarcopenia) modifies ALL others; P-04 (Osteoporosis) governs all fracture/arthroplasty; P-07 (Falls) is required by all neuromotor protocols. These are not editorial preferences — they are clinical knowledge dependencies.
- **High-overlap pairs must be differentiated before drafting:** The P-02/P-12 Lombalgia pair and the P-10/P-11 arthroplasty pair require explicit scope differentiation before any text is written. Otherwise one protocol will be a near-duplicate of the other, which creates confusion and maintenance burden without adding clinical value.
- **Cardiorespiratory precautions block flows backward:** When Phase 6 is complete, the universal Cardiorespiratory Precautions section must be retrofitted into all 10 preceding protocols. Plan for this revision pass.
- **Cross-protocol comorbidity flags mature late by design:** They cannot be fully populated until enough protocols exist to cross-reference. The Cross-Reference Index should be started in Phase 1 but completed incrementally.

### Research Flags

Phases needing deeper literature research during planning:

- **Phase 1 (P-01 OA):** Verify OARSI 2024 update publication status; confirm WOMAC-BR and SPPB-BR Brazilian Portuguese validation citations; confirm central sensitization screening tools (PCS, CSI) inclusion rationale.
- **Phase 4 (P-05, P-10, P-11):** Post-arthroplasty weight-bearing progression criteria (highly protocol- and surgeon-specific); surgical approach-specific hip precaution sets; cardiac comorbidity interaction thresholds.
- **Phase 5 (P-03, P-06, P-18):** Neuroplasticity evidence in chronic stroke; levodopa-exercise timing RCT literature; dementia-adapted implicit learning instruction design; PAINAD/Abbey Pain Scale Brazilian Portuguese versions.
- **Phase 6 (P-15, P-16):** ATS/ERS 2023 Pulmonary Rehab Statement final status; ESC 2023 cardiac rehab updates; SpO2 monitoring cut-offs for exercise start/stop decisions.
- **Phase 7 (P-02 vs. P-12 scope):** Requires explicit differentiation research before any text is drafted. If clinical management is essentially identical, P-12 becomes a variant section within P-02.

Phases with standard patterns (research-phase can be skipped or abbreviated):

- **Phase 2 (P-08 Sarcopenia, P-04 Osteoporosis):** EWGSOP2 and IOF/NOF guidelines are well-established and stable. Verify EWGSOP3 status but expect EWGSOP2 remains current standard.
- **Phase 3 (P-07 Falls):** Cochrane review by Sherrington on exercise and falls prevention is well-documented. Standard balance intervention hierarchy is established.
- **Phase 8 (P-14 Pelvic Floor):** Well-defined domain with clear hyper/hypo tone differentiation. Main research need is confirming ICIQ-SF Brazilian Portuguese validation.

---

## Confidence Assessment

| Area | Confidence | Notes |
|------|------------|-------|
| Stack (evidence resources and standards) | HIGH | PubMed, Cochrane, PEDro, TIDieR, CERT, Oxford CEBM, ICF, ACSM — all are established, stable, internationally endorsed frameworks with decades of use |
| Features (protocol content requirements) | HIGH | Table stakes reflect decades of clinical guideline development consensus; stable knowledge. Differentiator implementation details benefit from current literature verification during execution |
| Architecture (document structure and build order) | MEDIUM-HIGH | Template structure reflects APTA CPG, WHO Rehabilitation, and Cochrane report standards (HIGH). Build order within tiers is a judgment call (MEDIUM) but tier groupings are HIGH confidence |
| Pitfalls (risk identification) | MEDIUM | Pitfalls reflect established clinical consensus and published geriatric rehabilitation literature. Specific mitigation thresholds (e.g., exact MCIDs, specific polypharmacy cut-offs) should be verified against current guidelines during each protocol's research phase |

**Overall confidence:** MEDIUM-HIGH

The evidence frameworks, document architecture, and phase structure are well-grounded. The primary uncertainty is not about whether the approach is correct, but about whether specific parameter values and recent guideline updates (OARSI 2024, EWGSOP3, ATS/ERS 2023) have changed since training cutoff. This is a verification gap, not a conceptual gap.

### Gaps to Address

- **OARSI 2024 guideline update:** In-progress as of late 2024. Verify final publication at oarsi.org before completing P-01 and P-20. If published, it supersedes 2019 guidance on OA management.
- **EWGSOP3 status:** Discussed in literature; confirm whether EWGSOP2 (2018) remains current standard or has been superseded. Verify at myespen.eu before completing P-08.
- **MoCA-BR normative data:** Confirm most current Brazilian Portuguese normative data and validation status before using in protocols where cognitive screening is primary (P-18, P-06).
- **Brazilian Portuguese tool validation citations:** Before finalizing P-01 template, confirm validation citations for: SPPB-BR (Nakano 2007 — likely still current), WOMAC-BR, MoCA-BR, SF-36 Brazil, PDQ-39 Brazil, ODI-BR. Using a non-Brazilian Portuguese version introduces measurement error and invalidates comparison with Brazilian clinical literature.
- **AGS Beers Criteria edition:** 2023 version was current at knowledge cutoff. Confirm 2026 status given 3-year update cycle.
- **ATS/ERS 2023 Pulmonary Rehabilitation Statement:** Confirm final publication and whether it has been updated since 2023.
- **Web access for real-time verification:** All four research agents worked from training knowledge; no live database access was available. Before beginning any protocol draft, run searches on PubMed and Cochrane for current systematic reviews in that condition category.

---

## Sources

### Primary (HIGH confidence)

- Oxford Centre for Evidence-Based Medicine — Levels of Evidence (2011): cebm.ox.ac.uk/resources/levels-of-evidence
- WHO ICF: who.int/standards/classifications/international-classification-of-functioning-disability-and-health
- TIDieR Checklist: tidierguide.org
- CERT (Consensus on Exercise Reporting Template): certreportingtool.weebly.com
- AGREE II: agreetrust.org
- Cruz-Jentoft AJ et al. (2019). Sarcopenia: revised European consensus (EWGSOP2). Age and Ageing.
- Fried LP et al. (2001). Frailty in older adults. J Gerontol A Biol Sci Med Sci.
- ACSM Guidelines for Exercise Testing and Prescription, 11th ed. (2022)
- WHO ICOPE Implementation Framework (2019)
- PEDro Database: pedro.org.au
- Cochrane Library: cochranelibrary.com
- PubMed: pubmed.ncbi.nlm.nih.gov

### Secondary (MEDIUM confidence)

- AGS Clinical Practice Guidelines and Beers Criteria 2023: americangeriatrics.org
- IASP Chronic Pain in Older Adults Guidelines: iasp-pain.org
- OARSI Clinical Practice Guidelines (2019; 2024 update status unconfirmed): oarsi.org
- ATS/ERS Pulmonary Rehabilitation Statement (2023 final status unconfirmed): thoracic.org
- ESC Heart Failure Guidelines 2021/2023: escardio.org
- MDS Evidence-based medicine review (Parkinson's): movementdisorders.org
- APTA Clinical Practice Guidelines (multiple conditions): apta.org/patient-care/clinical-practice-guidelines
- SIGN Guidelines (stroke, falls, dementia): sign.ac.uk
- Nakano MM et al. (2007). SPPB Brazilian validation.
- Bohannon RW — TUG normative values in older adults (multiple publications; MCID ~3.5s)
- Sherrington C et al. — Cochrane review on exercise and falls prevention
- Louw A et al. — Pain Neuroscience Education systematic reviews
- Fragala MS et al. (2019). Resistance Training for Older Adults: NSCA Position Statement. J Strength Cond Res.

### Tertiary (LOW confidence — need verification)

- EWGSOP3 status: discussed in literature; confirm at myespen.eu
- OARSI 2024 update: in-progress as of late 2024; confirm at oarsi.org
- Brazilian Portuguese validation of outcome tools beyond SPPB-BR and MoCA-BR: verify per tool before protocol use
- ACSM Older Adult Guidelines current edition number: verify current edition at acsm.org

---

*Research completed: 2026-03-12*
*Ready for roadmap: yes*
