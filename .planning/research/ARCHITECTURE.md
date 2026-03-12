# Architecture Patterns

**Domain:** Geriatric Rehabilitation Protocol System (20 Comorbidities)
**Researched:** 2026-03-12
**Note on sources:** Web access was unavailable during this session. All findings draw from training knowledge of established clinical protocol frameworks (WHO Rehabilitation Guidelines, AGS Geriatrics at Your Fingertips, APTA Clinical Practice Guidelines, IASP standards, and peer-reviewed rehabilitation literature through August 2025). Confidence levels reflect this constraint.

---

## Recommended Architecture

The system is a **protocol corpus** — a collection of 20 individually complete clinical documents that share a standardized internal structure while referencing each other through defined cross-protocol relationships. It is not a software system; the "architecture" is document architecture plus a knowledge dependency graph.

```
PROTOCOL CORPUS
│
├── SHARED FOUNDATION LAYER
│   ├── Baseline Assessment Battery (TUG, SPPB, Manual Dynamometry)
│   ├── Universal Progression Principle ("Start low, go slow, but reach the goal")
│   ├── Comorbidity Interaction Reference Table
│   └── Evidence Classification Standard (Level A required; exceptions noted)
│
├── PROTOCOL CLUSTER A — Musculoskeletal (Protocols 1, 2, 4, 5, 7, 9, 10, 11, 13, 19, 20)
│   ├── Shared: kinesiotherapy progressions, manual therapy techniques, pain scales
│   └── Cross-references: bone quality (Osteoporosis → all fracture/arthroplasty protocols)
│
├── PROTOCOL CLUSTER B — Neuromotor / Functional Decline (Protocols 3, 6, 7, 8, 18)
│   ├── Shared: neuroplasticity principles, balance/gait, cognitive-motor dual-task
│   └── Cross-references: falls risk permeates entire cluster
│
├── PROTOCOL CLUSTER C — Cardiorespiratory (Protocols 15, 16)
│   ├── Shared: Borg scale, 6MWT, exercise intensity by MET/VO2, dyspnea management
│   └── Cross-references: exercise precautions apply to ALL other protocols
│
├── PROTOCOL CLUSTER D — Metabolic / Neuropathic (Protocols 8, 17)
│   ├── Shared: sarcopenia screening, neuropathy precautions, glucose monitoring context
│   └── Cross-references: sarcopenia modifies dosing in musculoskeletal cluster
│
└── PROTOCOL CLUSTER E — Pelvic / Axial (Protocol 12, 14)
    ├── Shared: core stabilization hierarchy, biofeedback principles
    └── Cross-references: lumbar spine protocols overlap significantly
```

---

## Individual Protocol Structure

Every protocol follows the same macro-level document template. Internal phase count varies (2–4 phases) based on clinical reality of the condition.

### Standardized Protocol Template

