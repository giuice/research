# Phase 2: Modificadores Transversais — Research

**Researched:** 2026-03-13
**Domain:** Evidence-Based Geriatric Rehabilitation — Sarcopenia (P-08) and Osteoporosis (P-04) as Cross-Protocol Modifier Documents
**Confidence:** HIGH (structural inheritance, EWGSOP2 criteria) / HIGH (bone-loading constraint evidence) / MEDIUM (GLIS 2024 operational cutoffs — conceptual consensus only, no formal revised cutoffs) / MEDIUM (frailty-stratified RT dosage — gap in literature confirmed)

---

<phase_requirements>
## Phase Requirements

| ID | Description | Research Support |
|----|-------------|-----------------|
| PROT-02 | P-08 Sarcopenia — complete protocol with EWGSOP2-anchored frailty-stratified resistance dosing modifier table and polypharmacy interaction section (protein-exercise coordination, dietitian referral pathway) | EWGSOP2 (2018) diagnostic algorithm confirmed current standard; GLIS 2024 conceptual consensus published but no revised numerical cutoffs; resistance training dosage meta-analyses (PMC12602684, PMC12288929) provide evidence base; drug-induced sarcopenia literature (PMC11503558) supports polypharmacy section |
| PROT-03 | P-04 Osteoporose — complete protocol with bone-loading constraint set by BMD category, long-term HEP adherence strategies, and cross-reference to P-08 resistance dosing | "Too Fit to Fracture" (PMC5112023), UK consensus (PMC9304091), and multiple position statements establish spinal precaution framework; BHOF/NOF 2022 guide provides treatment approach; exercise position statement (PMC10345999) provides resistance/impact parameters; BMD T-score stratification confirmed by WHO criteria |

</phase_requirements>

---

## Summary

Phase 2 produces two protocols that function as authoritative modifiers for all 20 protocols in the series. P-08 Sarcopenia provides the frailty-stratified resistance dosing table that downstream protocols cite instead of independently deriving resistance training parameters. P-04 Osteoporose provides the bone-loading constraint set — movement restrictions, spinal precautions, and impact limits by BMD category — that governs all fracture, arthroplasty, and vertebral protocols.

Both protocols must inherit the complete Phase 1 template architecture (15 sections, TIDieR/CERT, two-column frailty-stratified dosage tables, Oxford CEBM evidence annotations, BR-validated outcome tools, safety architecture). The critical distinction from P-01 is purpose: while P-01 is a standalone clinical protocol, P-08 and P-04 are simultaneously standalone protocols AND cross-protocol reference anchors. Both must be fully self-contained for direct clinical use, while also providing clearly labeled modifier tables that any other protocol in the series can cite directly.

The key research findings for Phase 2 are: (1) EWGSOP2 (2018) remains the operational standard — no EWGSOP3 formal update has been published as of March 2026; the 2024 GLIS paper established only a conceptual definition and explicitly states operational criteria are "forthcoming"; (2) resistance training dosage evidence for sarcopenia now has a 2025 systematic review (PMC12602684) identifying optimal parameters, though frailty-stratified dosage tables are confirmed as a gap in the literature — this makes the Phase 1 SHARED-FOUNDATION template the appropriate anchor; (3) bone-loading constraints for osteoporosis are best organized around the evidence-based movement restriction categories from "Too Fit to Fracture" and the UK "Strong, Steady and Straight" consensus, stratified by fracture history and BMD severity.

**Primary recommendation:** Build P-08 first (resistance dosing modifier table established first for P-04 to cross-reference in its kinesiotherapy section), then P-04 (bone constraint table that all later protocols cite). Both must explicitly label their modifier tables as cross-protocol references.

---

## Standard Stack

### Core Diagnostic Standards and Frameworks

| Framework | Version/Year | Purpose | Why Standard |
|-----------|-------------|---------|--------------|
| EWGSOP2 | 2018 — Cruz-Jentoft AJ et al. Age Ageing 2019;48(1):16-31. PubMed 30312372 | Sarcopenia diagnosis — low strength + low muscle mass + poor performance | Most-used European standard; GLIS 2024 built on it; no EWGSOP3 to replace it |
| GLIS 2024 Conceptual Consensus | 2024 — Kirk B et al. Age Ageing 2024. PMC11210221 | Global conceptual definition of sarcopenia (muscle mass + strength + muscle-specific strength) | Contextual update only; does NOT replace EWGSOP2 cutoffs; signals future operational update coming |
| SARC-F Questionnaire | Morley JE et al. J Am Med Dir Assoc 2013 | Screening tool for sarcopenia risk (5 questions, score 0–10; ≥4 = at risk) | Validated screening instrument; first step in EWGSOP2 FACS algorithm |
| WHO BMD T-Score Categories | WHO 1994 (operationalized by IOF) | Classifies bone mineral density: normal (≥-1.0), osteopenia (-1.0 to -2.5), osteoporosis (≤-2.5) | Universal standard; foundation for all bone-loading constraint stratification |
| FRAX | WHO/NOGG 2008+ (Brazil-specific country model) | 10-year fracture probability; integrates BMD T-score + clinical risk factors | Critical for identifying high fracture risk beyond T-score alone; Brazil-specific model available |
| "Too Fit to Fracture" Consensus | Giangregorio LM et al. Osteoporos Int 2014. PubMed 25510579; PMC5112023 | Exercise recommendations for osteoporosis with and without vertebral fracture | International Delphi consensus; most cited source for exercise precautions in osteoporosis |
| UK "Strong, Steady and Straight" | PMC9304091. 2022 | Physical activity and exercise for osteoporosis — comprehensive consensus | Most recent comprehensive exercise guidance (2022); includes BMD-category stratification for impact exercise |
| BHOF/NOF Clinician's Guide | 2022 — Bone Health and Osteoporosis Foundation | Pharmacological and non-pharmacological osteoporosis management | Standard North American reference; used alongside IOF/NOGG for international alignment |
| TIDieR + CERT | TIDieR-BR (2023) PMC9957771; CERT 2016 | Intervention description and exercise reporting standard | Mandatory per Phase 1 template — inherited by Phase 2 |
| Oxford CEBM 2011 | cebm.ox.ac.uk | Evidence grading per intervention | Standard inherited from Phase 1 |
| Fried Frailty Phenotype | 2001 — Fried LP et al. J Gerontol A | Frailty classification (Robust/Pré-frágil/Frágil) | Primary classifier from SHARED-FOUNDATION; links to dosage table rows |

