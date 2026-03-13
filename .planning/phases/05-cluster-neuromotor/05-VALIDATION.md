---
phase: 5
slug: cluster-neuromotor
status: draft
nyquist_compliant: false
wave_0_complete: false
created: 2026-03-13
---

# Phase 5 — Validation Strategy

> Per-phase validation contract for feedback sampling during execution.

---

## Test Infrastructure

| Property | Value |
|----------|-------|
| **Framework** | Manual document inspection (clinical documentation project — no automated test framework) |
| **Config file** | Not applicable |
| **Quick run command** | Manual review of 15 sections against phase requirement checklist |
| **Full suite command** | Review against PROT-08, PROT-09, PROT-10 + phase success criteria + SHARED-FOUNDATION updated |
| **Estimated runtime** | ~5 minutes per protocol review |

---

## Sampling Rate

- **After every task commit:** Manual inspection of key protocol sections (Sections 1, 2, 4, 8, 9, 13, 15)
- **After every plan wave:** Verify all cross-references between protocols + dual-task template correctly referenced by P-06 and P-18
- **Before `/gsd:verify-work`:** All 3 protocols complete + SHARED-FOUNDATION updated
- **Max feedback latency:** Manual review cycle

---

## Per-Task Verification Map

| Task ID | Plan | Wave | Requirement | Test Type | Verification Method | File Exists | Status |
|---------|------|------|-------------|-----------|---------------------|-------------|--------|
| 05-01-01 | 01 | 1 | PROT-08 | Structural inspection | P-03-AVC.md has 15 sections with neuroplasticity-grounded progression (Sections 5/6/7) | ❌ W0 | ⬜ pending |
| 05-01-02 | 01 | 1 | PROT-08 | Content inspection | P-03 includes aphasia/apraxia instruction adaptation subsection | ❌ W0 | ⬜ pending |
| 05-01-03 | 01 | 1 | PROT-08 | Content inspection | P-03 includes dual-task template (CLUSTER NEUROMOTOR template) in Phase 3 | ❌ W0 | ⬜ pending |
| 05-02-01 | 02 | 2 | PROT-09 | Content inspection | P-06-PARKINSON.md has 45–60 min post-dose levodopa scheduling rule | ❌ W0 | ⬜ pending |
| 05-02-02 | 02 | 2 | PROT-09 | Content inspection | P-06 includes on/off state prescription differentiation table | ❌ W0 | ⬜ pending |
| 05-02-03 | 02 | 2 | PROT-09 | Content inspection | P-06 includes formal caregiver training section with minimum load and defined content | ❌ W0 | ⬜ pending |
| 05-02-04 | 02 | 2 | PROT-10 | Content inspection | P-18-DEMENCIA.md has cognitive-adapted instruction system by MMSE/MoCA stratified | ❌ W0 | ⬜ pending |
| 05-02-05 | 02 | 2 | PROT-10 | Content inspection | P-18 Section 2 includes MMSE-BR or MoCA-BR as mandatory baseline instrument | ❌ W0 | ⬜ pending |
| 05-02-06 | 02 | 2 | PROT-10 | Content inspection | P-18 HEP policy: 2–3 exercises + mandatory pictographic sheet for MMSE < 24 | ❌ W0 | ⬜ pending |
| 05-02-07 | 02 | 2 | PROT-10 | Content inspection | P-18 Section 8 includes PAINAD-BR as primary pain instrument for MMSE < 18 | ❌ W0 | ⬜ pending |
| 05-SF-01 | 02 | 2 | PROT-08/09/10 | Cross-reference inspection | None of three protocols re-derives resistance dosage table (cites P-08 Section 6.3) | ❌ W0 | ⬜ pending |
| 05-SF-02 | 02 | 2 | PROT-08/09/10 | Cross-reference inspection | None of three protocols re-derives balance hierarchy (cites P-07 Section 7.2) | ❌ W0 | ⬜ pending |
| 05-SF-03 | 02 | 2 | PROT-08/09/10 | Index update | SHARED-FOUNDATION Section 8.1 populated with P-03, P-06, P-18 rows | ❌ W0 | ⬜ pending |

*Status: ⬜ pending · ✅ green · ❌ red · ⚠️ flaky*

---

## Wave 0 Requirements

- [ ] `protocols/P-03-AVC.md` — covers PROT-08
- [ ] `protocols/P-06-PARKINSON.md` — covers PROT-09
- [ ] `protocols/P-18-DEMENCIA.md` — covers PROT-10
- [ ] Update `protocols/SHARED-FOUNDATION.md` Section 8.1 with P-03, P-06, P-18 rows

---

## Manual-Only Verifications

| Behavior | Requirement | Why Manual | Test Instructions |
|----------|-------------|------------|-------------------|
| All protocol content | PROT-08/09/10 | Documentation project — no executable code | Review each section against clinical evidence standards and phase success criteria |
| Cross-reference integrity | PROT-08/09/10 | Semantic verification of citations | Confirm each protocol's cross-references to P-08 Section 6.3, P-07 Section 7.2, and SHARED-FOUNDATION resolve correctly |
| Dual-task template reuse | PROT-08 | Template created in P-03 must be usable by P-06 and P-18 | Verify P-06 and P-18 reference (not re-derive) the dual-task template from P-03 |

---

## Validation Sign-Off

- [ ] All tasks have verification criteria mapped
- [ ] Sampling continuity: no 3 consecutive tasks without verification
- [ ] Wave 0 covers all MISSING references
- [ ] No watch-mode flags
- [ ] Feedback latency acceptable for manual review
- [ ] `nyquist_compliant: true` set in frontmatter

**Approval:** pending