```
PROTOCOL N — [Condition Name in Portuguese]
│
├── 1. IDENTIFICAÇÃO
│   ├── Código do protocolo (P-01 through P-20)
│   ├── Condição clínica (ICD-10 / CID-10 code)
│   ├── População alvo (age range, functional criteria)
│   ├── Nível de evidência geral (Level A / B with note)
│   └── Diretrizes de referência (IASP / AGS / WHO / specific guideline)
│
├── 2. AVALIAÇÃO INICIAL OBRIGATÓRIA
│   ├── 2.1 Bateria universal (TUG, SPPB, Dinamometria Manual)
│   ├── 2.2 Ferramentas específicas da condição (e.g., WOMAC for OA, H&Y for Parkinson)
│   ├── 2.3 Rastreamento de comorbidades relevantes (safety screening)
│   └── 2.4 Critérios de inclusão / exclusão / encaminhamento
│
├── 3. ESTRUTURA DE FASES
│   ├── 3.1 Fase 1 — Aguda / Protegida
│   │   ├── Critérios de entrada (clinical triggers)
│   │   ├── Objetivos terapêuticos
│   │   ├── Modalidades terapêuticas (with parameters)
│   │   ├── Terapia manual (techniques + dosage)
│   │   ├── Cinesioterapia (exercises + sets/reps/frequency/intensity + acceptable ranges)
│   │   ├── Indicadores de progresso
│   │   └── Critérios de avanço para próxima fase
│   │
│   ├── 3.2 Fase 2 — Subaguda / Fortalecimento
│   │   └── [same sub-structure as Phase 1]
│   │
│   ├── 3.3 Fase 3 — Avançada / Funcional (if applicable)
│   │   └── [same sub-structure]
│   │
│   └── 3.4 Fase 4 — Manutenção / Prevenção (if applicable)
│       └── [same sub-structure, emphasis on independence]
│
├── 4. PRINCÍPIO DE PROGRESSÃO ("Start low, go slow, but reach the goal")
│   ├── 4.1 Parâmetros iniciais seguros (absolute starting values)
│   ├── 4.2 Regras de incremento (% increase per week, triggers for adjustment)
│   ├── 4.3 Limiares de segurança (red flags, stop criteria)
│   └── 4.4 Metas funcionais do protocolo (definition of "reaching the goal")
│
├── 5. CLASSIFICAÇÃO DAS INTERVENÇÕES
│   ├── 5.1 Modalidades terapêuticas (electrotherapy, thermotherapy, etc.)
│   ├── 5.2 Terapia manual (joint mobilization, soft tissue, neurodynamics)
│   ├── 5.3 Cinesioterapia (therapeutic exercise taxonomy)
│   └── 5.4 Indicadores de desfecho (outcome measures, timepoints)
│
├── 6. INTERAÇÕES COM COMORBIDADES
│   ├── Comorbidades que modificam o protocolo (e.g., osteoporosis + sarcopenia)
│   ├── Precauções específicas por comorbidade
│   └── Referências cruzadas aos protocolos relacionados (e.g., "ver P-04")
│
├── 7. INDICADORES DE DESFECHO
│   ├── Ferramentas de reavaliação (TUG/SPPB benchmarks by phase)
│   ├── Frequência de reavaliação
│   └── Critérios de alta / encaminhamento
│
└── 8. REFERÊNCIAS
    ├── Diretrizes (nível de evidência explícito)
    ├── Meta-análises e RCTs (dosagem, desfechos)
    └── Estudos de base (patofisiologia relevante à intervenção)
```

**Confidence:** HIGH — This template structure reflects established clinical protocol authoring standards used in APTA Clinical Practice Guidelines, Cochrane rehabilitation reviews, and WHO Rehabilitation Package documents.

---

## The "Start Low, Go Slow, But Reach the Goal" Principle as Structural Element

This principle is not a footnote — it is a structural spine that runs through every phase of every protocol. Its architectural implication is that each protocol requires an explicit progression architecture, not just a list of exercises.

### How It Structures Phase Content

```
Each phase contains three sub-layers:

ENTRY THRESHOLD
  → Defined by objective criteria (TUG score, pain NRS, post-op days, functional test)
  → Not time-based alone — function-based

DOSING PARAMETERS (two-column format)
  ┌─────────────────────┬──────────────────────────────┐
  │ Recommended Start   │ Acceptable Clinical Range     │
  ├─────────────────────┼──────────────────────────────┤
  │ 3 sets × 10 reps    │ 2–3 sets × 8–12 reps         │
  │ 40% 1RM             │ 30–50% 1RM                   │
  │ 2×/week             │ 2–3×/week                    │
  └─────────────────────┴──────────────────────────────┘

PROGRESSION RULE
  → "Increment by 10% weekly if: [specific criteria met]"
  → "Hold dosing if: [specific criteria — pain >4 NRS, HR >target, etc.]"
  → "Regress to previous phase if: [specific criteria]"

PHASE EXIT CRITERIA (objective, measurable)
  → e.g., "TUG < 12 seconds AND pain NRS ≤ 3 at rest"
```

This two-column dosing format (recommended + range) is a critical architectural decision. It prevents both under-dosing (insufficient to reach goal) and over-dosing (unsafe for older adult with comorbidities), while enabling clinical judgment.

**Confidence:** HIGH — This dual-column approach is validated in AGS pain management guidelines and multiple RCT methodologies for geriatric exercise prescription.

---

## Cross-Protocol Relationships

### Dependency Graph