### Outcome Tools (BR-Validated Versions Required)

| Condition | Tool | BR Validation | Purpose in Protocol |
|-----------|------|---------------|---------------------|
| Sarcopenia | SPPB-BR | Nakano 2007; Guralnik 1994 | Severity classification + phase progression |
| Sarcopenia | Dinamometria Manual (Jamar) | EWGSOP2 — Dodds et al. 2016; Cruz-Jentoft 2019 | Primary sarcopenia assessment + treatment response |
| Sarcopenia | Velocidade de Marcha 4m | EWGSOP2 component | Severity classifier (< 0,8 m/s = severe sarcopenia) |
| Sarcopenia | TUG | Ibrahim et al. 2017, PMC5626462 | Functional mobility + phase progression |
| Osteoporose | TUG | Ibrahim et al. 2017, PMC5626462 | Fall risk + functional mobility |
| Osteoporose | SPPB-BR | Nakano 2007 | Balance/strength functional assessment |
| Osteoporose | FRAX (Brasil) | WHO Brazil model | 10-year fracture risk stratification |
| Both | MoCA-BR | Memoria et al. 2013, PubMed 22368034 | Cognitive screening (especially for P-08, where cognitive frailty is frequent) |

### Sarcopenia-Specific Assessment (EWGSOP2 FACS Algorithm)

| Step | Tool | Cutoffs | Interpretation |
|------|------|---------|---------------|
| F — Find (Screening) | SARC-F | ≥ 4/10 = at risk | Proceed to Assessment |
| A — Assess (Provável) | Força de preensão (Jamar) | H < 27 kg; M < 16 kg | Provável Sarcopenia — confirmar |
| A — Assess (alt) | Levantar-sentar 5× (cadeira) | > 15 seg = baixa força | Alternativa quando dinamômetro indisponível |
| C — Confirm (Confirmada) | Massa muscular — DEXA ou BIA | DEXA: H < 7,0 kg/m² (ASM/h²), M < 5,5 kg/m² | Sarcopenia Confirmada |
| S — Severity | Velocidade de marcha | < 0,8 m/s | Sarcopenia Grave |
| S — Severity (alt) | SPPB-BR | ≤ 8 pontos | Sarcopenia Grave (alternativa) |
| S — Severity (alt) | TUG | > 20 seg | Sarcopenia Grave (alternativa) |

*Fonte: Cruz-Jentoft AJ et al. EWGSOP2. Age Ageing 2019;48(1):16-31. PubMed 30312372*

---

## Architecture Patterns

### Recommended Document Structure — P-08 Sarcopenia (Plan 02-01)

The 15-section P-01 template is inherited with adaptations:

```
P-08-SARCOPENIA.md
├── 1. Critérios Diagnósticos e de Inclusão
│   ├── EWGSOP2 FACS Algorithm (4 steps: Find/Assess/Confirm/Severity)
│   ├── Critérios de inclusão (SARC-F ≥ 4, força preensão abaixo limiar, ≥ 60 anos)
│   └── Critérios de exclusão (doença neuromuscular primária, caquexia oncológica ativa)
├── 2. Avaliação Inicial Mandatória
│   ├── TUG + SPPB-BR + Dinamometria Manual (herdados SHARED-FOUNDATION)
│   ├── SARC-F (5 perguntas — rastreio)
│   └── Velocidade de marcha 4m (< 0,8 m/s = sarcopenia grave)
├── 3. Alinhamento com Diretrizes
│   └── EWGSOP2 2019, GLIS 2024 (contextual), ESPEN protein guidelines
├── 4. Estrutura de Fases (3 fases — herdadas do template P-01)
├── 5-7. Intervenções por Fase (Modalidade / Terapia Manual / Cinesioterapia)
│   └── *** TABELA MODIFICADORA DE DOSAGEM DE RESISTÊNCIA — seção rotulada ***
│       "Este quadro é a referência normativa de dosagem de resistência para
│       todos os 20 protocolos desta série. Cite P-08 Seção X ao invés de
│       derivar parâmetros independentemente."
├── 8. Monitoramento de Dor (NRS por fase)
├── 9. Bandeiras Vermelhas e Escalonamento
├── 10. Interações com Polifarmácia
│   ├── Estatinas → miotoxicidade (risco aumentado com >40 mg sinvastatina)
│   ├── Corticosteroides crônicos → miopatia corticoesteroide
│   ├── Inibidores de aromatase → perda muscular em mulheres pós-menopausa
│   ├── Diuréticos → hipocalemia → fraqueza muscular
│   ├── Betabloqueadores → RPE, não FC como indicador de intensidade
│   └── *** Seção Proteína-Exercício — coordenação e encaminhamento ao nutricionista ***
├── 11. Precauções Cardiorrespiratórias (herdadas)
├── 12. Indicadores de Desfecho
│   ├── Força de preensão (MCID: H 5,0-6,5 kg; M 2,7-5,0 kg)
│   ├── SPPB-BR (MCID: 0,5-1,0 pontos)
│   ├── Velocidade de marcha (MCID: 0,1 m/s)
│   └── TUG (MCID: 2,0-3,0 seg)
├── 13. Rastreabilidade e Flags de Comorbidade
│   └── Cross-reference flags: P-04, P-01, P-05, P-07, P-10, P-11
├── 14. Referências por Nível de Evidência
└── 15. As 8 Questões de Validade Clínica
```

### Recommended Document Structure — P-04 Osteoporose (Plan 02-02)

