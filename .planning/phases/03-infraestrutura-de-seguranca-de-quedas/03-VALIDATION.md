---
phase: 3
slug: infraestrutura-de-seguranca-de-quedas
status: draft
nyquist_compliant: false
wave_0_complete: false
created: 2026-03-13
---

# Phase 3 — Validation Strategy

> Per-phase validation contract for feedback sampling during execution.

---

## Test Infrastructure

| Property | Value |
|----------|-------|
| **Framework** | Manual clinical review (documentation/specification project — no automated test suite) |
| **Config file** | None |
| **Quick run command** | N/A — reviewer reads document against protocol checklist |
| **Full suite command** | N/A — manual review of all 15 sections + 2 modifier sections |
| **Estimated runtime** | ~10 minutes per manual review pass |

---

## Sampling Rate

- **After every task commit:** Manual review of changed sections against checklist
- **After every plan wave:** Full manual review of all deliverables
- **Before `/gsd:verify-work`:** All checklist items must pass
- **Max feedback latency:** N/A (manual review)

---

## Per-Task Verification Map

| Task ID | Plan | Wave | Requirement | Test Type | Method | File Exists | Status |
|---------|------|------|-------------|-----------|--------|-------------|--------|
| 03-01-01 | 01 | 1 | PROT-04 | Manual review | Confirm balance hierarchy table: 4 rows with numerical TUG, SPPB, BBS entry criteria; modifier label present | ❌ W0 | ⬜ pending |
| 03-01-02 | 01 | 1 | PROT-04 | Manual review | Confirm session-level fall risk protocol: all 4 elements (VAS fatigue, BP check, gait belt by TUG, supervised exit) with operational thresholds | ❌ W0 | ⬜ pending |
| 03-01-03 | 01 | 1 | PROT-04 | Manual review | Verify P-07 is self-contained, TIDieR/CERT compliant, ≥15 sections, all in BR-PT | ❌ W0 | ⬜ pending |
| 03-01-04 | 01 | 1 | PROT-04 | Manual review | Search for BBS-BR, FES-I-BR, TSK-11-BR — confirm -BR suffix and validation citations (Miyamoto 2004; Camargos 2010; Salvador 2020) | ❌ W0 | ⬜ pending |
| 03-01-05 | 01 | 1 | PROT-04 | Manual review | Confirm balance hierarchy modifier label with downstream protocol list and citation format | ❌ W0 | ⬜ pending |
| 03-01-06 | 01 | 1 | PROT-04 | Manual review | Verify P-07 answers all 8 clinical validity questions (who, when, where, what, how much, how fast, how to measure, why) | ❌ W0 | ⬜ pending |

*Status: ⬜ pending · ✅ green · ❌ red · ⚠️ flaky*

---

## Wave 0 Requirements

- [ ] `protocols/P-07-QUEDAS.md` — PROT-04 (entire file, Plan 03-01)
- [ ] SHARED-FOUNDATION.md update — P-07 row in cross-reference index (Section 8.1 matrix)

*(No existing P-07 file — all content is greenfield for Phase 3)*

---

## Manual-Only Verifications

| Behavior | Requirement | Why Manual | Test Instructions |
|----------|-------------|------------|-------------------|
| Balance hierarchy has objective entry criteria for each level | PROT-04 | Clinical content review — no code to test | Verify table has 4 rows (static/dynamic/dual-task/perturbation) with TUG, SPPB, BBS numerical thresholds |
| Session fall risk protocol has operational thresholds | PROT-04 | Clinical content review | Check VAS fatigue tiers, BP drop criterion (≥20 mmHg systolic), TUG-anchored gait belt table, exit criteria list |
| TIDieR/CERT compliance | PROT-04 | Specification compliance check | Cross-reference section headers against TIDieR/CERT checklist from Phase 1 template |
| All assessment tools use -BR validated versions | PROT-04 | Clinical accuracy review | Search for BBS, FES-I, TSK-11 — confirm -BR suffix and Brazilian validation citation |

---

## Validation Sign-Off

- [ ] All tasks have manual verification criteria defined
- [ ] Sampling continuity: every task has at least one verification method
- [ ] Wave 0 covers all file creation requirements
- [ ] Feedback method documented for each task
- [ ] `nyquist_compliant: true` set in frontmatter

**Approval:** pending
