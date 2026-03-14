---
phase: 08-protocolos-especializados
plan: "01"
subsystem: protocols
tags: [geriatric-rehabilitation, diabetic-neuropathy, metabolic-safety, fall-prevention, sensory-reeducation]
dependency_graph:
  requires: [P-07-QUEDAS, P-08-SARCOPENIA, P-04-OSTEOPOROSE, SHARED-FOUNDATION]
  provides: [P-17-NEUROPATIA-PERIFERICA-DIABETICA]
  affects: [SHARED-FOUNDATION-section-8.1]
tech_stack:
  added: []
  patterns: [15-section-protocol, frailty-stratified-dosage, SE-hierarchy-NPD, pre-session-safety-infrastructure]
key_files:
  created:
    - protocols/P-17-NEUROPATIA-PERIFERICA-DIABETICA.md
  modified: []
decisions:
  - "Pre-session glucose thresholds (< 90 / 90-250 / 250-300 / > 300 mg/dL) classified as MEDIUM confidence — ADA 2025 recommends glucose monitoring without publishing specific PT-ambulatorial operational thresholds; values derived from Colberg 2016 + clinical consensus"
  - "MNSI-BR validation classified as MEDIUM confidence — original Feldman 1994 instrument (PMID 7821168) cited; specific Brazilian cultural validation PMID not confirmed; verify LILACS before definitive publication"
  - "Sensory re-education hierarchy SE-1 to SE-4 classified as MEDIUM confidence — derived from sensorimotor training evidence (PMC12069999, PMC12167735) + adaptation of P-07 Seção 7.2; no single guideline consolidates this specific hierarchy with these labels"
  - "NUNCA wobble board or BOSU in confirmed loss of protective sensation (monofilament negative) — established as absolute restriction in NPD protocol"
  - "Cardiac autonomic neuropathy (NAC) documented as reason for RPE Borg 6-20 as primary intensity monitor in NPD — same physiological rationale as P-16 with beta-blockers (blunted HR response)"
  - "P-07 integration designated OBRIGATORIO for ALL NPD patients (not conditional) due to 15x elevated fall risk — strongest cross-protocol dependency in the corpus"
metrics:
  duration_minutes: 40
  completed_date: "2026-03-14"
  tasks_completed: 2
  files_created: 1
  files_modified: 0
---

# Phase 8 Plan 01: P-17 Neuropatia Periférica Diabética Summary

**One-liner:** Complete 15-section NPD protocol with mandatory pre-session glucose check (4-tier thresholds from Colberg 2016), sensory re-education hierarchy SE-1 to SE-4 adapting P-07 Seção 7.2, pre-session foot inspection per ADA 2025, and MEDIUM-confidence annotations on derived clinical thresholds.

## What Was Built

`protocols/P-17-NEUROPATIA-PERIFERICA-DIABETICA.md` — 956-line protocol (target was 600–750; extended due to complexity of safety infrastructure documentation and 8-question clinical validity section). Complete 15-section structure following TIDieR/CERT standard established in P-01.

### Key Clinical Content Delivered

**1. INFRAESTRUTURA DE SEGURANÇA — Verificação Glicêmica Pré-Sessão (Seção 2.3)**
4-tier operational table:
- < 90 mg/dL → NÃO INICIAR + 15g HC rápido + remensurar
- 90–250 mg/dL → INICIAR normalmente
- 250–300 mg/dL (sem cetonúria) → INICIAR com cautela, baixa intensidade, monitorar a cada 20 min
- > 300 mg/dL OU cetonúria → NÃO INICIAR + contatar médico

Documented as MEDIUM confidence (Colberg 2016 + clinical consensus, not explicit ADA operational table for PT context).

**2. Hierarquia de Re-educação Sensorial SE-1 a SE-4 (Seção 5.3, 6.2, 7.2, 7.3)**
- SE-1: Superfície firme, olhos abertos, visão como canal substituto à propriocepção
- SE-2: Foam de baixa densidade (máx), olhos abertos prioritariamente, olhos fechados só BBS-BR ≥ 46
- SE-3: Dupla tarefa em superfície FIRME — NUNCA dupla tarefa em superfície instável em NPD
- SE-4: Ambiente externo, terreno variado, supervisão direta obrigatória, calçado ortopédico

Referenced as "progressão de equilíbrio adaptada para déficit sensorial periférico — baseada em P-07 Seção 7.2 com modificações para NPD" — MEDIUM confidence noted.

**3. Procedimento Mandatório de Inspeção dos Pés (Seção 2.4)**
Protocol integrated pre-session: visual inspection (2–3 min bilateral) + calçado verification + monthly monofilament mapping + immediate action when lesion found (suspend orthostatism → adapt to sedestação).