```
P-04-OSTEOPOROSE.md
├── 1. Critérios Diagnósticos e de Inclusão
│   ├── WHO BMD T-score categories (Normal ≥-1.0; Osteopenia -1.0 a -2.5; Osteoporose ≤-2.5)
│   ├── FRAX — risco de fratura em 10 anos (Brasil-modelo)
│   └── Osteoporose estabelecida = T-score ≤-2.5 + fratura por fragilidade
├── 2. Avaliação Inicial Mandatória
│   ├── TUG + SPPB-BR + Dinamometria Manual (herdados)
│   └── Avaliação postural + cifose torácica (marcha de previsão de queda)
├── 3. Alinhamento com Diretrizes
│   └── BHOF/NOF 2022, UK NOGG 2024, IOF, "Too Fit to Fracture" 2014
├── 4. Estrutura de Fases (adaptada)
├── 5-7. Intervenções por Fase
│   └── *** TABELA DE RESTRIÇÕES DE CARGA ÓSSEA — seção rotulada ***
│       "Este quadro é o conjunto normativo de restrições de carga óssea para
│       todos os protocolos desta série. Cite P-04 Seção X ao avaliar risco
│       de fratura em qualquer protocolo."
├── 8-11. Segurança (NRS, bandeiras, polifarmácia, cardiorrespiratório)
│   └── Polifarmácia: Bifosfonatos, corticosteroides, SERMs, denosumabe,
│       suplementos de cálcio/vitamina D — interações com exercício
├── 12. Indicadores de Desfecho
│   ├── TUG (risco de queda — meta < 13,5 seg)
│   ├── SPPB-BR (equilíbrio — meta ≥ 10)
│   └── FRAX reavaliação anual
├── 13. Rastreabilidade e Flags de Comorbidade
│   └── Cross-reference: P-08 (resistência), P-05 (fratura de fêmur), P-07 (quedas),
│       P-09 (coluna), P-10 (ATJ), P-11 (ATQ), P-16 (IC), P-19 (fraturas vertebrais)
├── 14. Referências por Nível de Evidência
└── 15. As 8 Questões de Validade Clínica
```

### Pattern 1: Cross-Protocol Modifier Table — Labeled Section

**What:** Both P-08 and P-04 must contain a clearly labeled table or section that any of the 20 protocols can reference directly.

**For P-08:** The modifier table is the frailty-stratified resistance dosing table (Section 5 or 6, Cinesioterapia). Label it explicitly as the authoritative cross-protocol dosing reference.

**For P-04:** The modifier table is the bone-loading constraint set (Section 5 or 6). Label it explicitly as the cross-protocol fracture/loading constraint reference.

**Example labeling (mandatory at top of each modifier section):**

```markdown
> **MODIFICADOR TRANSVERSAL — REFERÊNCIA CRUZADA**
> Esta tabela é a referência normativa de [dosagem de resistência / restrições de carga óssea]
> para todos os 20 protocolos de reabilitação geriátrica desta série.
> Quando qualquer protocolo (P-01 a P-20) menciona sarcopenia ou exercício resistido,
> deve citar: "Dosagem conforme P-08, Seção [X]."
> [OU] Quando qualquer protocolo cita risco de fratura ou carga óssea,
> deve citar: "Restrições conforme P-04, Seção [X]."
```

### Pattern 2: EWGSOP2 FACS Algorithm for P-08

**What:** The diagnostic algorithm for sarcopenia follows the 4-step FACS process (Find-Assess-Confirm-Severity).

**Example flow diagram (to be rendered in markdown):**

```
SARC-F ≥ 4?
  └─ Não → Vigilância anual (repetir SARC-F); exercício preventivo
  └─ Sim → Avaliar força de preensão
              └─ ≥ 27 kg (H) / ≥ 16 kg (M) → Sarcopenia improvável; monitorar
              └─ < 27 kg (H) / < 16 kg (M) → PROVÁVEL SARCOPENIA
                    └─ Confirmar massa muscular (DEXA / BIA)
                          └─ Normal → Sarcopenia não confirmada; tratar fraqueza
                          └─ Baixa → SARCOPENIA CONFIRMADA
                                └─ Avaliar desempenho físico (marcha < 0,8 m/s / SPPB ≤ 8 / TUG > 20)
                                      └─ Sim → SARCOPENIA GRAVE
```

### Pattern 3: Bone-Loading Constraint Set for P-04 (3 Categories)

**What:** Organize bone-loading constraints around 3 axes — spinal precautions, impact stratification, and resistance loading — each stratified by fracture risk category.

**Fracture Risk Categories for P-04 (basis for constraint stratification):**

| Categoria | Critério | Base da Restrição |
|-----------|----------|-------------------|
| **Baixo risco** | T-score > -2,5; sem fratura prévia; FRAX < 10% (quadril) ou < 20% (osteoporose maior) | Restrições mínimas; evitar apenas movimentos de alto risco combinado |
| **Médio risco** | T-score -2,5 a -3,0; sem fratura prévia; ou FRAX limítrofe | Restrições moderadas; supervisão em progressão de carga |
| **Alto risco** | T-score < -3,0; OU fratura prévia por fragilidade sem fratura vertebral | Restrições significativas; evitar impacto de alta intensidade |
| **Muito alto risco** | Osteoporose estabelecida + fratura vertebral por compressão prévia | Restrições máximas; apenas exercícios de baixo impacto; HEP adaptado |

**The 3-axis constraint framework:**

```
Eixo 1 — PRECAUÇÕES ESPINAIS (válidas para todos os níveis):
- EVITAR: Flexão espinal carregada (especialmente flexão + rotação combinadas)
- EVITAR: Extensão cervical forçada de alta carga
- PRIORIZAR: Exercícios de extensão espinal (fortalecem extensores do tronco)
- PERMITIR: Rotação suave, controlada, dentro de ADM confortável
- INSTRUÇÃO OBRIGATÓRIA: "Dobradiça do quadril" (hip hinge) para todos os agachamentos/levantamentos

Eixo 2 — RESTRIÇÕES DE IMPACTO (estratificadas por risco de fratura):
- Baixo/Médio risco: Impacto moderado permitido (50 impactos/sessão, ex.: marcha rápida, pulos leves, salto de corda)
- Alto risco: Apenas impacto de baixa intensidade (marcha rápida, tai chi); sem pulos com aterrissagem
- Muito alto risco: Sem exercício de impacto; hidroterapia e exercícios em cadeia fechada de baixa carga

Eixo 3 — CARGA DE RESISTÊNCIA (estratificada por risco de fratura):
- Baixo/Médio risco: 50-85% 1RM; 5-12 repetições; 2-3×/semana; máquinas + peso livre com técnica supervisionada
- Alto risco: 40-60% 1RM; 8-15 repetições; 2×/semana; preferir máquinas (controle de movimento); supervisão obrigatória
- Muito alto risco: Exercícios funcionais de baixa carga; sem levantamento de peso acima da capacidade de controle postural; derivar para P-08 para dosagem de resistência adaptada
```

### Anti-Patterns to Avoid

