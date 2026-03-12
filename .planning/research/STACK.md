# Technology Stack — Evidence-Based Geriatric Rehabilitation Protocols

**Project:** Protocolos de Reabilitação Geriátrica Baseados em Evidências
**Researched:** 2026-03-12
**Research mode:** Ecosystem (clinical/academic domain — no software stack)
**Note on sources:** WebSearch and WebFetch were unavailable in this environment.
All findings are drawn from training knowledge (cutoff August 2025) supplemented
by known official sources. Confidence levels reflect this constraint; items marked
LOW should be verified against current official documentation before use.

---

## What "Stack" Means Here

This is not a software project. The "stack" is the set of authoritative sources,
validated tools, reporting standards, and documentation frameworks that define
how evidence-based geriatric rehabilitation protocols are built, structured,
and communicated. Each layer of the stack answers a specific question:

| Stack Layer | Question Answered |
|-------------|-------------------|
| Evidence Databases | Where do I find the best studies? |
| Guideline Bodies | Whose clinical recommendations carry authority? |
| Evidence Grading Systems | How do I classify evidence quality? |
| Assessment Tools | How do I measure patient status at baseline? |
| Outcome Measurement Frameworks | How do I measure whether the protocol worked? |
| Protocol Structuring Standards | How do I format a protocol for clinical/academic use? |
| Documentation Formats | In what structure do I write the final document? |

---

## 1. Evidence Databases

### Primary (Required)

| Database | URL | Why This One | Confidence |
|----------|-----|--------------|------------|
| PubMed / MEDLINE | pubmed.ncbi.nlm.nih.gov | Comprehensive index of RCTs, systematic reviews, and meta-analyses; the starting point for any Level A evidence search in rehabilitation medicine | HIGH |
| Cochrane Library | cochranelibrary.com | Gold standard for systematic reviews and meta-analyses; Cochrane reviews are specifically cited as Level A by IASP, AGS, and WHO; essential for exercise dosage and intervention comparisons | HIGH |
| PEDro (Physiotherapy Evidence Database) | pedro.org.au | Indexes only RCTs and systematic reviews in physiotherapy; includes PEDro scale scores (methodological quality) for every record; the specialist database for rehabilitation; freely available | HIGH |
| CINAHL | ebscohost.com/nursing/products/cinahl-databases | Nursing and allied health; captures physiotherapy outcome studies not indexed in PubMed | MEDIUM |

### Secondary (Supplement When Needed)

| Database | URL | Why | Confidence |
|----------|-----|-----|------------|
| EMBASE | embase.com | Stronger European coverage than PubMed; useful for COPD, cardiac rehab, Parkinson's | MEDIUM |
| SPORTDiscus | ebscohost.com/academic/sportdiscus | Exercise science specifics, dosage studies | MEDIUM |
| LILACS (Literatura Latino-Americana) | lilacs.bvsalud.org | Brazilian and Latin American clinical studies; bridges international evidence to local context | MEDIUM |
| BVS / Biblioteca Virtual em Saúde | bvsalud.org | Portuguese-language synthesis; useful for translating international evidence to Brazilian clinical practice | MEDIUM |

### What NOT to Use

| Source | Why to Avoid |
|--------|--------------|
| Google Scholar as primary | Cannot filter by study design; no quality rating; mixes preprints, opinion pieces, and grey literature with peer-reviewed evidence |
| ResearchGate PDFs | Version control unknown; may be preprint or retracted versions |
| UpToDate alone | Synthesizes well but is a tertiary source; must trace back to primary literature for Level A claims |
| Wikipedia / general websites | Not peer-reviewed; never citable for clinical protocols |

---

## 2. Authoritative Guideline Bodies

These organizations produce the guidelines that define "Level A" recommendations
for this project's 20 comorbidities.

### Tier 1 — Explicitly Named in PROJECT.md (Required)

| Organization | Scope | Key Publications | Confidence |
|-------------|-------|-----------------|------------|
| IASP (International Association for the Study of Pain) | Chronic pain, neuropathic pain, central sensitization | IASP Chronic Pain Guidelines; Classification of Chronic Pain (ICD-11 alignment); Low Back Pain Task Force | HIGH |
| AGS (American Geriatrics Society) | Comprehensive geriatric care | AGS Beers Criteria (medication safety); AGS Clinical Practice Guidelines; JAGS (Journal of the American Geriatrics Society) | HIGH |
| WHO (World Health Organization) | Global framework, frailty, functional decline | ICOPE (Integrated Care for Older People) 2019+; ICD-11; WHO Rehabilitation 2030 | HIGH |

