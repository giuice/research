---
phase: 8
slug: protocolos-especializados
status: draft
nyquist_compliant: false
wave_0_complete: false
created: 2026-03-14
---

# Phase 8 — Validation Strategy

> Per-phase validation contract for feedback sampling during execution.

---

## Test Infrastructure

| Property | Value |
|----------|-------|
| **Framework** | Nenhum — projeto de documentação clínica (ver CLAUDE.md) |
| **Config file** | Não aplicável |
| **Quick run command** | `grep -c "glicemia\|hipoglicemia" protocols/P-17-NEUROPATIA-PERIFERICA-DIABETICA.md` |
| **Full suite command** | Ver Per-Task Verification Map abaixo |
| **Estimated runtime** | ~2 seconds |

---

## Sampling Rate

- **After every task commit:** Executar verificação do artefato imediatamente após criação de cada arquivo
- **After every plan wave:** Verificação completa de todos os requisitos de fase
- **Before `/gsd:verify-work`:** Todos os grep retornam contagem > 0 + inspeção visual de qualidade
- **Max feedback latency:** 2 seconds

---

## Per-Task Verification Map

| Task ID | Plan | Wave | Requirement | Test Type | Automated Command | File Exists | Status |
|---------|------|------|-------------|-----------|-------------------|-------------|--------|
| 08-01-01 | 01 | 1 | PROT-19 | Inspeção doc | `grep -c "glicemia\|glicosímetro\|hipoglicemia" protocols/P-17-NEUROPATIA-PERIFERICA-DIABETICA.md` | ❌ W0 | ⬜ pending |
| 08-01-02 | 01 | 1 | PROT-19 | Inspeção doc | `grep -c "P-07.*Seção 7.2\|SE-1\|SE-2\|SE-3\|SE-4" protocols/P-17-NEUROPATIA-PERIFERICA-DIABETICA.md` | ❌ W0 | ⬜ pending |
| 08-01-03 | 01 | 1 | PROT-19 | Inspeção doc | `grep -c "inspeção.*pés\|monofilamento\|cuidados.*pés" protocols/P-17-NEUROPATIA-PERIFERICA-DIABETICA.md` | ❌ W0 | ⬜ pending |
| 08-02-01 | 02 | 1 | PROT-20 | Inspeção doc | `grep -c "Passo 0\|hipertônico\|hipotônico\|Modified Oxford" protocols/P-14-DISFUNCAO-ASSOALHO-PELVICO.md` | ❌ W0 | ⬜ pending |
| 08-02-02 | 02 | 1 | PROT-20 | Inspeção doc | `grep -c "15243675\|Tamanini\|ICIQ-SF" protocols/P-14-DISFUNCAO-ASSOALHO-PELVICO.md` | ❌ W0 | ⬜ pending |
| 08-03-01 | 03 | 2 | OUT-04 | Inspeção doc | `grep -c "P-14.*Disfunção\|P-17.*Neuropatia" protocols/SHARED-FOUNDATION.md` | ❌ W0 | ⬜ pending |

*Status: ⬜ pending · ✅ green · ❌ red · ⚠️ flaky*

---

## Wave 0 Requirements

- [ ] `protocols/P-17-NEUROPATIA-PERIFERICA-DIABETICA.md` — cobre PROT-19
- [ ] `protocols/P-14-DISFUNCAO-ASSOALHO-PELVICO.md` — cobre PROT-20
- [ ] `protocols/SHARED-FOUNDATION.md` (linhas P-14 e P-17 na Seção 8.1) — cobre OUT-04

*Existing infrastructure covers automated verification via grep inspection.*

---

## Manual-Only Verifications

| Behavior | Requirement | Why Manual | Test Instructions |
|----------|-------------|------------|-------------------|
| Coerência clínica do Cross-Reference Index | OUT-04 | Requer julgamento clínico sobre completude e navegabilidade | Inspeção visual: todas as 20 comorbidades mapeadas, interações bidireccionais, modificadores de dosagem presentes |
| Hierarquia SE-1→SE-4 clinicamente progressiva | PROT-19 | Progressão clínica requer avaliação de expertise | Verificar que cada nível adiciona complexidade sensoriomotora adequada |
| Diferenciação terapêutica hiper/hipo correta | PROT-20 | Inversão terapêutica é risco iatrogênico | Verificar que PFMT é contraindicado em hipertônico e indicado em hipotônico |

---

## Validation Sign-Off

- [ ] All tasks have `<automated>` verify or Wave 0 dependencies
- [ ] Sampling continuity: no 3 consecutive tasks without automated verify
- [ ] Wave 0 covers all MISSING references
- [ ] No watch-mode flags
- [ ] Feedback latency < 2s
- [ ] `nyquist_compliant: true` set in frontmatter

**Approval:** pending