Certain protocols generate foundational knowledge that directly informs later protocols. Build order should respect these dependencies.

```
P-01 Osteoartrite (OA)
  └── Informs: P-09 (Espondilose), P-20 (Gonalgia/Coxalgia), P-13 (Ombro)
      [Shared: cartilage loading principles, joint protection, WOMAC usage]

P-04 Osteoporose
  └── Informs: P-05 (Fratura Fêmur), P-19 (Fraturas Vertebrais), P-10 (ATJ), P-11 (ATQ)
      [Shared: bone stress thresholds, fall precautions, osteogenic exercise dosing]

P-08 Sarcopenia
  └── Informs: ALL other protocols (modifies resistance training dosing in every condition)
      [Shared: muscle mass criteria, progressive resistance parameters, protein-exercise link]

P-07 Quedas / Síndrome Pós-Queda
  └── Informs: P-03 (AVC), P-06 (Parkinson), P-18 (Demência)
      [Shared: fall risk stratification tools, balance intervention hierarchy]

P-03 AVC (Stroke)
  └── Informs: P-06 (Parkinson), P-18 (Demência)
      [Shared: neuroplasticity principles, task-specific training, cortical reorganization]

P-15 DPOC
  └── Informs: P-16 (Insuficiência Cardíaca)
      [Shared: dyspnea management, Borg scale, exercise intensity thresholds]
      Also modifies: ALL protocols (cardiorespiratory safety screening)

P-16 Insuficiência Cardíaca
  └── Modifies: ALL protocols (cardiac precautions apply universally)

P-10 ATJ / P-11 ATQ
  └── Informs each other (bilateral procedure, shared biomechanical logic)
      Both informed by: P-01 (OA), P-04 (Osteoporose), P-08 (Sarcopenia)

P-02 Lombalgia Crônica
  └── Informs: P-09 (Espondilose), P-12 (Lombalgia Inespecífica)
      [Overlap is high — P-12 may be a variant rather than a separate protocol]

P-17 Neuropatia Periférica
  └── Informs: P-07 (Quedas) — neuropathy is major falls risk factor
      Modified by: P-08 (Sarcopenia)

P-14 Assoalho Pélvico
  └── Informs: P-12 (Lombalgia Inespecífica) — core stabilization overlap
```

### Shared Assessment Tools Across Protocols

| Tool | Protocols Using It | Layer |
|------|--------------------|-------|
| TUG (Timed Up and Go) | All 20 | Universal baseline |
| SPPB (Short Physical Performance Battery) | All 20 | Universal baseline |
| Dinamometria Manual | All 20 | Universal baseline |
| Berg Balance Scale | P-03, P-06, P-07, P-18 | Neuromotor cluster |
| WOMAC | P-01, P-09, P-10, P-11, P-20 | OA/Arthroplasty cluster |
| NRS/VAS Pain | All pain-related (P-01, 02, 09, 12, 13, 19, 20) | Pain monitoring |
| Borg Scale (RPE) | P-15, P-16, all resistance protocols | Cardiorespiratory safety |
| Hoehn & Yahr | P-06 | Parkinson-specific |
| MoCa / MMSE | P-18 | Dementia-specific |
| Tinetti | P-07, P-03, P-06 | Falls cluster |
| 6MWT | P-15, P-16 | Cardiorespiratory cluster |
| MRC Muscle Scale | P-08, P-17 | Muscle weakness |

**Confidence:** HIGH — These are the validated, guideline-endorsed tools for their respective conditions as of 2025.

---

## Suggested Build Order

Build order follows the dependency graph above. Earlier protocols generate reusable architectural decisions (template refinement, parameter formats, cross-reference conventions) and clinical knowledge blocks that later protocols consume.

### Tier 1 — Foundation Protocols (Build First)

These establish the template AND generate knowledge blocks used by many later protocols.