### Tier 2 — Condition-Specific (Required per Comorbidity)

| Organization | Comorbidities Covered | Key Publications | Confidence |
|-------------|----------------------|-----------------|------------|
| OARSI (Osteoarthritis Research Society International) | OA knee, hip, hand, spine | OARSI Clinical Practice Guidelines for OA Management (updated 2019, 2024 revision in progress) | HIGH |
| EULAR (European League Against Rheumatism) | OA, inflammatory arthritis | EULAR recommendations for OA exercise and physical therapy | HIGH |
| ESC (European Society of Cardiology) | Heart failure, cardiac rehab | ESC Heart Failure Guidelines 2021/2023; Cardiac Rehab position papers | HIGH |
| ATS/ERS (American/European Thoracic Society) | COPD, pulmonary rehab | ATS/ERS Pulmonary Rehabilitation Statement (2023 update) | HIGH |
| MDS (Movement Disorder Society) | Parkinson's disease | MDS Evidence-based medicine review; MDS-UPDRS | HIGH |
| NOF / IOF (National Osteoporosis Foundation / International Osteoporosis Foundation) | Osteoporosis, vertebral fractures | IOF Position statements; FRAX tool; bone-loading exercise guidelines | HIGH |
| NICE (UK National Institute for Health and Care Excellence) | Multi-condition; especially back pain, OA, stroke, dementia | NICE Clinical Guidelines (NG-series) — freely accessible online | HIGH |
| AHA/ACSM | Cardiac rehab, exercise prescription in older adults | ACSM's Exercise Prescription for Older Adults (latest edition) | HIGH |
| APTA (American Physical Therapy Association) | Physical therapy practice guidelines | Clinical Practice Guidelines by specialty (e.g., hip fracture, knee OA, falls) | HIGH |
| SIGN (Scottish Intercollegiate Guidelines Network) | Stroke rehab, falls, dementia | SIGN guidelines freely available; methodologically rigorous | HIGH |
| AAN (American Academy of Neurology) | Parkinson's, stroke, peripheral neuropathy, dementia | AAN Practice Guidelines (evidence-based) | HIGH |
| ADA (American Diabetes Association) | Diabetic peripheral neuropathy | ADA Standards of Medical Care in Diabetes (annual update) | HIGH |

### Tier 3 — Brazilian / Portuguese Context

| Organization | Role | Confidence |
|-------------|------|------------|
| CFisio / CREFITO (Conselho Federal/Regional de Fisioterapia) | Regulatory body for physiotherapy in Brazil; practice scope standards | HIGH |
| COFFITO | Sets competency frameworks for Brazilian physiotherapists | MEDIUM |
| SBGG (Sociedade Brasileira de Geriatria e Gerontologia) | Brazilian geriatric guidelines; bridges international evidence to Brazilian context | MEDIUM |
| MS / Ministério da Saúde (Brazil) | Clinical Protocols and Therapeutic Guidelines (PCDTs) — mandatory for SUS | MEDIUM |

---

## 3. Evidence Grading Systems

The choice of grading system affects how every intervention is classified in the
protocol. The project requires "Level A evidence." That label must be defined
using a specific grading system consistently across all 20 protocols.

### Recommended: Oxford CEBM Levels of Evidence (2011)

**Why:** Universally recognized, simple 1–5 scale, explicitly maps study design
to evidence level. Most international guidelines (OARSI, IASP, AGS) use CEBM or
a derivative. Makes "Level A" claims traceable and defensible.

| Level | Study Type | Label in Protocol |
|-------|-----------|-------------------|
| 1a | Systematic review of RCTs | Level A |
| 1b | Individual RCT (narrow CI) | Level A |
| 2a | Systematic review of cohort studies | Level B |
| 2b | Individual cohort / low-quality RCT | Level B |
| 3 | Case-control studies | Level C |
| 4 | Case series | Level D |
| 5 | Expert opinion | Level E |

Source: Centre for Evidence-Based Medicine, University of Oxford.
URL: cebm.ox.ac.uk/resources/levels-of-evidence

**Confidence: HIGH**

### Supporting System: GRADE (Grading of Recommendations Assessment, Development and Evaluation)

