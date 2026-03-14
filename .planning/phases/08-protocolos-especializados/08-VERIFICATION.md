---
phase: 08-protocolos-especializados
verified: 2026-03-14T13:00:00Z
status: passed
score: 11/11 must-haves verified
re_verification: false
human_verification:
  - test: "Review clinical accuracy of SE-1 to SE-4 sensory re-education hierarchy in P-17"
    expected: "Hierarchy is clinically appropriate for DPN patients with peripheral proprioceptive loss, correctly restricting foam pad to low-density and prohibiting wobble board/BOSU in confirmed loss of protective sensation"
    why_human: "MEDIUM-confidence annotation is honest — no single guideline consolidates this exact SE-1/SE-4 progression hierarchy. A geriatric PT specialist should confirm the clinical logic of substituting visual channel for lost proprioception at each SE level."
  - test: "Review clinical accuracy of pre-session glucose thresholds in P-17 (< 90 / 90-250 / 250-300 / > 300 mg/dL)"
    expected: "Operational thresholds are appropriate for PT ambulatorial context and consistent with Colberg 2016 recommendations, with MEDIUM-confidence note clearly stated"
    why_human: "MEDIUM-confidence annotation is correct — ADA 2025 does not publish specific PT-context numerical thresholds. A clinician or diabetologist should confirm the table values are safe for geriatric patients with autonomic neuropathy."
  - test: "Verify P-14 Passo 0 Estrutural classification framework usability in clinical practice"
    expected: "A physiotherapist can classify hypertonic vs. hypotonic pelvic floor using the Modified Oxford Scale + PERFECT Scheme + palpation framework in Section 1.4 without requiring external reference"
    why_human: "The framework involves internal vaginal assessment technique — clinical completeness and instruction adequacy for a PT setting requires hands-on professional evaluation."
---

# Phase 8: Protocolos Especializados — Verification Report

**Phase Goal:** Create specialized protocols P-17 (Neuropatia Periférica Diabética) and P-14 (Disfunção do Assoalho Pélvico), and complete the cross-reference index.
**Verified:** 2026-03-14T13:00:00Z
**Status:** PASSED
**Re-verification:** No — initial verification

---

## Goal Achievement

### Observable Truths

| # | Truth | Status | Evidence |
|---|-------|--------|----------|
| 1 | P-17 includes a pre-session glucose check protocol with 4-tier thresholds (< 90 / 90-250 / 250-300 / > 300 mg/dL) and condutas | VERIFIED | 27 matches for `glicemia\|glicosimetro\|hipoglicemia`; Section 2.3 contains explicit 4-tier table with action per tier |
| 2 | P-17 includes sensory re-education hierarchy SE-1 through SE-4 referencing P-07 Section 7.2 with NPD adaptations | VERIFIED | 72 matches for SE-1/SE-2/SE-3/SE-4; 10 matches for "P-07.*Seção 7.2"; explicit adaptation note in Section 5.3 |
| 3 | P-17 includes mandatory pre-session foot inspection procedure per ADA 2025 | VERIFIED | 12 matches for foot inspection terms; Section 2.4 documents bilateral 2–3 min inspection + monofilament mapping |
| 4 | P-17 includes MNSI and monofilament 10g as inclusion/assessment instruments | VERIFIED | 26 matches for `monofilamento\|MNSI`; MNSI cited Feldman 1994 PMID 7821168 with MEDIUM confidence note |
| 5 | P-17 includes NPD-specific red flags (diabetic foot ulcer, hypoglycemia, critical limb ischemia, acute foot drop, autonomic instability) | VERIFIED | 13 matches; Section 9.1 contains 8 specific red flags with immediate action for each |
| 6 | P-17 is a complete 15-section protocol in Brazilian Portuguese with frailty-stratified dosage tables, NÃO COBRE block, universal Section 11, and all 8 clinical validity questions | VERIFIED | 956 lines; 15 section headers confirmed; 13 matches for Robusto/Pré-frágil/Frágil; 4 matches for "NÃO COBRE"; Section 11 at line 678; Q1–Q8 present |
| 7 | P-14 differentiates hypertonic vs. hypotonic pelvic floor as mandatory Step 0 (Passo 0 Estrutural) BEFORE any exercise selection | VERIFIED | 5 matches for "Passo 0"; 30 matches for hipertônico/hipotônico; Section 1.4 contains full classification framework |
| 8 | P-14 cites ICIQ-SF-BR with PMID 15243675 (Tamanini 2004) as primary outcome instrument | VERIFIED | 15 matches for `ICIQ-SF\|15243675\|Tamanini` |
| 9 | P-14 uses Modified Oxford Grading Scale and PERFECT Scheme for pelvic floor muscle assessment | VERIFIED | 4 matches for Modified Oxford; 6 matches for PERFECT |
| 10 | P-14 prescribes down-training for hypertonic and PFMT for hypotonic with explicit Kegel contraindication in hypertonic | VERIFIED | 34 matches for down-training/relaxamento; 4 matches for CONTRAINDICAÇÃO; "CONTRAINDICAÇÃO ABSOLUTA" callout embedded in Fase 1 Via Hipertônico section |
| 11 | SHARED-FOUNDATION Section 8.1 has all 20 rows complete — P-14 and P-17 rows fully populated | VERIFIED | Status line 609: "20/20 — COMPLETO"; P-17 row at line 631 contains 5 interaction pathways, full safety infrastructure; P-14 row at line 628 contains 4 interaction pathways, Passo 0 warning, iatrogenic warning |

