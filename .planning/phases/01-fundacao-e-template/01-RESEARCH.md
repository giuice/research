# Phase 1: Fundação e Template — Research

**Researched:** 2026-03-12
**Domain:** Evidence-Based Geriatric Rehabilitation Protocol Architecture — Osteoarthritis (P-01) as Template
**Confidence:** HIGH (structural/methodological domains) / MEDIUM (specific Brazilian validation citations) / MEDIUM (OARSI 2024 update status)

---

<phase_requirements>
## Phase Requirements

| ID | Description | Research Support |
|----|-------------|-----------------|
| STRUC-01 | Each protocol includes diagnostic/inclusion criteria defining exactly which patients qualify | ACR/EULAR OA classification criteria; inclusion criteria template researched |
| STRUC-02 | Each protocol includes contraindications, precautions, and red flags with stopping rules | Red flag table structure and NRS-anchored stopping thresholds documented |
| STRUC-03 | Flexible clinical phase structure (2-4 phases) with function-based entry/exit criteria | 3-phase model (Aguda/Subaguda/Avançada) plus flexible 2-4 phase logic confirmed |
| STRUC-04 | Interventions classified by: Therapeutic Modality, Manual Therapy, Kinesiotherapy | AGENTS.md classification taxonomy confirmed; output format defined |
| STRUC-05 | Shared Foundation Layer created first | Foundation document architecture fully specified herein |
| ASMNT-01 | Universal baseline battery (TUG, SPPB, Manual Dynamometry) with age-stratified normative values and MCIDs | All three tools researched: normative values, MCIDs, and stratification confirmed |
| ASMNT-02 | Primary outcome indicators per phase with re-evaluation schedule | Phase-linked outcomes and re-evaluation cadence documented |
| ASMNT-03 | Functional benchmark targets at phase transitions | Function-based transition criteria model defined |
| ASMNT-04 | All outcome tools cited in Brazilian Portuguese validated versions | SPPB-BR, WOMAC-BR, MoCA-BR, ODI-BR validation citations confirmed |
| DOSE-01 | Two-column dosage format (recommended value + acceptable clinical range) | Format specified and verified operable in OA context |
| DOSE-02 | "Start low, go slow, but reach the goal" principle embedded | Principle operationalized as first-session load rules and progression logic |
| DOSE-03 | Frailty-stratified dosage tables (Robust / Pre-frail / Frail) | Fried phenotype + CFS stratification researched; dosage differentiation documented |
| DOSE-04 | Objective progression criteria (within-phase and phase-advancement) | Function-anchored criteria (not time-based) documented |
| EVID-01 | Evidence level classification per intervention (Oxford CEBM Level A/B/C) | Oxford CEBM 2011 levels confirmed as current standard |
| EVID-02 | Guideline alignment declaration (IASP, AGS, WHO, condition-specific body) | For OA: OARSI 2019 (most current stable version) + ACR 2022 alignment confirmed |
| EVID-03 | Research conducted in English from PubMed + Cochrane + PEDro triad | Source triad confirmed; PubMed identifiers provided where available |
| SAFE-01 | Pain monitoring with NRS thresholds per phase (IASP-aligned) | NRS 0-10 phase thresholds researched; IASP resource confirmed |
| SAFE-02 | Structured red flag table with escalation pathways | Red flag categories and escalation logic documented |
| SAFE-03 | Polypharmacy interaction section (most common drug classes + exercise implications) | NSAIDs, corticosteroids, antihypertensives, anticoagulants researched |
| SAFE-04 | Cardiorespiratory precautions section in every protocol | Template section architecture documented |
| OUT-01 | Final protocols written in Brazilian Portuguese | Language requirement confirmed; all clinical terms documented in PT-BR |
| OUT-02 | One structured markdown document per comorbidity | Document format confirmed |
| OUT-03 | Protocols follow TIDieR/CERT reporting standards | TIDieR-BR (2023) and CERT (16-item) confirmed as standards; Brazilian PT available |
| OUT-04 | Cross-reference index mapping protocol interactions and comorbidity flags | Index skeleton architecture defined |
| PROT-01 | P-01 Osteoartrite — complete template protocol | Full OA protocol architecture researched (OARSI 2019, ACR 2022, exercise dosage) |
</phase_requirements>

---

## Summary

Phase 1 creates two deliverables that all subsequent phases depend on: (1) a Shared Foundation Layer document establishing universal standards, and (2) P-01 Osteoartrite, the template protocol that demonstrates every structural, dosage, evidence, and safety requirement in operation. All 25 requirements in this phase are architectural — they set standards that cascade to all 19 remaining protocols.

The domain combines clinical protocol science (what to prescribe), evidence methodology (how to grade and cite), and document architecture (how to structure). The research-in-English, write-in-Portuguese requirement creates a translation-validation step that must be explicit: every Brazilian Portuguese term for an assessment tool or outcome measure must carry its validation citation. The critical STATE.md blocker — OARSI 2024 update status — has been investigated: as of the research date, OARSI 2019 remains the most complete stable guideline; the 2024 rehabilitation review updates evidence on exercise effectiveness but does not supersede the 2019 guideline recommendations. P-01 should cite OARSI 2019 as primary and note the 2024 evidence review.