- **Restringir excessivamente o exercício na osteoporose:** Evidências mostram que grupos com intervenção têm MENOS fraturas (5,8%) que grupos controle (9,6%) — a restrição excessiva é deletéria. Usar framework de risco estratificado, nunca restrição global.
- **Usar GLIS 2024 como substituição ao EWGSOP2:** O GLIS 2024 é uma definição conceitual; os critérios operacionais permanecem os do EWGSOP2 até publicação formal dos critérios GLIS operacionais.
- **Tabela de dosagem de resistência em P-08 sem classificador de fragilidade:** A tabela de dosagem DEVE ser estratificada por fragilidade (Robusto/Pré-frágil/Frágil) seguindo o Fenótipo de Fried da SHARED-FOUNDATION — não apenas por grau de sarcopenia.
- **Prescrever proteína sem encaminhamento ao nutricionista:** A proteína ≥ 1,2 g/kg/dia é recomendada, mas a prescrição dietética é fora do escopo da fisioterapia — a seção de polifarmácia/coordenação em P-08 DEVE incluir pathway de encaminhamento ao nutricionista.
- **Usar apenas T-score para estratificar restrições em P-04:** FRAX integra múltiplos fatores de risco; T-score isolado pode subestimar risco (maioria das fraturas ocorre em pacientes com T-score > -2,5).

---

## Don't Hand-Roll

| Problem | Don't Build | Use Instead | Why |
|---------|-------------|-------------|-----|
| Sarcopenia diagnostic algorithm | Custom strength/mass screening | EWGSOP2 FACS (Find-Assess-Confirm-Severity) | Validated 4-step algorithm; SARC-F as entry point; operationally defined cutoffs (grip < 27/16 kg; ASM/h² < 7,0/5,5 kg/m²) |
| Fracture risk stratification | Custom BMD categories | WHO T-score + FRAX Brazil model | T-score alone misses most fractures; FRAX integrates age, sex, weight, prior fracture, family history, smoking, alcohol, corticosteroids, RA |
| Exercise precautions for osteoporosis | Physician-restriction approach | "Too Fit to Fracture" + UK "Strong, Steady and Straight" frameworks | Evidence base; exercise intervention groups have FEWER fractures than controls; framework balances benefit vs. risk |
| Resistance training dosage for sarcopenia | Ad hoc protocol | Evidence base: 60–70% 1RM, 3 sets × 8–12 reps, 3×/week, ≥ 12 weeks, stratified by frailty (SHARED-FOUNDATION format) | Multiple 2024-2025 meta-analyses converge on these parameters; frailty stratification from Phase 1 foundation |
| Protein-exercise coordination | Generic nutrition note | PROT-AGE recommendations (≥ 1,2 g/kg/dia) + explicit dietitian referral pathway | Protein intake is beyond PT scope of practice; combined protein+exercise evidence is stronger than either alone |
| Sarcopenia screening | Clinical judgment | SARC-F (5-item, 0–10; cutoff ≥ 4) | Validated, fast (< 2 min); first step in EWGSOP2 algorithm; widely used in clinical settings |
| BMD-stratified exercise restrictions | Expert opinion | WHO T-score + "Too Fit to Fracture" Delphi consensus + UK consensus (PMC9304091) | Delphi consensus methodology across international experts; stronger than single-center opinion |

**Key insight:** Both P-08 and P-04 are modifier protocols — their value to the series comes entirely from using internationally validated frameworks as anchors, not custom derivations. Downstream protocols will cite these; the citation chain must trace to authoritative sources.

---

## Common Pitfalls

### Pitfall 1: Treating GLIS 2024 as a Replacement for EWGSOP2
**What goes wrong:** Citing the 2024 GLIS paper (Kirk B et al., PMC11210221) as a new diagnostic standard that supersedes EWGSOP2 cutoffs.
**Why it happens:** The GLIS paper was described as a "global consensus," creating the impression of updated operational criteria.
**How to avoid:** GLIS 2024 established only a conceptual definition — the paper explicitly states "this conceptual definition will now serve to develop an operational definition." Cutoffs (grip < 27/16 kg; ASM/h² < 7,0/5,5 kg/m²; gait speed < 0,8 m/s) remain from EWGSOP2 (2018). Note in P-08: "Critérios operacionais baseados em EWGSOP2 (2018) — aguardando publicação dos critérios operacionais do GLIS."
**Warning signs:** Any sentence claiming specific numerical cutoffs from "GLIS 2024."

### Pitfall 2: Over-Restricting Exercise in Osteoporosis
**What goes wrong:** Prohibiting resistance training or all impact activities for patients with osteoporosis out of fracture concern.
**Why it happens:** Fracture risk creates therapeutic anxiety; exercise-related fractures are overestimated.
**How to avoid:** UK consensus (PMC9304091) found exercise intervention groups sustained fewer fractures (5,8%) than control groups (9,6%). Adopt a risk-stratified approach: low/medium risk → progressive resistance + moderate impact; high risk → supervised resistance + low impact only; very high risk → supervised low-load + balance-focused.
**Warning signs:** Protocol language that says "contraindicado exercício de resistência" without fracture risk stratification.

### Pitfall 3: Sarcopenia Dosage Table Not Stratified by Frailty (Only by Sarcopenia Severity)
**What goes wrong:** Building the resistance dosing table with rows for Provável/Confirmada/Grave sarcopenia instead of Robusto/Pré-frágil/Frágil (Fried).
**Why it happens:** Sarcopenia severity (EWGSOP2) is clinically intuitive for this protocol; frailty stratification (Fried) seems redundant.
**How to avoid:** The Phase 1 SHARED-FOUNDATION dosage format is frailty-stratified (Fried Phenotype) — all protocols must follow this format for consistency and cross-protocol comparability. The sarcopenia severity (Confirmada/Grave) maps to the clinical context WITHIN each frailty tier. In P-08, annotate how sarcopenia severity interacts with frailty tier (e.g., Sarcopenia Grave em paciente Frágil → faixa Frágil + redução adicional de 20% na carga inicial).
**Warning signs:** A dosage table in P-08 without the three Fried frailty rows.