**Score:** 11/11 truths verified

---

### Required Artifacts

| Artifact | Expected | Status | Details |
|----------|----------|--------|---------|
| `protocols/P-17-NEUROPATIA-PERIFERICA-DIABETICA.md` | Complete P-17 protocol for diabetic peripheral neuropathy | VERIFIED | 956 lines; substantive clinical content; Portuguese; 15 sections |
| `protocols/P-14-DISFUNCAO-ASSOALHO-PELVICO.md` | Complete P-14 protocol for pelvic floor dysfunction | VERIFIED | 721 lines; substantive clinical content; Portuguese; 15 sections |
| `protocols/SHARED-FOUNDATION.md` | Complete 20-protocol cross-reference index in Section 8.1 | VERIFIED | 662 lines; P-14 row at line 628; P-17 row at line 631; status "20/20 — COMPLETO" at line 609 |

---

### Key Link Verification

| From | To | Via | Status | Details |
|------|----|-----|--------|---------|
| `P-17-NEUROPATIA-PERIFERICA-DIABETICA.md` | `P-07-QUEDAS.md` | P-07 Seção 7.2 balance hierarchy with SE-1 to SE-4 adaptations | VERIFIED | Lines 143, 257, 338, 340, 789 — explicit references to "P-07 Seção 7.2" with SE hierarchy adaptation notes |
| `P-17-NEUROPATIA-PERIFERICA-DIABETICA.md` | `P-08-SARCOPENIA.md` | P-08 Seção 6.3 resistance dosing modifier for distal amyotrophy | VERIFIED | Lines 145, 258, 287, 403, 433 — conditional activation on dynamometry threshold |
| `P-17-NEUROPATIA-PERIFERICA-DIABETICA.md` | `P-04-OSTEOPOROSE.md` | P-04 Seção 5.2 bone-loading constraints | VERIFIED | Lines 259, 286, 496, 804 — bone load ceiling constraint for coexistent osteoporosis |
| `P-14-DISFUNCAO-ASSOALHO-PELVICO.md` | `P-07-QUEDAS.md` | P-07 Seção 5.2 fall risk when urge incontinence increases fall risk | VERIFIED | Lines 126, 139, 148, 149, 553 — FES-I-BR >= 23 and TUG > 13.5 s trigger P-07 Section 5.2 |
| `P-14-DISFUNCAO-ASSOALHO-PELVICO.md` | `P-08-SARCOPENIA.md` | P-08 Seção 6.3 resistance dosing modifier for pelvic sarcopenia | VERIFIED | Lines 128, 314, 561, 579, 675 — Oxford <= 2 triggers modifier |
| `SHARED-FOUNDATION.md` | `P-17-NEUROPATIA-PERIFERICA-DIABETICA.md` | P-17 row in Section 8.1 cross-reference index | VERIFIED | Line 631 — full row with interaction pathways, safety infrastructure, safety warnings |
| `SHARED-FOUNDATION.md` | `P-14-DISFUNCAO-ASSOALHO-PELVICO.md` | P-14 row in Section 8.1 cross-reference index | VERIFIED | Line 628 — full row with Passo 0 structural requirement, PFMT contraindication warning |

Cross-referenced sections confirmed to exist in target protocols:
- P-07 Section 5.2 (INFRAESTRUTURA DE SEGURANÇA — PROTOCOLO DE RISCO DE QUEDA POR SESSÃO): confirmed at line 276
- P-07 Section 7.2 (Tabela de Hierarquia de Intervenção de Equilíbrio): confirmed at line 561
- P-08 Section 6.3 (Tabela de Dosagem de Exercício Resistido — MODIFICADOR TRANSVERSAL): confirmed at line 419
- P-04 Section 5.2 (MODIFICADOR TRANSVERSAL — Tabela de Restrições de Carga Óssea): confirmed at line 322

---

### Requirements Coverage