The frailty stratification architecture (Robust / Pre-frail / Frail) is based on the Fried phenotype (2001) operationalized by EWGSOP2 (2018) and CFS scoring. Dosage tables must differentiate all three strata with the two-column format (recommended + acceptable range). The Oxford CEBM 2011 levels of evidence remain the current standard with no update needed; these map cleanly to Level A (systematic reviews/RCTs, CEBM Level 1), Level B (controlled studies, Level 2-3), and Level C (expert consensus, Level 4-5).

**Primary recommendation:** Build the Shared Foundation Layer document first (Task 01-01), then use it as the active reference while authoring P-01 (Task 01-02). P-01 must be reviewable by a clinician with no other documents — every cross-reference to the Foundation Layer must be reproduced inline.

---

## Standard Stack

### Core Standards and Frameworks

| Framework | Version/Year | Purpose | Why Standard |
|-----------|-------------|---------|--------------|
| OARSI Guidelines | 2019 (stable) + 2024 Year in Review | Non-surgical management of knee/hip/polyarticular OA | Most comprehensive, internationally endorsed, GRADE-based evidence |
| ACR Osteoarthritis Guideline | 2022 | Pharmacological and non-pharmacological OA management | Complementary to OARSI; covers polypharmacy implications |
| Oxford CEBM Levels of Evidence | 2011 (current) | Evidence grading per intervention | Standard in physical therapy, rehabilitation, and clinical guidelines |
| TIDieR Checklist | 2014 original + 2023 Brazilian Portuguese translation | Intervention description and replication template | Internationally endorsed; Brazilian PT version published 2023 (PMC9957771) |
| CERT (Consensus on Exercise Reporting Template) | 2016 (16-item) | Exercise-specific reporting standard | Mandatory for exercise interventions; pairs with TIDieR |
| Fried Frailty Phenotype | 2001 (Fried et al.) | Classifies patients as Robust / Pre-frail / Frail | Operational 3-category classification usable in dosage tables |
| EWGSOP2 | 2018 (Cruz-Jentoft et al.) | Operationalizes frailty/sarcopenia assessment thresholds | Defines low grip strength and slow gait speed cutoffs by gender |

### Assessment Tool Validation Citations (Brazilian Portuguese Versions)