**Why supplement with GRADE:** WHO and Cochrane use GRADE; it captures not just
study design but also consistency, directness, precision, and publication bias.
When citing Cochrane reviews or WHO ICOPE, GRADE ratings (Strong/Conditional,
High/Moderate/Low/Very Low) should be reported alongside CEBM levels.

URL: gradeworkinggroup.org

**Confidence: HIGH**

### What NOT to Use

| System | Why to Avoid |
|--------|-------------|
| Proprietary guideline ratings alone (e.g., "Class I/IIa/IIb" from ESC) | Not generalizable; varies by specialty; creates inconsistency across 20 protocols |
| PEDro scale as evidence level | PEDro rates methodological quality of individual trials, not the body of evidence; it is a search/filter tool, not a grading system |

---

## 4. Mandatory Assessment Tools (Baseline)

These are specified in PROJECT.md as mandatory for every protocol. Research
confirms their validation status and appropriateness for geriatric populations.

### Tier 1 — Mandatory in Every Protocol (PROJECT.md Requirement)

| Tool | Full Name | What It Measures | Validation Status | Confidence |
|------|-----------|-----------------|-------------------|------------|
| TUG | Timed Up and Go Test | Functional mobility, fall risk, lower limb function | Validated across multiple geriatric populations; MCID = 3.4 sec (community), varies by condition; MDS recommended for Parkinson's; NICE-endorsed for falls | HIGH |
| SPPB | Short Physical Performance Battery | Lower extremity function (balance, gait speed, chair stands); composite 0–12 score | Validated for frailty, sarcopenia, post-surgical recovery; MCID = 1 point; widely used in European geriatric trials (LIFE study, SPRINT-T) | HIGH |
| Manual Dynamometry | Handheld dynamometer for grip/muscle strength | Muscle strength, sarcopenia screening | Grip strength (Jamar or equivalent) is the most validated single measure for sarcopenia (EWGSOP2 criteria); isometric strength testing validated for knee extensors, hip abductors | HIGH |

### Tier 2 — Condition-Specific Assessments (Required Per Protocol)

These should be selected based on each comorbidity. The table below maps
recommended tools to the 20 conditions.

| Tool | Acronym | Condition(s) | Psychometric Status | Confidence |
|------|---------|-------------|---------------------|------------|
| Berg Balance Scale | BBS | Falls, stroke, Parkinson's, hip fracture | Validated; MDC = 4–7 pts (varies); ceiling effect in higher-functioning patients | HIGH |
| Mini-BESTest | — | Falls, Parkinson's, post-stroke | More sensitive than BBS for high-functioning older adults; validated 2009, widely adopted | HIGH |
| Functional Gait Assessment | FGA | Falls, Parkinson's, vestibular | 10-item; validated for older adults; predicts fall risk | HIGH |
| Numeric Pain Rating Scale | NPRS / NRS | All pain-related protocols (OA, LBP, shoulder, vertebral fracture) | 11-point scale; MCID = 1.5–2 points in musculoskeletal conditions | HIGH |
| WOMAC | Western Ontario and McMaster Universities OA Index | OA knee/hip, post-arthroplasty | Gold standard for OA outcome research; validated; MCID varies (pain subscale ~10 mm VAS equivalent) | HIGH |
| KOOS / HOOS | Knee/Hip Injury and OA Outcome Score | OA knee/hip, post-arthroplasty (ATJ, ATQ) | More responsive than WOMAC for younger older adults post-surgery; MCID established | HIGH |
| ODI | Oswestry Disability Index | LBP, spinal stenosis, vertebral fractures | Validated; MCID = 10 points; standard in spinal rehabilitation research | HIGH |
| RMDQ | Roland-Morris Disability Questionnaire | LBP, chronic non-specific LBP | 24-item; MCID = 3–5 points; validated for primary care and rehab | HIGH |
| MDS-UPDRS | Movement Disorder Society – UPDRS | Parkinson's disease | Gold standard for Parkinson's severity; replaces original UPDRS; validated MDS 2008 | HIGH |
| MMSE / MoCA | Mini-Mental State Exam / Montreal Cognitive Assessment | Dementia/Alzheimer's screening | MMSE widely used; MoCA more sensitive for MCI; both validated for Brazilian Portuguese | HIGH |
| Barthel Index | BI | Stroke, hip fracture, general ADL | Classic functional independence measure; validated across populations | HIGH |
| FIM | Functional Independence Measure | Stroke, hip fracture, general rehabilitation | 18-item; validated; standard in inpatient rehabilitation | HIGH |
| CAT | COPD Assessment Test | COPD | 8-item; validated; MCID = 2 points; endorsed by GOLD guidelines | HIGH |
| 6MWT | 6-Minute Walk Test | COPD, heart failure, cardiac rehab | Validated; MCID = 25–35 m (COPD), 30–35 m (HF); widely used in pulmonary/cardiac rehab trials | HIGH |
| MLHFQ | Minnesota Living with Heart Failure Questionnaire | Heart failure | 21-item; validated for cardiac rehab outcomes | HIGH |
| Borg RPE Scale | — | COPD, HF, cardiac rehab — exercise intensity monitoring | 6–20 scale; validated for monitoring exertion in older adults with cardiopulmonary conditions | HIGH |
| Utah Toe Test / Michigan Neuropathy Screening | MNSI | Diabetic peripheral neuropathy | MNSI validated for screening and monitoring diabetic neuropathy | MEDIUM |
| CMAP / Monofilament Test | — | Peripheral neuropathy | 10g Semmes-Weinstein monofilament is the clinical standard for protective sensation testing | HIGH |
| FRAX | Fracture Risk Assessment Tool | Osteoporosis, vertebral fractures | WHO-endorsed; validated across populations; estimates 10-year fracture probability | HIGH |
| Shoulder Pain and Disability Index | SPADI | Painful shoulder syndrome | Validated; MCID = 13 points; recommended by APTA CPG for shoulder | HIGH |
| PRAFAB / ICIQ | — | Pelvic floor dysfunction | ICIQ-SF (International Consultation on Incontinence Questionnaire – Short Form) validated for urinary incontinence | HIGH |
| Gait speed (4-meter/10-meter walk test) | — | All protocols — frailty and sarcopenia screening | Gait speed < 0.8 m/s = high fall risk; < 1.0 m/s = sarcopenia criterion (EWGSOP2) | HIGH |