| Order | Protocol | Why First |
|-------|----------|-----------|
| 1 | P-01 Osteoartrite | Broadest evidence base; establishes the document template; kinesiotherapy/manual therapy framework used by 6+ later protocols |
| 2 | P-08 Sarcopenia | Modifies resistance training dosing in every subsequent protocol; must be defined early so all later protocols can reference it |
| 3 | P-04 Osteoporose | Bone quality constraints govern all fracture, arthroplasty, and vertebral protocols; critical safety layer |
| 4 | P-07 Quedas / Síndrome Pós-Queda | Fall risk stratification is referenced in all neuromotor and frailty protocols; establishes balance intervention hierarchy |

### Tier 2 — High-Dependency Protocols (Build Second)

These depend on Tier 1 knowledge AND generate knowledge for Tier 3.

| Order | Protocol | Dependencies |
|-------|----------|-------------|
| 5 | P-05 Fratura de Fêmur Proximal | P-04 (bone quality), P-08 (sarcopenia), P-07 (falls prevention) |
| 6 | P-10 ATJ Pós-op | P-01 (OA progression), P-04 (bone), P-08 (sarcopenia) |
| 7 | P-11 ATQ Pós-op | P-05 (proximal femur logic), P-10 (bilateral arthroplasty pattern), P-04 |
| 8 | P-03 AVC Crônico | P-07 (balance/falls), establishes neuroplasticity framework for P-06 and P-18 |
| 9 | P-06 Doença de Parkinson | P-03 (neuroplasticity), P-07 (falls), P-08 (sarcopenia) |
| 10 | P-15 DPOC | Standalone cardiorespiratory; establishes exercise intensity/monitoring framework for P-16 |
| 11 | P-16 Insuficiência Cardíaca | P-15 (cardiorespiratory framework); generates cardiac precaution block used by all remaining |

### Tier 3 — Secondary Musculoskeletal Protocols

| Order | Protocol | Dependencies |
|-------|----------|-------------|
| 12 | P-02 Lombalgia Crônica + Estenose | P-01 (kinesiotherapy template), P-04 (bone) |
| 13 | P-09 Espondilose | P-02 (overlap high; refine rather than rebuild) |
| 14 | P-12 Lombalgia Inespecífica | P-02 (high overlap; differentiate clearly) |
| 15 | P-19 Fraturas Vertebrais | P-04 (osteoporosis), P-02 (spinal rehab logic) |
| 16 | P-13 Síndrome do Ombro Doloroso | P-01 (OA/kinesiotherapy), P-08 (sarcopenia context) |
| 17 | P-20 Gonalgia / Coxalgia Degenerativa | P-01 (OA is primary diagnosis; P-20 may be refinement or differentiation) |

### Tier 4 — Specialized / Complex Protocols

| Order | Protocol | Dependencies |
|-------|----------|-------------|
| 18 | P-17 Neuropatia Periférica | P-08 (sarcopenia), P-07 (falls); specialized neuropathic pain framework |
| 19 | P-18 Demência / Alzheimer | P-03 (neuroplasticity), P-06 (motor-cognitive coupling), P-07 (falls) |
| 20 | P-14 Assoalho Pélvico | Relatively standalone; P-12 (core overlap); pelvic floor is specialized domain |

**Build order rationale:** The sequence front-loads the protocols with the widest downstream influence (OA, Sarcopenia, Osteoporosis, Falls) so that by the time the 5th protocol is drafted, the author has a stable, validated template and a set of clinical knowledge blocks to cross-reference rather than re-derive.

**Confidence:** MEDIUM-HIGH — Based on established clinical knowledge dependency logic. The specific ordering within tiers is a judgment call; the tier groupings are HIGH confidence.

---

## Component Boundaries

| Component | Responsibility | Boundary |
|-----------|---------------|----------|
| Shared Foundation Layer | Universal baseline assessments, progression principle, evidence standard, comorbidity interaction table | Defined once; referenced by all 20 protocols. Changes here propagate to all. |
| Individual Protocol Document | Complete, self-contained clinical guidance for one comorbidity | Must be usable in isolation (clinician without other documents). Cross-references are optional depth. |
| Phase Block | Clinical guidance for one rehabilitation phase within a protocol | Entry criteria, dosing, progression rules, exit criteria. Phase is the atomic unit of clinical decision-making. |
| Dosing Parameter Block | Exercise parameters with recommended value + acceptable range | Two-column format; always includes units, timeframe, and adjustment trigger. |
| Cross-Reference Index | Maps which protocols interact, which tools are shared | Maintained as Appendix or standalone reference document. Critical for multi-morbid patients. |

