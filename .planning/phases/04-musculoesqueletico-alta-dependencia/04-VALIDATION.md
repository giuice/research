---
phase: 4
slug: musculoesqueletico-alta-dependencia
status: draft
nyquist_compliant: false
wave_0_complete: false
created: 2026-03-13
---

# Phase 4 — Validation Strategy

> Per-phase validation contract for feedback sampling during execution.

---

## Test Infrastructure

| Property | Value |
|----------|-------|
| **Framework** | Inspeção manual de documento (projeto de documentação clínica) |
| **Config file** | Não aplicável |
| **Quick run command** | Revisão manual das 15 seções contra checklist |
| **Full suite command** | Revisão contra requisitos PROT-05, PROT-06, PROT-07 + success criteria da fase |
| **Estimated runtime** | ~10 minutos por protocolo |

---

## Sampling Rate

- **After every task commit:** Revisão manual das seções-chave do protocolo (Seção 1, 2, 4, 9, 13, 15)
- **After every plan wave:** Verificação de todas as referências cruzadas entre protocolos da fase
- **Before `/gsd:verify-work`:** Todos os 3 protocolos completos + SHARED-FOUNDATION atualizado
- **Max feedback latency:** N/A (inspeção manual)

---

## Per-Task Verification Map

| Task ID | Plan | Wave | Requirement | Test Type | Automated Command | File Exists | Status |
|---------|------|------|-------------|-----------|-------------------|-------------|--------|
| 04-01-01 | 01 | 1 | PROT-05 | Inspeção estrutural | Revisão 15 seções P-05 | ❌ W0 | ⬜ pending |
| 04-01-02 | 01 | 1 | PROT-05 | Inspeção de conteúdo | CFS mandatório na avaliação inicial | ❌ W0 | ⬜ pending |
| 04-01-03 | 01 | 1 | PROT-05 | Inspeção de conteúdo | Referência P-07 Seção 5.2 e 7.2 em Seção 13 | ❌ W0 | ⬜ pending |
| 04-01-04 | 01 | 1 | PROT-05 | Inspeção de conteúdo | TEV consciência sem prescrição de regime | ❌ W0 | ⬜ pending |
| 04-02-01 | 02 | 2 | PROT-06 | Inspeção estrutural | Revisão 15 seções P-10 + escopo diferenciado | ❌ W0 | ⬜ pending |
| 04-02-02 | 02 | 2 | PROT-06 | Inspeção de conteúdo | 5 Ps síndrome compartimental em Seção 9 | ❌ W0 | ⬜ pending |
| 04-02-03 | 02 | 2 | PROT-07 | Inspeção estrutural | Revisão 15 seções P-11 + precauções por abordagem | ❌ W0 | ⬜ pending |
| 04-02-04 | 02 | 2 | PROT-07 | Inspeção de referências | Seção 13 P-10/P-11 cita P-08, P-04, P-07 sem re-derivar | ❌ W0 | ⬜ pending |
| 04-02-05 | 02 | 2 | PROT-07 | Atualização de índice | SHARED-FOUNDATION Seção 8.1 com P-05, P-10, P-11 | ❌ W0 | ⬜ pending |

*Status: ⬜ pending · ✅ green · ❌ red · ⚠️ flaky*

---

## Wave 0 Requirements

- [ ] `protocols/P-05-FRATURA-FEMUR.md` — cobre PROT-05
- [ ] `protocols/P-10-ATJ.md` — cobre PROT-06
- [ ] `protocols/P-11-ATQ.md` — cobre PROT-07
- [ ] Atualização de `protocols/SHARED-FOUNDATION.md` Seção 8.1 com linhas P-05, P-10, P-11

*Existing infrastructure covers structural template (15 seções de P-01).*

---

## Manual-Only Verifications

| Behavior | Requirement | Why Manual | Test Instructions |
|----------|-------------|------------|-------------------|
| CFS na admissão P-05 | PROT-05 | Conteúdo clínico textual | Verificar Seção 2 contém CFS como mandatório |
| TEV consciência sem prescrição | PROT-05 | Semântica de escopo | Verificar que nenhuma tabela de agente+dose+duração existe |
| Diferenciação P-10/P-11 | PROT-06, PROT-07 | Análise comparativa | Comparar Seção 1 de ambos — escopos mutuamente exclusivos |
| Precauções por abordagem ATQ | PROT-07 | Conteúdo clínico | Verificar subseção posterior vs. anterior em P-11 |
| Referências cruzadas Seção 13 | PROT-05/06/07 | Inspeção de links | Confirmar citações a P-04 5.2, P-08 6.3, P-07 5.2/7.2 |

---

## Validation Sign-Off

- [ ] All tasks have verification criteria mapped
- [ ] Sampling continuity: every protocol reviewed after creation
- [ ] Wave 0 covers all MISSING references
- [ ] No automated test infrastructure needed (documentation project)
- [ ] Feedback latency < 10min per protocol review
- [ ] `nyquist_compliant: true` set in frontmatter

**Approval:** pending
