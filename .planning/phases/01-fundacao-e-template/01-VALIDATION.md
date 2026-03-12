---
phase: 1
slug: fundacao-e-template
status: draft
nyquist_compliant: false
wave_0_complete: false
created: 2026-03-12
---

# Phase 1 — Validation Strategy

> Per-phase validation contract for feedback sampling during execution.

---

## Test Infrastructure

| Property | Value |
|----------|-------|
| **Framework** | Manual clinical review (documentation/specification project — no automated test suite) |
| **Config file** | None |
| **Quick run command** | N/A — reviewer reads document against checklist |
| **Full suite command** | N/A — full 8-question clinical validity checklist |
| **Estimated runtime** | ~15 minutes per document (manual review) |

---

## Sampling Rate

- **After every task commit:** Review document section against requirement checklist
- **After every plan wave:** Full 8-question clinical validity checklist pass on P-01
- **Before `/gsd:verify-work`:** All requirements verified against produced documents
- **Max feedback latency:** N/A (manual review — no automated latency target)

---

## Per-Task Verification Map

| Task ID | Plan | Wave | Requirement | Test Type | Method | Status |
|---------|------|------|-------------|-----------|--------|--------|
| 1-01-01 | 01 | 1 | STRUC-05 | Manual review | Foundation Layer document exists with all 8 sections | ⬜ pending |
| 1-01-02 | 01 | 1 | ASMNT-01 | Manual review | TUG/SPPB/Dynamometry norms + MCIDs present | ⬜ pending |
| 1-01-03 | 01 | 1 | ASMNT-04 | Manual review | All tools cited with "-BR" suffix + validation citation | ⬜ pending |
| 1-01-04 | 01 | 1 | EVID-01 | Manual review | Oxford CEBM grading standard defined | ⬜ pending |
| 1-01-05 | 01 | 1 | DOSE-01 | Manual review | Two-column format specification present | ⬜ pending |
| 1-01-06 | 01 | 1 | DOSE-03 | Manual review | Frailty-stratified table template defined | ⬜ pending |
| 1-02-01 | 02 | 2 | STRUC-01 | Manual review | P-01 has ACR criteria + inclusion/exclusion | ⬜ pending |
| 1-02-02 | 02 | 2 | STRUC-02 | Manual review | Red flag table with ≥5 entries + escalation | ⬜ pending |
| 1-02-03 | 02 | 2 | STRUC-03 | Manual review | ≥2 phases with functional entry/exit criteria | ⬜ pending |
| 1-02-04 | 02 | 2 | STRUC-04 | Manual review | Interventions classified by Modalidade/Manual/Cinesioterapia | ⬜ pending |
| 1-02-05 | 02 | 2 | DOSE-02 | Manual review | "Start low, go slow" principle operationalized | ⬜ pending |
| 1-02-06 | 02 | 2 | DOSE-04 | Manual review | Functional progression criteria (not time-only) | ⬜ pending |
| 1-02-07 | 02 | 2 | EVID-02 | Manual review | OARSI 2019 + ACR 2022 alignment declarations | ⬜ pending |
| 1-02-08 | 02 | 2 | EVID-03 | Manual review | Sources from PubMed + Cochrane + PEDro triad | ⬜ pending |
| 1-02-09 | 02 | 2 | SAFE-01 | Manual review | NRS thresholds table with 3 phase rows | ⬜ pending |
| 1-02-10 | 02 | 2 | SAFE-02 | Manual review | Red flag table matching template format | ⬜ pending |
| 1-02-11 | 02 | 2 | SAFE-03 | Manual review | Polypharmacy section with ≥4 drug classes | ⬜ pending |
| 1-02-12 | 02 | 2 | SAFE-04 | Manual review | Cardiorespiratory precautions section present | ⬜ pending |
| 1-02-13 | 02 | 2 | OUT-01 | Manual review | Entire P-01 in Brazilian Portuguese | ⬜ pending |
| 1-02-14 | 02 | 2 | OUT-02 | Manual review | Single structured markdown document | ⬜ pending |
| 1-02-15 | 02 | 2 | OUT-03 | Manual review | TIDieR/CERT compliance checklist pass | ⬜ pending |
| 1-02-16 | 02 | 2 | OUT-04 | Manual review | Cross-reference index with comorbidity flags | ⬜ pending |
| 1-02-17 | 02 | 2 | PROT-01 | Manual review | P-01 answers all 8 clinical validity questions | ⬜ pending |
| 1-02-18 | 02 | 2 | ASMNT-02 | Manual review | Primary outcomes per phase + re-evaluation schedule | ⬜ pending |
| 1-02-19 | 02 | 2 | ASMNT-03 | Manual review | Functional benchmark targets at phase transitions | ⬜ pending |

*Status: ⬜ pending · ✅ green · ❌ red · ⚠️ flaky*

---

## Wave 0 Requirements

- [ ] No existing documents — all content is greenfield
- [ ] Clinical reviewer designation needed before final sign-off
- [ ] Open questions from RESEARCH.md should be explicitly flagged in documents as "verificar antes de publicação definitiva"

*Documentation project — no test framework installation needed.*

---

## Manual-Only Verifications

| Behavior | Requirement | Why Manual | Test Instructions |
|----------|-------------|------------|-------------------|
| Clinical accuracy of dosage parameters | DOSE-01, DOSE-03 | Dosage values require clinical domain expertise | Clinician reviews dosage tables against OARSI 2019 + ACR 2022 recommendations |
| Evidence level assignment correctness | EVID-01 | Correct mapping of citations to Oxford CEBM levels requires literature review | Cross-check each intervention's cited level against source study design |
| Brazilian Portuguese terminology | OUT-01, ASMNT-04 | Language accuracy requires native speaker review | Native PT-BR clinician reviews all clinical terminology |
| 8-question clinical validity completeness | PROT-01 | Subjective assessment of whether each question is "unambiguously answered" | Reviewer attempts to answer each question using only P-01; gaps = fail |
| TIDieR/CERT compliance | OUT-03 | Requires checklist walkthrough against standard items | Walk through TIDieR 12-item + CERT 16-item checklists against P-01 |

*All verifications are manual for this documentation project.*

---

## Validation Sign-Off

- [ ] All tasks have manual verification method assigned
- [ ] Sampling continuity: every requirement has a verification row
- [ ] Wave 0 covers all greenfield gaps
- [ ] No automated test dependencies (documentation project)
- [ ] Feedback latency: N/A (manual)
- [ ] `nyquist_compliant: true` set in frontmatter

**Approval:** pending