### Critical Boundary Rules

1. Each protocol is self-contained. A clinician should not need to read another protocol to treat a single-condition patient. Cross-references add depth but are not required reading.

2. Phase exit criteria must be objective, not time-based. "4 weeks" is insufficient; "TUG < 12 seconds AND NRS pain < 3" is correct. This is architectural, not stylistic.

3. The universal baseline battery (TUG, SPPB, Manual Dynamometry) is never modified within individual protocols. It may be supplemented but not replaced. This ensures comparability across all 20 protocols.

4. Comorbidity interaction notes within each protocol must reference, not duplicate. If osteoporosis modifies arthroplasty post-op care, P-10 and P-11 say "see P-04" plus a one-line modifier, not a full re-derivation.

---

## Data Flow Through the Protocol System

```
PATIENT ENCOUNTER
       ↓
UNIVERSAL BASELINE ASSESSMENT
(TUG + SPPB + Dynamometry → functional profile)
       ↓
CONDITION-SPECIFIC ASSESSMENT
(Tools from Section 2.2 of relevant protocol)
       ↓
COMORBIDITY SCREENING
(Which other protocols apply? → consult Cross-Reference Index)
       ↓
PHASE ENTRY DETERMINATION
(Match patient profile to Phase Entry Criteria in primary protocol)
       ↓
INTERVENTION SELECTION
(Phase block: modalities + manual therapy + kinesiotherapy + dosing)
       ↓
PROGRESSION MONITORING
("Start low, go slow" → weekly dosing adjustment against benchmarks)
       ↓
PHASE TRANSITION GATE
(Exit criteria met? → advance; Not met? → hold or regress)
       ↓
FINAL OUTCOME MEASUREMENT
(TUG/SPPB benchmarks + condition-specific outcome tools)
       ↓
DISCHARGE OR MAINTENANCE PHASE
```

This flow is identical for all 20 protocols. The content of each step differs by condition; the architecture does not.

---

## Scalability Considerations

| Concern | For Single Protocol | For 20-Protocol Corpus |
|---------|--------------------|-----------------------|
| Template drift | N/A | Enforce shared template from Protocol 1; retrofit is painful |
| Cross-reference integrity | N/A | Assign protocol codes (P-01 to P-20) before writing any; use codes not titles |
| Multi-morbid patients | One protocol + comorbidity notes | Cross-Reference Index becomes essential; consider a "Multi-Morbidity Appendix" |
| Evidence updates | Update one protocol | Flag protocols sharing the same foundational study; updates may cascade |
| Language consistency | N/A | Maintain a clinical terminology glossary (Portuguese terms) shared across all protocols |

---

## Anti-Patterns to Avoid

### Anti-Pattern 1: Time-Based Phase Progression
**What:** "Phase 1 lasts 2 weeks, Phase 2 lasts 4 weeks."
**Why bad:** Older adults have highly variable recovery rates. Time-based criteria lead to premature advancement (injury risk) or prolonged restriction (deconditioning). This is directly contradicted by current geriatric rehabilitation evidence.
**Instead:** Function-based exit criteria using validated outcome measures (TUG, SPPB benchmarks).

### Anti-Pattern 2: Single Dosing Column (No Range)
**What:** "3 sets, 10 reps, 3x/week" with no range.
**Why bad:** Eliminates clinical judgment, ignores individual variation in frailty/sarcopenia/pain, and violates the "start low" principle by prescribing a fixed dose.
**Instead:** Two-column format — recommended value + acceptable clinical range.

### Anti-Pattern 3: Protocol Isolation (No Cross-References)
**What:** Writing each protocol as if the patient has only one condition.
**Why bad:** 80% of geriatric rehabilitation patients present with 2+ comorbidities. A protocol that ignores osteoporosis while prescribing high-impact loading for an arthroplasty patient is clinically dangerous.
**Instead:** Section 6 (Comorbidity Interactions) in every protocol; Cross-Reference Index maintained separately.