### Pitfall 4: Missing the Protein-Exercise Coordination Section in P-08
**What goes wrong:** Including polypharmacy interactions but omitting the protein-exercise coordination note and dietitian referral pathway.
**Why it happens:** Nutrition is perceived as outside PT scope; the connection to exercise outcome is underappreciated.
**How to avoid:** Evidence is unambiguous — combined protein+exercise significantly outperforms either alone. P-08 must include a dedicated subsection: protein target (≥ 1,2 g/kg/dia, PROT-AGE), timing (protein within 2h post-exercise), vitamin D (alvo sérico 50–75 nmol/L), and explicit pathway: "Encaminhar ao nutricionista quando: (a) paciente reporta ingestão proteica < 1,0 g/kg/dia, (b) IMC < 22, ou (c) sarcopenia grave confirmada."
**Warning signs:** A polypharmacy section in P-08 that covers drug classes but has no protein/nutrition coordination note.

### Pitfall 5: Bone-Loading Constraint Table Without FRAX Integration
**What goes wrong:** Stratifying exercise restrictions in P-04 by T-score alone (normal / osteopenia / osteoporose).
**Why it happens:** T-score is the most commonly known metric; FRAX adds complexity.
**How to avoid:** The majority of hip and vertebral fractures occur in patients with T-score above -2.5 (osteopenia range). FRAX integrates the full clinical risk profile (age, sex, fracture history, corticosteroid use, etc.). The constraint table in P-04 MUST reference FRAX alongside T-score for high and very high risk categories.
**Warning signs:** A constraint table in P-04 with only T-score columns and no mention of FRAX.

### Pitfall 6: Statins Not Included in P-08 Polypharmacy Section
**What goes wrong:** Limiting P-08 polypharmacy to the 6 standard drug classes from SHARED-FOUNDATION without adding statins.
**Why it happens:** Statins are a cardiovascular medication — their muscle toxicity effect in sarcopenia may not be obvious.
**How to avoid:** Drug-related sarcopenia literature (Kuzuya et al. 2024, PMC11503558) specifically identifies statins as having a genetically confirmed causal association with sarcopenia risk. In P-08, add a dedicated row for statins (sinvastatina, atorvastatina): "Miotoxicidade — risco aumentado com doses > 40 mg/dia de sinvastatina; monitorar CK se fadiga muscular incomum; comunicar clínico/cardiologista."
**Warning signs:** Polypharmacy table in P-08 without a statin entry.

### Pitfall 7: Spinal Flexion Restriction Without Evidence Annotation
**What goes wrong:** Stating "evitar flexão espinal" without citing the evidence basis.
**Why it happens:** The restriction is clinically obvious but the evidence citation is assumed.
**How to avoid:** Sinaki M et al. 1984 (PubMed 6487063) — the landmark RCT showing flexion exercise group had 89% additional fracture rate vs. 16% in extension exercise group in postmenopausal osteoporosis. Cite this. The restriction is Nível B (CEBM 2-3 — single RCT + multiple case series).
**Warning signs:** Spinal precaution statements in P-04 without evidence annotation.

---

## Code Examples

Verified patterns for Phase 2 document authorship.

### Template: Cross-Protocol Modifier Label (P-08 Resistance Dosing Table)

```markdown
> **MODIFICADOR TRANSVERSAL — DOSAGEM DE EXERCÍCIO RESISTIDO**
> Esta tabela é a referência normativa de dosagem de resistência para todos os 20
> protocolos de reabilitação geriátrica desta série (P-01 a P-20). Qualquer protocolo
> que aborde exercício resistido em paciente com sarcopenia confirmada deve citar:
> *"Ajustar dosagem conforme P-08 — Tabela de Dosagem de Resistência Estratificada
> por Fragilidade (Seção 6.3)."*
> Protocolos que detectam sarcopenia durante avaliação inicial devem encaminhar
> clinicamente a P-08 como protocolo principal ou co-tratamento.

### Tabela de Dosagem de Exercício Resistido — Modificador Transversal (P-08)

*Fonte: Meta-análise Aging Clin Exp Res 2025 (Springer, doi 10.1007/s40520-025-03235-w);
PMC12288929; EWGSOP2 (Cruz-Jentoft AJ 2019). Estratificação de fragilidade: Fried (2001).*

| Parâmetro | Robusto — Valor Rec. | Robusto — Faixa Aceitável | Pré-frágil — Valor Rec. | Pré-frágil — Faixa Aceitável | Frágil — Valor Rec. | Frágil — Faixa Aceitável |
|-----------|---------------------|--------------------------|------------------------|------------------------------|--------------------|-----------------------|
| Carga inicial | 65% 1RM | 50–75% 1RM | 50% 1RM | 40–65% 1RM | 35% 1RM | 25–50% 1RM |
| Séries | 3 | 2–4 | 2–3 | 1–3 | 2 | 1–3 |
| Repetições | 8–12 | 6–15 | 8–12 | 6–12 | 6–10 | 5–12 |
| Frequência | 3×/semana | 2–4×/semana | 2–3×/semana | 2–3×/semana | 2×/semana | 1–3×/semana |
| Duração mínima | 12 semanas | — | 12 semanas | — | 12 semanas | — |
| Sessão | 50–60 min | 40–60 min | 45–55 min | 30–55 min | 30–45 min | 20–45 min |
| Progressão | +5% quando RPE < 12 | — | +2,5–5% quando RPE < 13 | — | +2,5% quando RPE ≤ 12 | — |

*Nota Sarcopenia Grave (EWGSOP2): Paciente frágil com sarcopenia grave → iniciar na faixa Frágil
com redução adicional de 20% na carga inicial. Aumentar frequência de supervisão.*
```

### Template: Bone-Loading Constraint Table (P-04)