**4. Instrumentos MNSI + Monofilamento 10g (Seções 1.2, 1.3, 2.2)**
MNSI: Feldman 1994 (PMID 7821168) with MEDIUM confidence note on BR validation. Monofilament: 10-point mapping with 3-tier risk classification (preservada/reduzida/perdida) linked to SE level restrictions.

**5. Bandeiras Vermelhas NPD-Específicas (Seção 9.1)**
8 specific red flags with immediate action:
- Úlcera de pé (any Wagner grade) → suspend ortostatismo + pé diabético referral
- Hipoglicemia sintomática → glicemia + ADA protocol → SAMU if no improvement
- Hipoglicemia silenciosa (autonômica) → treat as above; document for medical review
- Dor isquêmica em repouso + ausência de pulso → SAMU 192
- Foot drop agudo → neurologia urgente
- Hipotensão ortostática sintomática → deitar + monitorar + SAMU if no reversal
- Cetonúria → NÃO INICIAR + médico imediatamente
- Eritema/calor localizado no pé → suspend carga + médico no mesmo dia

**6. Neuropatia Autonômica Cardíaca (NAC) — Precaução Única de P-17 (Seção 11.5)**
NAC documented with 4 manifestations (taquicardia de repouso, FC atenuada, hipotensão pós-exercício, isquemia silenciosa). RPE Borg 6–20 designated primary intensity monitor — same rationale as P-16 (beta-blocker-induced HR blunting).

**7. Polifarmácia (Seção 10)**
7 drug classes: insulinas/secretagogos (glucose check mandatory), metformina (B12 depletion → worsens neuropathy), gabapentinoides (fall risk per Beers 2023), duloxetina/amitriptilina (orthostatic hypotension), anti-hipertensivos/betabloqueadores (RPE-only when beta-blocker active), estatinas (myalgia differentiation), opioides.

**8. Cross-Protocol Modifier Chain**
- P-04 Seção 5.2 (if osteoporosis): bone loading constraints
- P-08 Seção 6.3 (if sarcopenia/distal amyotrophy): resistance dosing modifier
- P-07 Seções 5.2 + 7.2 (MANDATORY ALL patients): session safety protocol + balance hierarchy SE adaptations

## Decisions Made

1. **MEDIUM confidence on glucose thresholds:** ADA 2025 recommends monitoring without publishing specific PT-ambulatorial numerical thresholds. Table derived from Colberg 2016 + clinical consensus. Documented with explicit note — not cited as "ADA explicit guideline."

2. **MEDIUM confidence on MNSI-BR:** Original Feldman 1994 instrument valid internationally; specific Brazilian cultural validation PMID not confirmed in this research. Cited as "adapted for clinical use in Brazil" — verify LILACS before definitive publication.

3. **MEDIUM confidence on SE-1 to SE-4 hierarchy:** No single guideline consolidates this specific progression with these labels. Derived from sensorimotor training evidence in DPN + P-07 adaptation. Documented explicitly.

4. **Absolute restriction NUNCA wobble board/BOSU in confirmed loss of protective sensation:** Physiological rationale documented in Q8 — loss of peripheral proprioceptive channel means high-instability surface exceeds compensatory capacity of visual and vestibular systems.

5. **P-07 OBRIGATÓRIO for ALL NPD patients:** Not conditional — the 15x elevated fall risk magnitude requires the full session safety infrastructure and balance hierarchy for all patients regardless of functional status.

6. **Line count exceeds target (956 vs 600–750):** Safety documentation complexity, NAC section, 8-question clinical validity section with detailed rationale, and NPD-specific red flags table required more space. Clinical completeness prioritized.

## Deviations from Plan

None — plan executed exactly as written. Both tasks (research synthesis and protocol authorship) were combined as the research was already compiled in 08-RESEARCH.md. The protocol was authored directly using the pre-researched content.

**Line count deviation:** Protocol is 956 lines vs target 600–750. The additional length comes from:
- NAC (cardiac autonomic neuropathy) subsection in Section 11.5 — not explicitly in the plan but required by the Section 11 template instruction to add NPD-specific cardiorespiratory content
- Detailed Q8 rationale for each major design decision (why glucose check, why SE-1, why NUNCA wobble board, etc.)
- Full foot inspection protocol verbatim (ADA 2025 compliance)
This is a justified deviation under Rule 2 (missing critical functionality) — clinical completeness takes priority.

## Self-Check: PASSED

- FOUND: `protocols/P-17-NEUROPATIA-PERIFERICA-DIABETICA.md` (956 lines)
- FOUND: `.planning/phases/08-protocolos-especializados/08-01-SUMMARY.md`
- FOUND: commit `4b59e82` — feat(08-01): create P-17 Neuropatia Periferica Diabetica protocol