### What NOT to Use as Primary Outcome Tools

| Tool | Reason |
|------|--------|
| VAS (Visual Analog Scale) alone for pain | NRS/NPRS performs equivalently with lower measurement error; NRS preferred for cognitively impaired older adults |
| Jamar dynamometer proprietary norms without age-adjusted references | Must use age/sex-adjusted normative tables (Mathiowetz et al. or EWGSOP2 thresholds) |
| SF-36 as sole outcome measure | Broad but insensitive to rehabilitation-specific changes; use condition-specific tools as primary, SF-36/SF-12 as secondary |

---

## 5. Outcome Measurement Frameworks

### Primary Framework: ICF (International Classification of Functioning, Disability and Health)

**Why:** WHO's ICF is the international standard for structuring rehabilitation
outcomes. It organizes outcomes into Body Functions/Structures, Activities,
and Participation — which maps directly to the three rehabilitation phases
(Acute/Protected, Subacute/Strengthening, Advanced/Functional) required by
this project. Every protocol should map its outcome measures to ICF domains.

URL: who.int/standards/classifications/international-classification-of-functioning-disability-and-health

**Confidence: HIGH**

### Supporting Framework: Core Outcome Sets (COS) via COMET Initiative

**Why:** Many rehabilitation conditions now have internationally agreed Core
Outcome Sets — minimum sets of outcomes that should be measured in clinical
trials and practice. Using COS ensures protocols measure what the research
community measures, making results comparable.

Key COS relevant to this project:
- OMERACT (Outcome Measures in Rheumatology) — OA, musculoskeletal
- COSMIN (COnsensus-based Standards for the selection of health Measurement
  INstruments) — methodological standard for evaluating outcome measures

URL: comet-initiative.org

**Confidence: HIGH**

### Frailty Staging Framework (Required for Geriatric Context)

**Why:** All 20 conditions in this project affect frail or pre-frail older
adults. Protocols must account for frailty status at baseline and progression.
Two validated staging systems are standard:

| Framework | Scale | Use Case |
|-----------|-------|----------|
| Fried Frailty Phenotype | 5 criteria (weight loss, exhaustion, low PA, slow gait, weak grip) | Classifies as robust/pre-frail/frail; validated for community-dwelling older adults |
| Clinical Frailty Scale (CFS) | 1–9 scale | Rapid bedside assessment; validated for hospital and community; endorsed by WHO ICOPE |

**Confidence: HIGH**