```markdown
> **MODIFICADOR TRANSVERSAL — RESTRIÇÕES DE CARGA ÓSSEA**
> Esta tabela é o conjunto normativo de restrições de carga óssea para todos os
> protocolos desta série. Qualquer protocolo que aborde paciente com osteoporose
> ou risco de fratura (P-01, P-05, P-07, P-10, P-11, P-09, P-19) deve citar:
> *"Aplicar restrições de carga óssea conforme P-04 — Tabela de Restrições por
> Categoria de Risco (Seção 5.2)."*

### Tabela de Restrições de Carga Óssea por Categoria de Risco (P-04)

*Fontes: Giangregorio LM et al. ("Too Fit to Fracture") Osteoporos Int 2014. PubMed 25510579;
Karlsson et al. UK "Strong, Steady and Straight" Consensus. PMC9304091 (2022);
BHOF/NOF Clinician's Guide 2022; WHO T-score criteria.*

| Categoria | Critério | Flexão Espinal | Rotação Espinal | Impacto | Resistência | Supervisão |
|-----------|----------|---------------|-----------------|---------|-------------|------------|
| **Baixo Risco** | T-score > -2,5; sem fratura prévia; FRAX < 10%/< 20% | Evitar flexão forçada com carga | Rotação suave permitida | Moderado (≤ 50 impactos/sessão; marcha rápida, pulos leves) | 50–85% 1RM; 5–12 reps; 2–3×/sem | Recomendada nas primeiras 4 sem |
| **Médio Risco** | T-score -2,5 a -3,0 OU FRAX limítrofe; sem fratura prévia | Evitar flexão carregada; hip hinge obrigatório | Rotação controlada permitida | Baixo-moderado (marcha rápida, Tai Chi; sem pulos de aterrissagem) | 40–70% 1RM; 8–12 reps; 2–3×/sem; preferir máquinas | Supervisão nas primeiras 8 sem |
| **Alto Risco** | T-score < -3,0 OU fratura por fragilidade prévia (sem fratura vertebral) | Evitar toda flexão carregada; Sem sit-ups, curl-ups | Evitar rotação + flexão combinadas | Baixo impacto apenas (marcha, hidroterapia, Tai Chi) | 30–50% 1RM; 10–15 reps; 2×/sem; máquinas; sem carga livre pesada | Supervisão contínua (4–12 sem) |
| **Muito Alto Risco** | Osteoporose + fratura vertebral por compressão prévia | CONTRAINDICADA toda flexão espinal carregada ou forçada | Evitar qualquer rotação com carga | Sem impacto (apenas hidroterapia ou marcha plana) | Exercícios funcionais baixa carga; Referir P-08 para dosagem; sem levantamento > controle postural | Supervisão contínua; fisioterapeuta presente |

> **Regra Geral Espinal (válida para TODAS as categorias):**
> Exercícios de extensão espinal são RECOMENDADOS (Nível B, CEBM 2 —
> Sinaki M et al. 1984, PubMed 6487063). Exercícios de flexão espinal
> carregados são EVITADOS em toda osteoporose com comprometimento vertebral.
> Técnica "hip hinge" deve ser ensinada a todos os pacientes como precaução universal.
```

### Template: Protein-Exercise Coordination Section (P-08, Polypharmacy / Coordenação Nutricional)

```markdown
### Coordenação Proteína-Exercício e Via de Encaminhamento Nutricional

*Nível de Evidência: A (CEBM Nível 1) — PMC12288929; PROT-AGE Study Group (PubMed 23867520)*

**Alvo de ingestão proteica:** ≥ 1,2 g/kg de peso corporal/dia para idosos em
exercício resistido ativo. Meta de 1,5 g/kg/dia em sarcopenia grave confirmada.

**Timing pós-exercício:** Ingestão de 20–25 g de proteína de alto valor biológico
(ex.: proteína do soro do leite / proteína animal) nas 2 horas após cada sessão
de exercício resistido maximiza a síntese proteica muscular.

**Vitamina D:** Alvo sérico 25-OH-D: 50–75 nmol/L. Suplementação 800–2.000 UI/dia
em pacientes com níveis abaixo do alvo (confirmar com equipe médica).

**Via de Encaminhamento ao Nutricionista — Critérios de Acionamento:**
Encaminhar ao nutricionista quando qualquer um dos critérios abaixo for identificado:

| Critério | Ação |
|----------|------|
| Ingestão proteica autorrelatada < 1,0 g/kg/dia | Encaminhar ao nutricionista (urgência moderada) |
| IMC < 22 kg/m² | Encaminhar ao nutricionista (urgência moderada) |
| Sarcopenia Grave confirmada (EWGSOP2) | Encaminhar ao nutricionista (urgência alta) |
| Perda de peso involuntária ≥ 4,5 kg em 12 meses | Encaminhar ao nutricionista + clínico (urgência alta) |
| Incapacidade de preparar ou ingerir refeições adequadas (AVDs) | Encaminhar ao nutricionista + assistente social |

> **Nota de Escopo:** A prescrição dietética (tipo, quantidade e fonte de proteína)
> é responsabilidade do nutricionista. O fisioterapeuta registra critérios de
> encaminhamento e comunica à equipe multidisciplinar. Não prescrever dieta —
> apenas identificar e encaminhar.
```

### Template: Sarcopenia-Specific Polypharmacy Section (P-08, drug classes beyond SHARED-FOUNDATION)

```markdown
### Interações com Polifarmácia — Extensão para Sarcopenia

*Além das 6 classes da Camada de Fundação Compartilhada, adicionar para P-08:*

| Classe Farmacológica | Mecanismo de Risco em Sarcopenia | Implicação Prescritiva |
|---------------------|----------------------------------|------------------------|
| **Estatinas** (sinvastatina > 40 mg, atorvastatina) | Miotoxicidade direta; inibição coenzima Q10; risco de miopatia; associação causal confirmada com sarcopenia | Monitorar CK se fadiga muscular incomum; comunicar clínico se sintomas; não suspender sem orientação médica; avaliar com SARC-F após início |
| **Inibidores de aromatase** (anastrozol, letrozol — em mulheres pós-menopausa com Ca de mama) | Perda de massa muscular e óssea acelerada; interação sinérgica com osteoporose | Combinar P-08 (resistência) + P-04 (osso); aumentar frequência de avaliação de força |
| **Diuréticos de alça** (furosemida) | Hipocalemia → fraqueza muscular; hipomagnesemia | Monitorar eletrólitos antes de intensificar exercício; sessões mais curtas; consultar clínico |
| **Corticosteroides crônicos** (> 3 meses) | Miopatia corticoesteroide (fibras tipo II); perda óssea acelerada (conecta P-04) | Carga de impacto reduzida; fortalecimento de baixa carga; densitometria antes de carga alta; comunicar ortopedista |
| **Antidepressivos ISRS** (fluoxetina, sertralina) | Associados a perda muscular em uso crônico; risco de hiponatremia | Monitorar função muscular; vigilância de SARC-F em uso > 6 meses |
```

---

## State of the Art

