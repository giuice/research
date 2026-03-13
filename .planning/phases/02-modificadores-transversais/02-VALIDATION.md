---
phase: 2
slug: modificadores-transversais
status: draft
nyquist_compliant: false
wave_0_complete: false
created: 2026-03-13
---

# Phase 2 — Validation Strategy

> Per-phase validation contract for feedback sampling during execution.

---

## Test Infrastructure

| Property | Value |
|----------|-------|
| **Framework** | Manual clinical review (no automated test suite — documentation project) |
| **Config file** | None |
| **Quick run command** | N/A — reviewer reads document against protocol checklist |
| **Full suite command** | N/A — manual review of all 15 sections |
| **Estimated runtime** | ~15 minutes per protocol (manual review) |

---

## Sampling Rate

- **After every task commit:** Reviewer checks modified section against protocol checklist
- **After every plan wave:** Full manual review of all 15 sections per protocol
- **Before `/gsd:verify-work`:** Full review must confirm all sections present and compliant
- **Max feedback latency:** N/A (manual review)

---

## Per-Task Verification Map

| Task ID | Plan | Wave | Requirement | Test Type | Method | File Exists | Status |
|---------|------|------|-------------|-----------|--------|-------------|--------|
| 02-01-XX | 01 | 1 | PROT-02 | Manual review | Confirm FACS algorithm present; dosage table has 3 Fried frailty rows; modifier label present; protein-exercise section with dietitian pathway | ❌ W0 | ⬜ pending |
| 02-01-XX | 01 | 1 | PROT-02 | Manual review | Count drug class rows in P-08 polypharmacy table: must be ≥ 9 entries total (baseline 6 + statins, aromatase inhibitors, diuretics) | ❌ W0 | ⬜ pending |
| 02-02-XX | 02 | 1 | PROT-03 | Manual review | Confirm bone-loading table has 4 risk rows; FRAX referenced alongside T-score; 3 constraint axes (espinal/impacto/resistência); modifier label | ❌ W0 | ⬜ pending |
| 02-02-XX | 02 | 1 | PROT-03 | Manual review | Search P-04 for "P-08" cross-reference in kinesiotherapy dosage section | ❌ W0 | ⬜ pending |
| 02-01+02 | 01,02 | 1 | PROT-02 + PROT-03 | Manual review | Checklist per protocol: who qualifies, when stop, where start, what to do, how much, how fast, how to measure, why | ❌ W0 | ⬜ pending |
| 02-01+02 | 01,02 | 1 | PROT-02 + PROT-03 | Manual review | Verify section count ≥ 15; verify TIDieR/CERT header; verify -BR suffix on all outcome tools | ❌ W0 | ⬜ pending |

*Status: ⬜ pending · ✅ green · ❌ red · ⚠️ flaky*

---

## Wave 0 Requirements

- [ ] `protocols/P-08-SARCOPENIA.md` — PROT-02 (entire file, Plan 02-01)
- [ ] `protocols/P-04-OSTEOPOROSE.md` — PROT-03 (entire file, Plan 02-02)
- [ ] SHARED-FOUNDATION.md update — P-08 and P-04 rows in cross-reference index (Section 8.1 matrix)

*(No existing test infrastructure — all content is greenfield for Phase 2)*

---

## Manual-Only Verifications

| Behavior | Requirement | Why Manual | Test Instructions |
|----------|-------------|------------|-------------------|
| EWGSOP2-anchored frailty-stratified resistance dosing table | PROT-02 | Clinical content review — no automated parsing for clinical validity | Verify FACS algorithm, 3 Fried rows, EWGSOP2 cutoffs match PubMed 30312372 |
| Bone-loading constraint set by BMD category | PROT-03 | Clinical content review — constraint thresholds require domain expertise | Verify 4 risk categories, 3 constraint axes, FRAX integration, alignment with "Too Fit to Fracture" |
| TIDieR/CERT compliance | PROT-02 + PROT-03 | Reporting standard adherence — requires section-by-section audit | Check all TIDieR items present; CERT checklist items addressed |
| Cross-protocol modifier labeling | PROT-02 + PROT-03 | Semantic verification — modifier tables clearly labeled for downstream citation | Verify explicit "Tabela de Referência Cruzada" labels on modifier tables |

---

## Validation Sign-Off

- [ ] All tasks have manual verification criteria defined
- [ ] Sampling continuity: every task has a reviewable output
- [ ] Wave 0 covers all MISSING references
- [ ] No watch-mode flags
- [ ] Feedback latency acceptable for manual review
- [ ] `nyquist_compliant: true` set in frontmatter

**Approval:** pending