| Requirement | Source Plan | Description | Status | Evidence |
|-------------|------------|-------------|--------|---------|
| PROT-19 | 08-01-PLAN.md, 08-03-PLAN.md | P-17 Neuropatia Periférica (diabética) | SATISFIED | `protocols/P-17-NEUROPATIA-PERIFERICA-DIABETICA.md` — 956-line complete protocol. Commits: `4b59e82` (protocol), `a0c52f4` (docs) |
| PROT-20 | 08-02-PLAN.md, 08-03-PLAN.md | P-14 Disfunção do Assoalho Pélvico | SATISFIED | `protocols/P-14-DISFUNCAO-ASSOALHO-PELVICO.md` — 721-line complete protocol. Commits: `e538f72` (protocol), `581715c` (docs) |

**Note — REQUIREMENTS.md traceability table inconsistency:** The checklist section of REQUIREMENTS.md (lines 67-68) correctly marks PROT-19 and PROT-20 as `[x]` done. However, the traceability table at the bottom (lines 142-143) still reads "Pending" for both. This is a documentation maintenance gap only — it does not affect the protocols themselves and should be corrected in REQUIREMENTS.md.

---

### Anti-Patterns Found

| File | Pattern | Severity | Impact |
|------|---------|----------|--------|
| All three protocol files | grep for "TODO" returns matches — all are false positives from Portuguese word "Todo/todos" (meaning "all/every") | None | Not a stub or anti-pattern; Portuguese clinical text uses "Todo exercício", "todos os pacientes" |
| `protocols/P-17-NEUROPATIA-PERIFERICA-DIABETICA.md` | Line count 956 vs target 600–750 | Info | SUMMARY documents justified deviation — NAC section, Q1–Q8 rationale, ADA foot inspection verbatim. Clinical completeness prioritized, no content truncated |
| `.planning/REQUIREMENTS.md` | Traceability table rows 142-143 show "Pending" for PROT-19 and PROT-20 despite checklist marking them `[x]` done | Warning | Inconsistency in requirements documentation only — does not affect protocol completeness |

No blocker anti-patterns found.

---

### Human Verification Required

#### 1. SE-1 to SE-4 Sensory Re-Education Hierarchy (P-17)

**Test:** Have a geriatric physiotherapist or neurorehabilitation specialist review the SE-1 through SE-4 hierarchy in P-17 Section 5.3
**Expected:** The progression from SE-1 (firm surface, eyes open as substitute proprioceptive channel) through SE-4 (external environment, direct supervision) is clinically appropriate for DPN patients with confirmed loss of protective sensation; NUNCA wobble board/BOSU restriction is confirmed as correct
**Why human:** Protocol carries a MEDIUM-confidence annotation — no single published guideline consolidates this exact hierarchy with these labels. Derived from PMC12069999, PMC12167735, and P-07 Section 7.2 adaptation.

#### 2. Pre-Session Glucose Thresholds (P-17)

**Test:** Have a diabetologist or endocrinologist confirm the 4-tier operational table in P-17 Section 2.3 (< 90 / 90-250 / 250-300 / > 300 mg/dL with corresponding condutas)
**Expected:** Thresholds are safe and consistent with Colberg 2016 position statement for aerobic and resistance exercise in diabetes; MEDIUM-confidence annotation is appropriately calibrated
**Why human:** ADA 2025 does not publish specific PT-ambulatorial operational thresholds. The values are derived from Colberg 2016 + clinical consensus, which the protocol correctly documents. Numerical safety thresholds for glycemia in exercise require clinical expert confirmation.

#### 3. Passo 0 Estrutural Clinical Usability (P-14)

**Test:** A pelvic floor physiotherapist should review P-14 Section 1.4 classification framework and the diagnostic differentiation table
**Expected:** Modified Oxford Grading Scale + PERFECT Scheme + palpation instructions are sufficient for a PT to perform Passo 0 without additional training materials; routing to down-training vs. PFMT track is unambiguous
**Why human:** Internal vaginal assessment technique and the clinical adequacy of written instructions for this specialized assessment cannot be verified programmatically.

---

### Gaps Summary

No gaps. All 11 observable truths verified, all 3 artifacts confirmed as substantive non-stub documents, all 7 key links verified with actual content and section existence confirmed in target protocols, requirements PROT-19 and PROT-20 satisfied.

The three human verification items relate to MEDIUM-confidence clinical content that the protocol itself already correctly flags — they do not represent implementation gaps but rather appropriately annotated areas of clinical uncertainty requiring specialist sign-off before production use.

The only maintenance item is updating the REQUIREMENTS.md traceability table rows 142-143 from "Pending" to reflect Phase 8 completion.

---

_Verified: 2026-03-14T13:00:00Z_
_Verifier: Claude (gsd-verifier)_