| Old Approach | Current Approach | When Changed | Impact for Phase 2 |
|--------------|------------------|--------------|---------------------|
| Sarcopenia = apenas perda de massa muscular | Sarcopenia = perda de força (primária) + perda de massa (confirmação) | EWGSOP2 2018-2019 | P-08 usa força de preensão como gatilho primário, não apenas medidas de massa |
| EWGSOP1 gait speed < 0,8 m/s em qualquer contexto | EWGSOP2: gait speed < 0,8 m/s = sarcopenia grave (severidade), não diagnóstico primário | EWGSOP2 2018 | Velocidade de marcha em P-08 classifica gravidade, não faz diagnóstico inicial |
| Osteoporose = evitar exercício de impacto | Osteoporose = exercício de impacto moderado INDICADO para baixo e médio risco | Too Fit to Fracture 2013-2014; UK 2022 | P-04 deve recomendar impacto moderado como intervenção ativa nos primeiros dois grupos de risco |
| Proteína ≥ 0,8 g/kg (recomendação universal adultos) | Proteína ≥ 1,2 g/kg para idosos; ≥ 1,5 g/kg em sarcopenia ativa + exercício | PROT-AGE 2013; ESPEN 2018 | P-08 deve citar atualização proteica explicitamente; encaminhamento ao nutricionista quando não atingido |
| Resistência como única intervenção em sarcopenia | Combinação resistência + aeróbico + equilíbrio + nutrição (intervenção multicomponente) | Múltiplas meta-análises 2023-2025 | P-08 Fase 2 e Fase 3 devem incluir aeróbico + equilíbrio integrados com resistência |
| Bifosfonatos dispensam orientação de exercício | Bifosfonatos + exercício resistido sinérgicos para ganho de DMO | BHOF 2022; UK NOGG 2024 | P-04 deve apresentar bisfonatos e exercício como complementares — citar necessidade de coordenação com equipe médica |

**Deprecated/Outdated:**
- EWGSOP1 (2010): Substituído por EWGSOP2 (2018) — usar EWGSOP2.
- Definição de sarcopenia baseada apenas em massa muscular reduzida: Substituída por definição baseada em força muscular reduzida como critério primário (EWGSOP2).
- Restrição total de exercício resistido em osteoporose grave: Substituída por abordagem estratificada de risco — exercício resistido supervisionado é indicado mesmo em alto risco, com adaptações.

---

## Open Questions

1. **GLIS 2024 Operational Criteria Publication Status**
   - What we know: The 2024 GLIS paper (PMC11210221) established a conceptual definition of sarcopenia and stated operational criteria are "forthcoming." No EWGSOP3 has been published as of March 2026.
   - What's unclear: When the GLIS operational criteria (with numerical cutoffs) will be published; whether they will change EWGSOP2 cutoffs significantly.
   - Recommendation: Use EWGSOP2 cutoffs in P-08 with explicit note: "Critérios operacionais baseados em EWGSOP2 (2018) — aguardando publicação dos critérios operacionais GLIS. Verificar Age Ageing journal para atualização."

2. **Frailty-Stratified Resistance Dosage for Sarcopenia — Evidence Gap**
   - What we know: 2025 meta-analyses (PMC12602684) confirm optimal overall parameters (3×/sem, 60–70% 1RM, 8–12 reps, ≥ 12 semanas) but explicitly acknowledge absence of frailty-stratified dosage data.
   - What's unclear: Whether different frailty tiers within sarcopenic patients require meaningfully different parameters beyond what the Phase 1 SHARED-FOUNDATION template provides.
   - Recommendation: Apply the Fried frailty stratification (SHARED-FOUNDATION) as the dosage stratifier, annotating that evidence is strongest for the combined parameters and frailty stratification is derived from clinical consensus and ACSM principles rather than direct RCT comparison.

3. **FRAX Brazil Model — Current Version and Calculation Tool**
   - What we know: FRAX has a Brazil-specific country model for 10-year fracture probability calculation. T-score alone is insufficient for risk stratification in P-04.
   - What's unclear: The current FRAX calculator version for Brazil; whether updated epidemiological data (fracture incidence rates) have been incorporated post-2020.
   - Recommendation: Reference FRAX at https://www.sheffield.ac.uk/FRAX/tool.aspx?country=55 (Brazil model). Note in P-04 that clinicians should use the online calculator with current patient data; the protocol cannot substitute for individualized FRAX calculation.

4. **AGS Beers Criteria 2025 Alternatives List (July 2025)**
   - What we know: AGS released a 2025 "Alternative Treatments to Selected Medications in the 2023 AGS Beers Criteria" document in July 2025 — a clinical resource update (not a new edition of the criteria themselves). The 2023 Beers Criteria remain the current edition.
   - What's unclear: Whether the 2025 alternatives list contains any new information relevant to sarcopenia or osteoporosis exercise management.
   - Recommendation: Continue citing AGS Beers Criteria 2023 as the current edition. Note the 2025 alternatives document as supplementary resource for clinicians seeking medication alternatives.

5. **Vitamin D Supplementation Thresholds for Sarcopenia in Brazil**
   - What we know: Target serum 25-OH-D is 50–75 nmol/L; supplementation 800–2,000 IU/day is commonly recommended. Brazil has high UV exposure but significant vitamin D deficiency in institutionalized geriatric populations.
   - What's unclear: Brazil-specific guidelines for vitamin D supplementation in sarcopenia; target levels may differ between outdoor-community-dwelling vs. institutionalized elders.
   - Recommendation: Use ESPEN target (50–75 nmol/L) with note to confirm with equipe médica before initiating supplementation recommendations; supplementation is outside PT scope of practice.

---

## Validation Architecture

> `nyquist_validation: true` is set in .planning/config.json. This is a documentation/specification project. Validation is manual clinical review, not automated testing.

### Test Framework

| Property | Value |
|----------|-------|
| Framework | Manual clinical review (no automated test suite — documentation project) |
| Config file | None |
| Quick run command | N/A — reviewer reads document against protocol checklist |
| Full suite command | N/A — manual review of all 15 sections |

### Phase Requirements — Validation Map