### Anti-Pattern 4: Unanchored Evidence Claims
**What:** "Evidence-based exercises include..." with no citation or level specified.
**Why bad:** Undermines the academic reference function of the corpus. "Level A" means nothing without the source.
**Instead:** Every intervention claim includes evidence level (A/B/C) and primary citation inline, with full references in Section 8.

### Anti-Pattern 5: Rebuilding Shared Knowledge per Protocol
**What:** Re-deriving the "Start low, go slow" progression rules, or the universal baseline assessment rationale, in every protocol.
**Why bad:** Creates inconsistency, bloats documents, and means changes require editing 20 files.
**Instead:** Shared Foundation Layer document. Protocols say "aplicar protocolo de progressão universal (ver Fundamentos)" and add condition-specific modifiers only.

### Anti-Pattern 6: Merging High-Overlap Protocols Without Differentiation
**What:** Writing P-02 (Lombalgia Crônica) and P-12 (Lombalgia Inespecífica) as near-identical documents.
**Why bad:** If they overlap 90%, one is a subset or variant — not a separate protocol. Having two nearly identical protocols creates confusion about when to use which.
**Instead:** Before drafting P-12, explicitly define what distinguishes it from P-02. If the difference is only pathological classification but not clinical management, consider whether P-12 is a section within P-02 rather than a standalone document.

---

## Phase-Specific Architecture Notes by Protocol Cluster

### Musculoskeletal Cluster (P-01, 05, 09, 10, 11, 13, 19, 20)
- Phase count: typically 3 (Aguda → Fortalecimento → Funcional)
- Arthroplasty protocols (P-10, P-11) may need 4 phases: Pós-operatório Imediato is distinct
- Key structural element: weight-bearing progression must be explicit (% body weight, assistive device weaning)

### Neuromotor Cluster (P-03, P-06, P-07, P-18)
- Phase count: typically 3-4; Parkinson and Dementia may need 4 (disease progression stages alter protocol)
- Key structural element: dual-task training must appear as a distinct sub-category within kinesiotherapy (motor + cognitive simultaneously)
- Balance intervention must follow a hierarchy: static → dynamic → dual-task → perturbation training

### Cardiorespiratory Cluster (P-15, P-16)
- Phase count: typically 3 (Estabilização → Condicionamento → Manutenção)
- Key structural element: exercise intensity expressed in MET equivalents AND Borg RPE simultaneously (not either/or)
- Session structure must be explicit: warm-up (5 min) + conditioning (20-45 min) + cool-down (5 min) with specific intensity for each segment

### Chronic Pain Cluster (P-02, P-12)
- Phase count: typically 3; chronic pain may not have a clear "acute phase"
- Key structural element: pain neuroscience education (PNE) is an intervention, not just psychosocial context — must appear in Section 5
- Outcome measures must include both pain AND function (NRS alone is insufficient)

### Metabolic/Neuropathic Cluster (P-08, P-17)
- Phase count: P-08 typically 3; P-17 may need 4 (sensory re-education is a distinct early phase)
- Key structural element: safety screening for peripheral neuropathy (skin inspection, footwear, vibration threshold) must be in Section 2 assessment

---

## Sources

**Note:** Web access was unavailable. The following authoritative sources inform this architecture document and should be verified against current versions:

- WHO Rehabilitation Programme. *Package of Interventions for Rehabilitation*. WHO, 2023 (HIGH confidence for assessment battery and phase structure principles).
- American Geriatrics Society (AGS). *Geriatrics at Your Fingertips*, 2024 edition (HIGH confidence for comorbidity management principles).
- American Physical Therapy Association (APTA). Clinical Practice Guidelines for OA, Falls, Stroke (HIGH confidence for condition-specific protocol structure).
- Fried LP et al. *Frailty in older adults* (Cardiovascular Health Study criteria — HIGH confidence for sarcopenia/frailty integration).
- IASP Terminology and Guidelines for Chronic Pain (HIGH confidence for pain classification and outcome measure standards).
- Sherrington C et al. Cochrane review on exercise and falls prevention (HIGH confidence for balance intervention hierarchy).
- Training knowledge: clinical protocol authoring standards from rehabilitation medicine literature through August 2025 (MEDIUM confidence for synthesis and build order recommendations).