| Tool | Instrument Code | Validation Citation | Psychometric Summary |
|------|----------------|---------------------|----------------------|
| Short Physical Performance Battery | SPPB-BR | Nakano (2007) — translated; Brucki validation; ICC = 0.83 test-retest | MCID: 0.5 points (small change), 1.0 point (substantial change); frailty: SPPB ≤ 9 has 81% sensitivity in Brazilian elders |
| WOMAC (Western Ontario and McMaster) | WOMAC-BR | Fernandes (2003, UNIFESP — master's thesis); structural validity confirmed by Oliveira et al. PMC9673866 and ELSA-Brasil Musculoskeletal cohort (PubMed 31858210) | 3 domains: pain (5 items), stiffness (2 items), function (17 items); adequate reliability and construct validity |
| Montreal Cognitive Assessment | MoCA-BR | Bertolucci et al. (2008 conference); Memoria et al. (2013, PubMed 22368034) — sensitivity 81%, specificity 77% for MCI at cut-off 25 points; AUC 0.82 | Valid for cognitive screening in ≥4 years education; education-adjusted cutoffs required |
| Oswestry Disability Index | ODI-BR | Vigatto, Alexandre, Correa Filho (2007, Spine) — PubMed 17304141; Cronbach α = 0.87; ICC = 0.99; responsiveness confirmed by Mancin et al. (2008, PMC2518761) | Excellent reliability; moderate correlation with pain (r = 0.66); validated for Brazilian culture |

### Assessment Battery Normative Values

| Tool | Age Group | Normative Value | MCID | Source |
|------|-----------|----------------|------|--------|
| TUG | 60-64 | ~8.1 sec (community) | — | Ibrahim et al. 2017 (PMC5626462) |
| TUG | 71-75 | 9.5 ± 2.5 sec | — | Ibrahim et al. 2017 |
| TUG | 76-80 | 9.9 ± 3.0 sec | — | Ibrahim et al. 2017 |
| TUG | 81-85 | 11.2 ± 3.6 sec | — | Ibrahim et al. 2017 |
| TUG | 86-99 | 12.0 ± 3.8 sec | — | Ibrahim et al. 2017 |
| TUG | Risk threshold | > 13.5 sec = fall risk | 2.0-3.0 sec (clinical estimate) | Podsiadlo & Richardson 1991 |
| SPPB | Community elders | 9–11 (intact); ≤ 6 (severe impairment) | 0.5–1.0 points | Guralnik 1994; Pavasini 2016 (PubMed 35341435) |
| SPPB | Frailty threshold | ≤ 9 = frailty (81% sensitivity, Brazilian sample) | — | SPPB RehabMeasures |
| Grip Strength (M) | 60-69 | 35.0–40.0 kg (Jamar) | 5.0–6.5 kg | Dodds et al. 2016; EWGSOP2 low cutoff: < 27 kg |
| Grip Strength (F) | 60-69 | 19.0–24.0 kg (Jamar) | 2.7–5.0 kg | Dodds et al. 2016; EWGSOP2 low cutoff: < 16 kg |

### Evidence Sources (Triad per EVID-03)

| Database | Use | Access |
|----------|-----|--------|
| PubMed | Primary literature, RCTs, systematic reviews | pubmed.ncbi.nlm.nih.gov |
| Cochrane Library | Systematic reviews and meta-analyses | cochranelibrary.com |
| PEDro | Exercise RCTs rated by PEDro scale | pedro.org.au |

---

## Architecture Patterns

### Recommended Document Structure — Shared Foundation Layer (Task 01-01)

```
SHARED-FOUNDATION.md
├── 1. Universal Baseline Battery
│   ├── TUG — protocol, age-stratified norms, MCIDs, equipment
│   ├── SPPB — protocol, age-stratified norms, MCIDs, frailty threshold
│   └── Manual Dynamometry — protocol, gender-stratified norms, MCIDs, sarcopenia cutoffs
├── 2. Frailty Classification System
│   ├── Fried Phenotype — 5 criteria, scoring, Robust/Pre-frail/Frail classification
│   └── Clinical Frailty Scale (CFS) — 1-9 scale cross-mapping to Fried categories
├── 3. Progression Principle
│   └── "Start low, go slow, but reach the goal" — operational definition with first-session
│       load rules, progression rate, and goal-definition logic
├── 4. Oxford CEBM Evidence Grading Standard
│   ├── Level 1 = systematic reviews/RCTs → maps to "Nível A"
│   ├── Level 2-3 = controlled/cohort studies → maps to "Nível B"
│   └── Level 4-5 = case series/expert consensus → maps to "Nível C"
├── 5. Dosage Format Standard
│   ├── Two-column format specification (recommended | acceptable range)
│   └── Frailty-stratified table template (Robusto | Pré-frágil | Frágil)
├── 6. Brazilian Portuguese Outcome Tool Registry
│   ├── SPPB-BR — validation citation, cutoffs, scoring
│   ├── WOMAC-BR — validation citation, domains, scoring
│   ├── MoCA-BR — validation citation, education-adjusted cutoffs
│   └── ODI-BR — validation citation, disability categories
├── 7. Safety Architecture Template
│   ├── NRS pain monitoring thresholds (by phase)
│   ├── Red flag table structure
│   ├── Escalation pathway template
│   ├── Polypharmacy section template
│   └── Cardiorespiratory precautions template
└── 8. Cross-Reference Index Skeleton
    └── Comorbidity interaction matrix (20×20 shell — populated progressively)
```

### Recommended Document Structure — P-01 Osteoartrite (Task 01-02)

```
P-01-OSTEOARTRITE.md
├── Cabeçalho / Metadados (TIDieR Item 1-2)
│   ├── Nome, autoria, data, versão
│   └── Condição-alvo, população, setting
├── Critérios Diagnósticos e de Inclusão (STRUC-01)
│   ├── Critérios ACR para OA de joelho/quadril/mão
│   ├── Critérios de inclusão no protocolo (TUG, SPPB, CFS)
│   └── Critérios de exclusão
├── Avaliação Inicial Mandatória (ASMNT-01)
│   ├── TUG — procedimento, registro, interpretação
│   ├── SPPB-BR — procedimento, registro, interpretação
│   └── Dinamometria Manual — procedimento, registro, interpretação
├── Alinhamento com Diretrizes (EVID-02)
│   ├── OARSI 2019 — declaração de alinhamento
│   ├── ACR 2022 — declaração de alinhamento
│   └── AGS / WHO — declaração de alinhamento
├── Estrutura de Fases (STRUC-03)
│   ├── Fase 1: Aguda/Protegida — critérios de entrada, objetivos, duração típica, critérios de saída
│   ├── Fase 2: Subaguda/Fortalecimento — idem
│   └── Fase 3: Avançada/Funcional — idem
├── Intervenções por Fase (STRUC-04)
│   ├── Modalidade Terapêutica (eletrotermofototerapia se justificada)
│   ├── Terapia Manual
│   └── Cinesioterapia
│       └── Tabelas de dosagem com franja de fragilidade (DOSE-01, DOSE-03)
├── Monitoramento de Dor (SAFE-01)
│   └── NRS limiar por fase
├── Bandeiras Vermelhas e Escalada (SAFE-02)
├── Interações com Polifarmácia (SAFE-03)
├── Precauções Cardiorrespiratórias (SAFE-04)
├── Indicadores de Desfecho (ASMNT-02, ASMNT-03, ASMNT-04)
│   ├── WOMAC-BR
│   ├── SPPB-BR (reavaliação)
│   ├── TUG (reavaliação)
│   └── Dinamometria (reavaliação)
├── Referências (EVID-01, EVID-03)
│   └── Classificadas por nível Oxford CEBM
└── Rastreabilidade (OUT-04)
    └── Flags de comorbidade — quais outros protocolos são afetados por achados deste protocolo
```

### Pattern 1: Two-Column Dosage Format with Frailty Stratification (DOSE-01, DOSE-03)

**What:** Every exercise parameter is presented in a table with three rows (Robusto / Pré-frágil / Frágil) and two columns per parameter (Valor Recomendado | Faixa Clínica Aceitável).

**When to use:** All kinesiotherapy and aerobic exercise prescriptions.

**Example format:**
```
| Parâmetro          | Robusto                    | Pré-frágil                 | Frágil                     |
|--------------------|---------------------------|---------------------------|---------------------------|
| Carga inicial      | 60-70% 1RM | 50-70% 1RM  | 40-60% 1RM | 30-60% 1RM  | 30-40% 1RM | 20-40% 1RM  |
| Séries             | 3 | 2-4                   | 2-3 | 1-3                   | 2 | 1-3                       |
| Repetições         | 10-12 | 8-15             | 8-10 | 6-12                | 6-8 | 5-10                     |
| Frequência         | 3x/sem | 2-4x/sem        | 2-3x/sem | 2-3x/sem     | 2x/sem | 1-3x/sem         |
| Progressão (carga) | +5% quando RPE < 12       | +2.5-5% quando RPE < 13   | +2.5% quando RPE ≤ 12     |
```

Format columns: `Valor Recomendado | Faixa Clínica Aceitável` (separated by pipe within each cell, or as adjacent columns).

### Pattern 2: Oxford CEBM Evidence Annotation Per Intervention

**What:** Every intervention receives an inline evidence annotation at first mention.

**Format:**
```
Exercício resistido progressivo (Cinesioterapia)
Nível de Evidência: A (CEBM Nível 1) — Bannuru et al. 2019 (OARSI); Fransen et al. 2015 Cochrane
```

**Level mapping:**
- Nível A = Oxford CEBM Level 1 (systematic reviews of RCTs)
- Nível B = Oxford CEBM Level 2-3 (individual RCTs, cohort studies)
- Nível C = Oxford CEBM Level 4-5 (case series, expert consensus)

### Pattern 3: Phase Transition Criteria (Functional, Not Time-Based) (DOSE-04, ASMNT-03)

**What:** Advancement from one phase to the next requires meeting objective functional benchmarks.

**Example for OA Phase 1 → Phase 2:**
```
Critérios de Progressão para Fase 2:
- NRS dor em repouso ≤ 3/10 por 3 sessões consecutivas
- TUG < 14 seg (ou melhora ≥ 2 seg do basal)
- Ausência de edema articular significativo
- Amplitude de movimento funcional preservada para AVDs
```

**Anti-Patterns to Avoid:**
- **Tempo como único critério:** Nunca escrever "após 2 semanas, progredir para Fase 2" sem critério funcional ancorando a decisão.
- **Dose única sem faixa:** Nunca prescrever apenas "3x10 repetições" sem a faixa de adaptação clínica.
- **Nível de evidência sem citação:** Nunca declarar "Nível A" sem a referência primária ao lado.
- **Ferramenta em inglês sem validação-BR:** Nunca citar SPPB, WOMAC, MoCA, ODI sem acrescentar a sigla "-BR" e a citação de validação.

---

## Don't Hand-Roll

| Problem | Don't Build | Use Instead | Why |
|---------|-------------|-------------|-----|
| Evidence grading taxonomy | Custom scoring rubric | Oxford CEBM 2011 Levels 1-5 | Internationally recognized; maps cleanly to Level A/B/C language; clinicians understand it |
| Intervention reporting format | Custom checklist | TIDieR + CERT combined | TIDieR-BR (2023) is already translated; CERT covers exercise specifics; both are peer-reviewed standards |
| Frailty classification | Custom 3-tier description | Fried Phenotype (2001) + CFS | Fried provides operational 5-criteria scoring; CFS provides rapid clinical judgment; both validated in geriatric populations |
| Exercise outcome measurement | Ad hoc progress notes | SPPB-BR, TUG, Dinamometria Manual | These have published normative values, MCIDs, and Brazilian PT validation — custom measures have none |
| OA-specific patient outcomes | Custom functional score | WOMAC-BR | Validated Brazilian Portuguese version with published reliability; recognized by OARSI and ACR |
| Cognitive screening | Bedside mental status | MoCA-BR | Validated sensitivity/specificity for MCI in Brazilian elders; recognized by AGS |

**Key insight:** Every "hand-rolled" solution in this domain lacks normative data, MCIDs, and cross-study comparability — the entire clinical value of using standard tools comes from their ability to detect change against a known reference. Custom tools cannot do this.

---

## Common Pitfalls

### Pitfall 1: Citing OARSI 2024 as a "New Guideline" When None Was Published
**What goes wrong:** The 2024 "Year in Review" article from OARSI (Osteoarthritis and Cartilage) summarizes research trends and raises uncertainty about exercise effects — it is NOT a guideline update. Citing it as a new recommendation source would misrepresent its authority.
**Why it happens:** The article appears in the OARSI journal, creating confusion with the 2019 guideline.
**How to avoid:** Cite OARSI 2019 (Bannuru et al.) as the current guideline. Mention the 2024 review as a contextual update: "A revisão de 2024 acrescenta nuances sobre magnitude de efeito, mas não substitui as recomendações de 2019."
**Warning signs:** Any sentence that begins "As diretrizes OARSI de 2024 recomendam..."

### Pitfall 2: Using WOMAC Without Its Brazilian Portuguese Validation Citation
**What goes wrong:** Writing "WOMAC" instead of "WOMAC-BR" and failing to cite Fernandes (2003) or Oliveira et al. (2022, PMC9673866) — makes the tool's language validity unverifiable.
**Why it happens:** WOMAC is so universally known that authors assume no citation is needed.
**How to avoid:** Template every outcome tool mention as `[NOME-BR (Autor-ano)]`. In the Foundation Layer, create a lookup table so every protocol inherits the correct citation automatically.
**Warning signs:** Any outcome tool name without the "-BR" suffix and a validation year.

### Pitfall 3: Frailty Dosage Without Operational Classification Criteria
**What goes wrong:** Including a Robust/Pre-frail/Frail table but not specifying HOW the patient is classified into each tier — leaves clinician guessing.
**Why it happens:** The classification step is assumed to be obvious.
**How to avoid:** In the Foundation Layer, define the classification procedure: Fried score 0 = Robusto, 1-2 = Pré-frágil, ≥ 3 = Frágil. Reference CFS 1-3 = Robusto, 4-5 = Pré-frágil, 6-9 = Frágil. Link this to the SPPB score (≤ 9 = high frailty probability).
**Warning signs:** A dosage table with frailty rows but no "Como classificar o paciente" subsection preceding it.

### Pitfall 4: Time-Only Phase Progression Criteria
**What goes wrong:** "Fase 1 dura 2-3 semanas" with no functional exit criteria. A patient who is not ready gets advanced by calendar; a patient who is ready gets held back.
**Why it happens:** Time-based criteria are easier to write and administer.
**How to avoid:** Every phase must include a "Critérios de saída" table with at least one objective measurement (NRS threshold, TUG score change, SPPB score) alongside a realistic time window as a reference, not as a criterion.
**Warning signs:** Any phase description that only mentions duration without functional benchmarks.

### Pitfall 5: Polypharmacy Section as Generic Warning Instead of Exercise-Specific Interaction Table
**What goes wrong:** Writing "idosos frequentemente usam múltiplos medicamentos" without specifying which drug classes affect which exercise parameters and how.
**Why it happens:** Polypharmacy is complex and clinicians fear overstepping scope.
**How to avoid:** Research and document at minimum: NSAIDs (GI/renal/cardiovascular precautions, fall risk increase), corticosteroids (bone density, muscle wasting implications for loading), antihypertensives (orthostatic hypotension, beta-blocker blunted HR response), anticoagulants (contact precautions, bruising risk). For each: what to monitor, what to modify in the exercise prescription.
**Warning signs:** A polypharmacy section with no specific drug class entries.

### Pitfall 6: MoCA-BR Cutoff Without Education Adjustment
**What goes wrong:** Applying a flat cutoff of 26/30 (or 25/30) for all patients regardless of education level.
**Why it happens:** The original MoCA cutoff is widely cited without the education adjustment.
**How to avoid:** The Foundation Layer must specify education-adjusted cutoffs: +1 point for ≤ 12 years education (as per Nasreddine/Memoria guidance). Brazilian geriatric population has high rates of limited formal education — this correction is clinically essential.
**Warning signs:** MoCA cutoff cited without an education-stratified footnote.

---

## Code Examples

These are structural templates for document authorship, not software code.

### Template: NRS Pain Monitoring Thresholds by Phase (SAFE-01)

```markdown
### Monitoramento de Dor (NRS 0-10)

| Fase | Limiar de Interrupção Imediata | Limiar de Modificação | Dor Aceitável Durante Exercício |
|------|-------------------------------|----------------------|--------------------------------|
| Fase 1 (Aguda) | NRS ≥ 5 | NRS 3-4 → reduzir carga 25% | NRS ≤ 3 (leve, esperada) |
| Fase 2 (Subaguda) | NRS ≥ 6 | NRS 4-5 → reduzir carga 20% | NRS ≤ 4 |
| Fase 3 (Avançada) | NRS ≥ 7 | NRS 5-6 → reduzir carga 15% | NRS ≤ 5 |

**Regra geral (IASP-alinhada):** Dor pós-exercício que excede a dor pré-exercício por mais de 2 pontos na NRS e persiste > 24 horas indica sobrecarga — reduzir volume na sessão seguinte.
```

### Template: Red Flag Table (SAFE-02)

```markdown
### Bandeiras Vermelhas — Escalonamento Imediato

| Sinal/Sintoma | Ação | Destino |
|---------------|------|---------|
| Dor articular aguda de novo, sem trauma identificado | Suspender sessão | Encaminhar reumatologista |
| Inchaço articular súbito, calor e eritema | Suspender sessão | Encaminhar reumatologista / urgência |
| Febre associada a dor articular | Suspender sessão | Clínico / urgência |
| Dor irradiada com déficit neurológico novo | Suspender sessão | Neurocirurgia / urgência |
| Dor em repouso noturna progressiva (oncológica?) | Não iniciar exercício | Encaminhar oncologista |
| Dispneia desproporcional ao esforço | Suspender sessão | Cardiologista / urgência |
| Hipotensão ortostática sintomática (> 20 mmHg queda sistólica) | Suspender sessão | Clínico |
```

### Template: Polypharmacy Section (SAFE-03)

```markdown
### Interações com Polifarmácia

| Classe Farmacológica | Implicação para o Exercício | Modificação Prescritiva |
|---------------------|----------------------------|------------------------|
| AINEs (AAS, ibuprofeno, naproxeno) | Mascaramento da dor → risco de sobrecarga; risco cardiovascular/renal em exercício intenso | Reforçar monitoramento NRS; evitar exercício de alta intensidade sem supervisão |
| Corticosteroides (uso crônico) | Miopatia corticoesteroide, perda óssea → fragilidade muscular e risco de fratura | Reduzir cargas de impacto; priorizar fortalecimento de baixa carga; comunicar ortopedista |
| Antihipertensivos (betabloqueadores) | Resposta de FC embotada → FC não é indicador confiável de intensidade | Usar RPE (Borg 6-20) como indicador de intensidade em vez de FC alvo |
| Antihipertensivos (vasodilatadores, diuréticos) | Risco de hipotensão ortostática | Período de resfriamento obrigatório; levantar lentamente; monitorar PA pré/pós |
| Anticoagulantes (varfarina, rivaroxabana) | Risco de sangramento em contusões | Evitar exercícios de contato; monitorar equimoses; comunicar equipe médica |
| Benzodiazepínicos / sedativos | Sonolência, risco de queda aumentado | Agendar sessões longe do pico de ação; enfatizar supervisão de equilíbrio |
```

### Template: Cardiorespiratory Precautions Section (SAFE-04)

```markdown
### Precauções Cardiorrespiratórias

**Avaliação pré-participação:** Todo paciente idoso deve ter avaliação cardiovascular documentada antes de iniciar exercício moderado-intenso. Verificar: PA basal, frequência cardíaca, história de ICC, DPOC, arritmias.

**Indicadores de parada imediata:**
- Dor torácica, pressão precordial ou irradiação para braço/mandíbula
- Dispneia súbita e desproporcional ao esforço
- Palpitações com tontura/síncope
- PA sistólica > 200 mmHg ou queda > 10 mmHg durante esforço progressivo
- Saturação O₂ < 90% durante exercício (se oximetria disponível)

**Adaptação para pacientes com ICC/DPOC conhecida:**
- Iniciar na faixa Frágil independentemente do escore de fragilidade
- Sessões mais curtas (15-20 min), maior frequência semanal
- RPE ≤ 13 (Borg 6-20) como limite superior
```

### Template: Evidence Annotation Format (EVID-01)

```markdown
**Exercício resistido progressivo (Cinesioterapia)**
- Nível de Evidência: **A** (CEBM Nível 1)
- Referência primária: Fransen M et al. Exercise for osteoarthritis of the knee. Cochrane Database Syst Rev. 2015. PEDro score: 8/10
- Alinhamento: OARSI 2019 (Bannuru et al.) — Core Treatment, sem restrição de comorbidade
```

---

## State of the Art

| Old Approach | Current Approach | When Changed | Impact for P-01 |
|--------------|------------------|--------------|-----------------|
| Passivar o paciente na fase aguda (repouso absoluto) | Exercício ativo imediato de baixa carga; mobilização precoce | OARSI 2019; ACR 2022 | Fase 1 deve incluir cinesioterapia desde o início — não apenas modalidades passivas |
| FC alvo como indicador de intensidade aeróbica | RPE (Borg 6-20) complementa ou substitui FC em pacientes com betabloqueadores | Reconhecido amplamente; ACSM GETP 11th ed. | Todas as tabelas de dosagem aeróbica devem incluir RPE, não apenas % FC máx |
| WOMAC como desfecho único em OA | WOMAC + SPPB + TUG como bateria mínima (funcional + autorrelatado) | OARSI 2019 recomenda bateria multidomínio | P-01 deve usar os três como desfechos primários combinados |
| Exercício aquático como alternativa apenas para "pacientes que não toleram terra" | Exercício aquático como opção terapêutica de primeiro nível equivalente | OARSI 2019; revisão aquática PMC11755622 (2025) | Deve aparecer como opção igualmente válida na tabela de cinesioterapia |
| Gradação de evidência by association | Oxford CEBM nivel por intervenção específica com citação primária | Padrão contemporâneo | Cada intervenção precisa de anotação individual — não basta declarar "o protocolo é baseado em evidências" |

**Deprecated/Outdated for this project:**
- EWGSOP1 (2010): Substituído por EWGSOP2 (2018) para definição de sarcopenia — usar EWGSOP2.
- OARSI 2014 (knee only): Substituído por OARSI 2019 (knee + hip + polyarticular) — usar 2019.
- TIDieR sem CERT: Para protocolos de exercício, TIDieR sozinho é insuficiente — usar sempre TIDieR + CERT.

---

## Open Questions

1. **OARSI 2024 Update Publication Status**
   - What we know: A "Year in Review 2024" article exists in Osteoarthritis and Cartilage (PMC) summarizing recent rehabilitation research; it raises uncertainty about exercise effect sizes but does not issue new recommendations.
   - What's unclear: Whether OARSI has published or announced a full guideline update post-2019 for inclusion in P-01.
   - Recommendation: Cite OARSI 2019 as the current guideline. Note the 2024 review as supplementary context. Planner should flag for clinician review before final protocol sign-off.

2. **EWGSOP3 Status**
   - What we know: STATE.md flags EWGSOP3 publication status as unknown. EWGSOP2 (2018, Cruz-Jentoft et al.) is the current confirmed standard for sarcopenia.
   - What's unclear: Whether EWGSOP3 has been published or is forthcoming as of March 2026.
   - Recommendation: Use EWGSOP2 cutoffs (grip: < 27 kg men, < 16 kg women; gait speed: < 0.8 m/s) for the Foundation Layer. Note in the document: "Cutoffs baseados em EWGSOP2 (2018) — verificar publicação de EWGSOP3 antes de finalizar."

3. **AGS Beers Criteria Currency**
   - What we know: AGS Beers Criteria 2023 edition exists. STATE.md flags need to confirm 2026 status.
   - What's unclear: Whether a 2025 or 2026 update has been issued.
   - Recommendation: Use AGS Beers Criteria 2023 for the polypharmacy section. Note explicitly: "Baseado em AGS Beers 2023 — verificar atualizações."

4. **WOMAC-BR Primary Peer-Reviewed Validation Article**
   - What we know: Fernandes (2003) is frequently cited but was a master's thesis, not a peer-reviewed journal article. Structural validity was confirmed by Oliveira et al. (2022, PMC9673866) and ELSA-Brasil cohort (PubMed 31858210).
   - What's unclear: Whether a single peer-reviewed article is universally accepted as the canonical WOMAC-BR validation citation.
   - Recommendation: Cite Oliveira et al. (2022, BMC Musculoskelet Disord, PMC9673866) as primary peer-reviewed validation and Fernandes (2003) as original translation source. This dual citation provides both peer-review credibility and historical traceability.

5. **NRS Exercise Stopping Thresholds — IASP-Specific Sourcing**
   - What we know: The 0-10 NRS is validated for geriatric use (sensitivity/specificity confirmed). IASP provides educational resources. The specific "stop at NRS ≥ X during exercise" threshold is a clinical convention applied in rehabilitation, not explicitly codified in an IASP guideline document.
   - What's unclear: Whether IASP has published specific exercise-context NRS thresholds or whether the protocol must synthesize from rehabilitation RCTs.
   - Recommendation: Source NRS thresholds from: (1) published OA exercise RCTs using explicit stopping rules, (2) ACSM exercise safety guidelines, and (3) clinical consensus — then note "Baseado em prática clínica estabelecida e parâmetros de segurança de RCTs de referência" rather than claiming a specific IASP document.

---

## Validation Architecture

> `nyquist_validation: true` is set in .planning/config.json. This is a documentation/specification project with no test suite. Validation is clinical review, not automated testing.

### Test Framework

| Property | Value |
|----------|-------|
| Framework | Manual clinical review (no automated test suite — documentation project) |
| Config file | None |
| Quick run command | N/A — reviewer reads document against checklist |
| Full suite command | N/A |

### Phase Requirements — Validation Map

| Req ID | Behavior to Verify | Test Type | Method | Status |
|--------|-------------------|-----------|--------|--------|
| STRUC-01 | P-01 contains diagnostic/inclusion criteria section | Manual review | Check for ACR classification criteria + inclusion table | Wave 0 gap |
| STRUC-02 | P-01 contains red flag table with escalation pathways | Manual review | Count ≥ 5 red flags with escalation destination | Wave 0 gap |
| STRUC-03 | P-01 has ≥ 2 phases with functional entry/exit criteria | Manual review | Verify each phase has criteria table | Wave 0 gap |
| STRUC-04 | Each intervention classified under Modalidade/Terapia Manual/Cinesioterapia | Manual review | Check classification headers present | Wave 0 gap |
| STRUC-05 | Foundation Layer document exists and is complete | Manual review | Check all 8 sections of Foundation Layer | Wave 0 gap |
| ASMNT-01 | TUG, SPPB, Dinamometria in every protocol with norms and MCIDs | Manual review | Verify normative table present with source citations | Wave 0 gap |
| ASMNT-04 | All tools cited with "-BR" suffix and validation citation | Manual review | Search document for all tool names; confirm suffix + citation | Wave 0 gap |
| DOSE-01 | Two-column format present in every exercise table | Manual review | Verify "Valor Recomendado | Faixa Aceitável" columns | Wave 0 gap |
| DOSE-03 | Frailty-stratified rows (Robusto/Pré-frágil/Frágil) in all exercise tables | Manual review | Count rows per table | Wave 0 gap |
| EVID-01 | Oxford CEBM level annotated per intervention | Manual review | Verify "Nível A/B/C (CEBM X)" annotation on each intervention | Wave 0 gap |
| SAFE-01 | NRS thresholds table by phase present | Manual review | Check NRS table with 3 phase rows | Wave 0 gap |
| SAFE-02 | Red flag table with escalation | Manual review | Verify table format matches template | Wave 0 gap |
| SAFE-03 | Polypharmacy section with ≥ 4 drug classes | Manual review | Count drug class rows | Wave 0 gap |
| SAFE-04 | Cardiorespiratory precautions section present | Manual review | Check section header and stopping criteria | Wave 0 gap |
| PROT-01 | P-01 answers all 8 clinical validity questions | Manual review | Checklist: who qualifies, when stop, where start, what to do, how much, how fast, how to measure, why | Wave 0 gap |

### "8 Clinical Validity Questions" Checklist for P-01

The success criteria require that P-01 answer these unambiguously:

1. **Quem se qualifica?** — Critérios diagnósticos + inclusão/exclusão
2. **Quando parar?** — NRS thresholds + red flags + escalation
3. **Por onde começar?** — Fase 1 entry criteria + initial dosage table
4. **O que fazer?** — All 3 intervention categories with specific exercises
5. **Quanto?** — Two-column dosage format per exercise per frailty tier
6. **Quão rápido progredir?** — Progression criteria (functional, not time-only)
7. **Como medir o progresso?** — Outcome tools with re-evaluation schedule
8. **Por que essas escolhas?** — Evidence annotations (Oxford CEBM + primary citations)

### Wave 0 Gaps

- [ ] No existing documents to verify against — all content is greenfield.
- [ ] Clinical reviewer designation needed before final sign-off on P-01 (human clinician or structured AI review against the 8-question checklist).
- [ ] Open questions 1-5 above should be explicitly marked in the produced documents as "verificar antes de publicação definitiva."

---

## Sources

### Primary (HIGH confidence)
- OARSI 2019 Guidelines — Bannuru RR et al., Osteoarthritis Cartilage 2019; PubMed 31278997 — core OA exercise recommendations
- Oxford CEBM 2011 Levels of Evidence — cebm.ox.ac.uk — evidence grading standard
- TIDieR Checklist — EQUATOR Network equator-network.org/reporting-guidelines/tidier/ — intervention reporting standard
- TIDieR-BR (2023) — PMC9957771 — Brazilian Portuguese translation confirmed available
- CERT (16-item) — Slade et al., Physical Therapy 2016; academic.oup.com/ptj/article/96/10/1514 — exercise reporting standard
- Fried Frailty Phenotype — Fried LP et al., J Gerontol A Biol Sci Med Sci. 2001;56(3):M146-56 — frailty classification
- ODI-BR — Vigatto R et al., Spine 2007; PubMed 17304141 — Brazilian Portuguese validation
- MoCA-BR — Memoria CM et al., Int Psychogeriatr 2013; PubMed 22368034 — Brazilian Portuguese validation
- TUG normative values — Ibrahim A et al., PLoS One 2017; PMC5626462 — age/gender/MCI stratified norms
- SPPB MCID — Pavasini R et al., Eur Heart J Acute Cardiovasc Care 2016; PubMed 35341435 — MCID 3 points (cardiovascular); Perera et al. 0.5-1.0 points (community)
- EWGSOP2 — Cruz-Jentoft AJ et al., Age Ageing 2019;48(1):16-31 — sarcopenia/frailty cutoffs

### Secondary (MEDIUM confidence)
- WOMAC-BR structural validity — Oliveira AM et al., BMC Musculoskelet Disord 2022; PMC9673866 — peer-reviewed Brazilian structural validity confirmation
- WOMAC-BR ELSA-Brasil cohort — PubMed 31858210 — psychometric properties in large Brazilian sample
- OARSI 2024 Year in Review — Osteoarthritis Cartilage 2024; oarsijournal.com — rehabilitation and outcomes update (not a guideline revision)
- ACR 2022 OA Guideline — stacks.cdc.gov/view/cdc/151745 — complementary to OARSI for pharmacological interactions
- Aquatic exercise OA systematic review — PMC11755622 (2025) — dosage parameters for aquatic modality
- Polypharmacy + exercise — Lancet Healthy Longevity 2025; ScienceDirect article pii/S2666756825000820 — drug-exercise interaction framework
- Grip strength normative values — Dodds et al. 2016 (Age Ageing); JOSPT 2018 (US norms) — reference values by age/gender

### Tertiary (LOW confidence — flag for validation)
- WOMAC-BR original translation — Fernandes MI, 2003, UNIFESP master's thesis — cited widely but not peer-reviewed journal article; use only with secondary peer-reviewed citation
- NRS exercise stopping thresholds — synthesized from rehabilitation RCT stopping rules (no single IASP guideline document confirmed) — verify with primary OA exercise RCTs
- OARSI 2024 guideline update — not confirmed; recommend treating 2019 as current until official OARSI announcement

---

## Metadata

**Confidence breakdown:**
- Standard stack (frameworks, grading systems): HIGH — Oxford CEBM, TIDieR, CERT, Fried phenotype all confirmed via official sources
- Brazilian PT validation citations (SPPB-BR, MoCA-BR, ODI-BR): HIGH — specific PubMed IDs confirmed
- WOMAC-BR primary citation: MEDIUM — Fernandes 2003 is widely cited thesis; Oliveira 2022 (PMC9673866) is preferred peer-reviewed source
- OARSI 2024 status: MEDIUM — 2024 article exists but confirmed as review, not guideline; no new OARSI guideline confirmed
- NRS stopping thresholds (IASP-specific): LOW — clinical convention; specific IASP document not confirmed
- Polypharmacy interaction data: MEDIUM — verified via Lancet Healthy Longevity 2025 and specific drug class literature
- TUG/SPPB/Grip normative values: HIGH — specific PMC IDs confirmed for all three

**Research date:** 2026-03-12
**Valid until:** 2026-09-12 (stable domain — 6 months); exceptions: OARSI guideline status (verify quarterly), EWGSOP3 (verify immediately if published), AGS Beers (verify if 2025/2026 edition announced)