| Req ID | Behavior to Verify | Test Type | Method | Status |
|--------|-------------------|-----------|--------|--------|
| PROT-02 | P-08 contains EWGSOP2-anchored frailty-stratified resistance dosing table labeled as cross-protocol modifier | Manual review | Confirm: (a) FACS algorithm present; (b) dosage table has 3 Fried frailty rows; (c) modifier label present; (d) protein-exercise section with dietitian pathway | Wave 0 — file to create |
| PROT-02 | P-08 polypharmacy section includes statins, inibidores de aromatase, and diuréticos beyond SHARED-FOUNDATION baseline 6 classes | Manual review | Count drug class rows in P-08 polypharmacy table: must be ≥ 9 entries total | Wave 0 — file to create |
| PROT-03 | P-04 contains bone-loading constraint table with 4 fracture risk categories (Baixo/Médio/Alto/Muito alto) | Manual review | Confirm: (a) table has 4 risk rows; (b) FRAX referenced alongside T-score; (c) 3 constraint axes (espinal/impacto/resistência); (d) modifier label present | Wave 0 — file to create |
| PROT-03 | P-04 cross-references P-08 for resistance dosing in kinesiotherapy section | Manual review | Search P-04 for "P-08" cross-reference in kinesiotherapy dosage section | Wave 0 — file to create |
| PROT-02 + PROT-03 | Both protocols answer all 8 clinical validity questions | Manual review | Checklist per protocol: who qualifies, when stop, where start, what to do, how much, how fast, how to measure, why | Wave 0 — files to create |
| PROT-02 + PROT-03 | Both protocols inherit all Phase 1 standards (15-section format, TIDieR/CERT, Oxford CEBM, BR-validated tools) | Manual review | Verify section count ≥ 15; verify TIDieR/CERT header; verify -BR suffix on all outcome tools | Wave 0 — files to create |

### Wave 0 Gaps

- [ ] `protocols/P-08-SARCOPENIA.md` — PROT-02 (entire file, Plan 02-01)
- [ ] `protocols/P-04-OSTEOPOROSE.md` — PROT-03 (entire file, Plan 02-02)
- [ ] SHARED-FOUNDATION.md update — P-08 and P-04 rows in cross-reference index (Section 8.1 matrix)

*(No existing test infrastructure — all content is greenfield for Phase 2)*

---

## Sources

### Primary (HIGH confidence)
- EWGSOP2 — Cruz-Jentoft AJ et al. Age Ageing 2019;48(1):16-31. PubMed 30312372 — sarcopenia definition, FACS algorithm, grip/mass/gait cutoffs
- GLIS 2024 Conceptual Consensus — Kirk B et al. Age Ageing 2024. PMC11210221 — global conceptual definition (NOT operational criteria)
- "Too Fit to Fracture" Consensus — Giangregorio LM et al. Osteoporos Int 2014. PubMed 25510579; PMC5112023 — exercise recommendations for osteoporosis with and without vertebral fracture
- UK "Strong, Steady and Straight" Consensus — PMC9304091 (2022) — exercise precautions stratified by vertebral fracture status; spinal flexion/impact guidance
- Sinaki M et al. 1984. PubMed 6487063 — extension vs. flexion RCT in osteoporosis; 89% fracture rate in flexion group vs. 16% in extension group
- BHOF/NOF Clinician's Guide 2022 — Bone Health and Osteoporosis Foundation — multicomponent exercise recommendation; pre-exercise evaluation requirement
- WHO T-score Categories — WHO 1994/IOF operationalization — Normal ≥-1.0; Osteopenia -1.0 to -2.5; Osteoporosis ≤-2.5
- PROT-AGE Study Group — PubMed 23867520 — protein ≥ 1.0–1.2 g/kg/day for older adults; evidence-based recommendation
- AGS Beers Criteria 2023 — PubMed 37139824 — current edition; 2025 alternatives list is supplementary only

### Secondary (MEDIUM confidence)
- Systematic review 2025 — Optimal RT prescriptions for sarcopenia — PMC12602684 — 3×/week, 50–60 min, 24 RCTs, 951 participants; no frailty stratification
- Nutrition and exercise sarcopenia review — PMC12288929 — combined protein+RT synergy; protein 1.5 g/kg/day in active sarcopenia; vitamin D targets
- Drug-related sarcopenia review — Kuzuya et al. 2024. PMC11503558 — statins, glucocorticoids, antidepressants, NSAIDs as sarcopenia-worsening medications
- Exercise guidelines osteoporosis position statement — PMC10345999 (2023) — resistance 50–85% 1RM, 5–12 reps, 2–3×/week; impact 3+ days/week ≥ 50 jumps/session (low/no fracture risk)
- Academy of Geriatric Physical Therapy CPG — PMC8983944 (2022) — PT management osteoporosis; emphasis on supervised programs; safety evidence from limited adverse events in trials
- Dose-response sarcopenia meta-analysis — Aging Clin Exp Res 2025 — training frequency and resistance type as main effect modifiers; 3×/week > 2×/week for grip strength
- FRAX Brazil model — WHO/Sheffield; country-55 model available at sheffield.ac.uk/FRAX

### Tertiary (LOW confidence — flag for validation)
- Handgrip strength dose-response (Bayesian network meta-analysis) — PMC12263917 (2025) — optimal 19-week program at 49% 1RM; details from search summary only, not full text verified
- Vitamin D supplementation thresholds for Brazilian geriatric sarcopenia — derived from ESPEN general guidance; Brazil-specific guideline not confirmed in this research

---

## Metadata

**Confidence breakdown:**
- EWGSOP2 diagnostic criteria and algorithm: HIGH — primary source confirmed (PubMed 30312372)
- Sarcopenia resistance training dosage parameters: HIGH for overall parameters; MEDIUM for frailty stratification (evidence gap confirmed by 2025 meta-analysis)
- GLIS 2024 status: HIGH — confirmed as conceptual only; no operational cutoffs published
- Bone-loading constraint framework: HIGH — "Too Fit to Fracture" (Delphi), UK consensus (PMC9304091), Sinaki RCT all confirmed
- BMD T-score stratification: HIGH — WHO criteria well-established
- FRAX integration: MEDIUM — Brazil model exists; current version and calibration not verified
- Drug-related sarcopenia (statins): MEDIUM — causal association confirmed by Kuzuya 2024 (PMC11503558); specific exercise interaction data limited
- Protein-exercise coordination: HIGH — PROT-AGE (PubMed 23867520) and PMC12288929 confirm ≥ 1,2 g/kg; combined intervention superiority is Level A evidence
- AGS Beers 2023 currency: HIGH — confirmed current edition; 2025 document confirmed as alternatives list only, not new edition

**Research date:** 2026-03-13
**Valid until:** 2026-09-13 (6 months — stable domain); exceptions: GLIS operational criteria (verify monthly — publication expected); EWGSOP3 (verify if announced); FRAX Brazil calibration (verify annually)