### Sarcopenia Diagnostic Criteria: EWGSOP2 (Required)

**Why:** Sarcopenia is a comorbidity (Protocol #8) AND a confounding factor in
nearly all 20 conditions. EWGSOP2 (European Working Group on Sarcopenia in
Older People, 2018 consensus) is the current international standard, using:
1. Low muscle strength (grip < 27 kg men / < 16 kg women)
2. Low muscle quantity/quality (DEXA, BIA, or CT)
3. Low physical performance (SPPB ≤ 8, gait speed ≤ 0.8 m/s, TUG ≥ 20 sec)

This links directly to the project's mandatory TUG, SPPB, and dynamometry tools.

**Confidence: HIGH**

---

## 6. Protocol Structuring Standards

These standards define how a clinical protocol document is formatted and what
elements it must contain to be considered complete and reproducible.

### Primary Standard: TIDieR (Template for Intervention Description and Replication)

**Why:** TIDieR (2014, BMJ) is the international reporting standard for describing
clinical interventions in sufficient detail for replication. It is endorsed by
CONSORT, SPIRIT, and most major rehabilitation journals. Any protocol published
academically must comply. TIDieR has 12 items:

1. Brief name
2. Why (rationale)
3. What (materials)
4. What (procedures)
5. Who provided (provider qualifications)
6. How (delivery mode)
7. Where (setting)
8. When and how much (dosage)
9. Tailoring (individualization)
10. Modifications
11. How well — planned (adherence/fidelity)
12. How well — actual (reported)

URL: tidierguide.org

**Confidence: HIGH**

### Supporting Standard: CERT (Consensus on Exercise Reporting Template)

**Why:** CERT (2016) is the exercise-specific extension of TIDieR. Critically
important for this project because most of the 20 protocols are exercise-based.
CERT adds 16 items specifically for exercise interventions, covering:
- Equipment
- Exercises (type, body part, joint angle)
- Sets, repetitions, frequency, intensity, progression rules
- Supervision level
- Adverse events monitoring

URL: certreportingtool.weebly.com

**Confidence: HIGH**

### Supporting Standard: AGREE II (Appraisal of Guidelines for Research and Evaluation)

**Why:** If any protocol is submitted for academic publication as a clinical
guideline or practice recommendation, AGREE II (23-item instrument across 6
domains) is the peer-review standard used to evaluate its quality. Designing
with AGREE II in mind makes the output publication-ready.

URL: agreetrust.org

**Confidence: HIGH**

### Clinical Phase Structure: AAOS / Rehabilitation Phase Model

The project specifies a flexible 2–4 phase model. The standard phase model
used in international rehabilitation literature is:

| Phase | Name | Criteria to Enter | Criteria to Progress |
|-------|------|------------------|---------------------|
| Phase 1 | Acute / Protected | Post-injury/surgery, pain control, inflammation management | Pain < 4/10 NRS at rest, hemodynamic stability |
| Phase 2 | Subacute / Strengthening | Pain controlled, wound closed, basic mobility restored | Strength > 60% contralateral, independent ambulation |
| Phase 3 | Advanced / Functional | Muscle strength baseline restored, balance adequate | Meet functional discharge criteria (condition-specific) |
| Phase 4 | Return to Full Activity | SPPB ≥ 10, TUG ≤ 12 sec, condition-specific goals met | — |

Note: Not all conditions need Phase 4. Neurological conditions (stroke,
Parkinson's, dementia) require modified frameworks.

**Confidence: MEDIUM** (Phase criteria are condition-specific; exact thresholds
vary by comorbidity and institutional protocol — treat these as defaults to
be refined per-condition.)

---

## 7. Documentation Format Standards

### For Clinical Use (Primary Format)

Structure each protocol document as follows, derived from TIDieR + CERT +
clinical practice guideline norms:

```
PROTOCOL DOCUMENT STRUCTURE (Brazilian Portuguese)

1. Identificação do Protocolo
   - Título / Condição
   - Versão e data
   - Nível de evidência predominante

2. Fundamentação Teórica (rationale)
   - Fisiopatologia resumida
   - Justificativa para as intervenções escolhidas
   - Referências principais (guidelines + RCTs)

3. Critérios de Inclusão e Exclusão
   - Perfil do paciente-alvo
   - Contraindicações absolutas e relativas

4. Avaliação Inicial Obrigatória
   - TUG (com valores normativos e MCID)
   - SPPB (com valores normativos e MCID)
   - Dinamometria Manual (com valores EWGSOP2)
   - Ferramentas condição-específicas (ver Seção 4 acima)

5. Fases de Reabilitação (2–4 conforme condição)
   Por fase:
   a. Critérios de entrada
   b. Objetivos clínicos
   c. Intervenções:
      - Modalidade Terapêutica
      - Terapia Manual
      - Cinesioterapia (parâmetros: séries × repetições × frequência × intensidade)
      - Gama de adaptação clínica
   d. Indicadores de progressão (critérios de saída)

6. Indicadores de Desfecho (Outcome Indicators)
   - Por domínio ICF: Funções Corporais / Atividades / Participação
   - Ferramentas, MCID, frequência de reavaliação

7. Parâmetros de Segurança e Sinais de Alerta
   - "Start low, go slow" application rules
   - Red flags / critérios de suspensão

8. Referências
   - Guidelines (Tier 1 e 2)
   - RCTs e meta-análises de dosagem
```

**Confidence: HIGH** (derived directly from TIDieR + CERT + PROJECT.md
requirements; structure is internally consistent)

### For Academic Use (Publication Format)

When protocols are submitted to journals or academic repositories:
- Use TIDieR checklist as submission supplement
- Follow PRISMA for systematic review elements
- EQUATOR Network (equator-network.org) maintains the master list of all
  reporting guidelines by study type

**Confidence: HIGH**

---

## 8. Exercise Dosage Frameworks

The project requires prescriptive exercise parameters with acceptable ranges.
The following frameworks provide the evidence base for those parameters.

### ACSM Exercise Prescription (Older Adults)

ACSM's Guidelines for Exercise Testing and Prescription (most recent edition:
11th, 2022) and Position Stand on Exercise and Physical Activity for Older
Adults provide the standard FITT-VP framework:

- **F**requency
- **I**ntensity (RPE, %1RM, heart rate zones)
- **T**ime (duration)
- **T**ype
- **V**olume
- **P**rogression

For geriatric populations, ACSM recommends "start low, go slow" — precisely
the principle specified in PROJECT.md, which validates this as the correct
foundation.

**Confidence: HIGH**

### WHO ICOPE Step 2 — Rehabilitation Care Plan

WHO ICOPE (Integrated Care for Older People) provides a rehabilitation care
plan template specifically for older adults with functional decline. ICOPE
covers five intrinsic capacity domains: locomotion, cognition, vitality,
sensory, psychological — all relevant to this project's 20 conditions.

**Confidence: HIGH**

### Resistance Training Dosage Evidence Base

For conditions requiring progressive resistance training (sarcopenia, OA, hip
fracture, post-arthroplasty):

| Parameter | Recommended Starting Range | Progression Target | Source |
|-----------|---------------------------|-------------------|--------|
| Intensity | 40–60% 1RM | 60–80% 1RM | ACSM; Fiatarone Singh meta-analyses |
| Sets | 1–2 initially | 2–4 | ACSM Position Stand |
| Reps | 10–15 | 8–12 | ACSM; EWGSOP2 position |
| Frequency | 2×/week minimum | 3×/week | ACSM; Cochrane sarcopenia reviews |
| Progression | When 2 × BORG < 13 consistently | +5–10% per 2 weeks | ACSM |

**Confidence: MEDIUM** (values are well-established but condition-specific
protocols may warrant different targets; verify against condition-specific
Cochrane reviews and RCTs during protocol research phases)

---

## 9. Stack Summary Table

| Layer | Recommended | Confidence |
|-------|-------------|------------|
| **Primary evidence database** | PubMed + Cochrane Library | HIGH |
| **Specialist rehab database** | PEDro | HIGH |
| **Brazilian/Latin context** | LILACS + BVS | MEDIUM |
| **Tier 1 guidelines** | IASP, AGS, WHO ICOPE | HIGH |
| **OA guidelines** | OARSI + EULAR | HIGH |
| **Cardiopulmonary guidelines** | ATS/ERS, ESC, AHA/ACSM | HIGH |
| **Neurological guidelines** | MDS, AAN, SIGN | HIGH |
| **Brazilian regulatory** | CFisio/CREFITO, SBGG | MEDIUM |
| **Evidence grading** | Oxford CEBM + GRADE | HIGH |
| **Frailty staging** | Fried Phenotype + CFS | HIGH |
| **Sarcopenia criteria** | EWGSOP2 | HIGH |
| **Mandatory baseline tools** | TUG + SPPB + Manual Dynamometry | HIGH |
| **Outcome framework** | ICF domains | HIGH |
| **Core outcome sets** | OMERACT (musculoskeletal), COMET | HIGH |
| **Protocol reporting standard** | TIDieR | HIGH |
| **Exercise reporting standard** | CERT | HIGH |
| **Guideline quality standard** | AGREE II | HIGH |
| **Exercise dosage framework** | ACSM FITT-VP + WHO ICOPE | HIGH |
| **Document structure** | TIDieR + CERT + Clinical template above | HIGH |
| **Academic reporting** | EQUATOR Network guidelines | HIGH |

---

## 10. Alternatives Considered and Rejected

| Category | Recommended | Alternative Considered | Why Not |
|----------|-------------|----------------------|---------|
| Evidence DB | PEDro | Hooked Physiotherapy | PEDro is open-access, more comprehensive, internationally validated |
| Evidence grading | Oxford CEBM + GRADE | Jadad scale alone | Jadad rates only RCT quality, not the body of evidence; too narrow |
| Protocol structure | TIDieR | Free-form narrative | TIDieR ensures reproducibility; free-form creates inconsistency across 20 protocols |
| Exercise reporting | CERT | Generic FITT table | CERT adds critical items (supervision, adverse events, fidelity) absent from basic FITT |
| Pain outcome | VAS alone | — | NRS performs equivalently, is easier to administer, and is preferred for cognitively impaired patients |
| Frailty staging | Fried + CFS | FRAIL scale | FRAIL has weaker predictive validity in hospital settings; Fried + CFS cover community and hospital contexts |

---

## 11. Gaps and Verification Needs

The following items should be verified against current official sources before
use in protocols, as they may have been updated since training cutoff (August 2025):

| Item | Gap / Risk | How to Verify |
|------|-----------|---------------|
| OARSI Guidelines | A 2024 update was in progress as of late 2024 | oarsi.org/research/guidelines |
| ATS/ERS Pulmonary Rehab Statement | 2023 update — confirm final publication status | thoracic.org |
| EWGSOP2 revision | EWGSOP3 was discussed in the literature; confirm current version | myespen.eu |
| MoCA Brazilian Portuguese validation | Confirm most current normative data for Brazil | mocatest.org |
| AGS Beers Criteria | Updated every 3 years; 2023 version current as of cutoff | americangeriatrics.org |
| GRADE confidence ratings | Verify for any Cochrane review cited; ratings can change on re-review | cochranelibrary.com |

---

## Sources

All sources below reflect training knowledge (cutoff August 2025). URLs are
provided for verification; access was not confirmed in this session.

**Evidence Databases**
- PubMed: pubmed.ncbi.nlm.nih.gov
- Cochrane Library: cochranelibrary.com
- PEDro: pedro.org.au
- LILACS: lilacs.bvsalud.org

**Guideline Bodies**
- WHO ICOPE: who.int/teams/integrated-health-services/ageing/icope
- AGS: americangeriatrics.org
- IASP: iasp-pain.org
- OARSI: oarsi.org
- MDS: movementdisorders.org
- ATS: thoracic.org
- ESC: escardio.org
- APTA CPG: apta.org/patient-care/clinical-practice-guidelines

**Standards**
- Oxford CEBM: cebm.ox.ac.uk/resources/levels-of-evidence
- GRADE: gradeworkinggroup.org
- TIDieR: tidierguide.org
- CERT: certreportingtool.weebly.com
- AGREE II: agreetrust.org
- EQUATOR Network: equator-network.org
- COMET Initiative: comet-initiative.org
- COSMIN: cosmin.nl
- ICF: who.int/standards/classifications/international-classification-of-functioning-disability-and-health

**Frailty and Sarcopenia**
- Fried LP et al. (2001). Frailty in older adults. J Gerontol A Biol Sci Med Sci.
- Rockwood K (2005). Clinical Frailty Scale. CMAJ.
- Cruz-Jentoft AJ et al. (2019). Sarcopenia: revised European consensus on definition and diagnosis (EWGSOP2). Age and Ageing.

**Exercise Dosage**
- ACSM Guidelines for Exercise Testing and Prescription, 11th ed. (2022)
- ACSM Position Stand: Physical Activity and Public Health in Older Adults
- WHO ICOPE Implementation Framework (2019)
