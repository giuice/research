---
phase: 7
slug: musculoesqueletico-secundario-e-dor-cronica
status: draft
nyquist_compliant: false
wave_0_complete: false
created: 2026-03-14
---

# Phase 7 — Validation Strategy

> Per-phase validation contract for feedback sampling during execution.

---

## Test Infrastructure

| Property | Value |
|----------|-------|
| **Framework** | Não aplicável — repositório de documentação clínica sem suite de testes automatizados |
| **Config file** | none |
| **Quick run command** | `grep -n "NÃO COBRE\|CSI\|PNE\|11.1 Protocolo de Avaliação Pré-Sessão" protocols/P-{XX}-*.md` |
| **Full suite command** | Verificação das 8 questões de validade clínica (Seção 15) + checklist de diferenciação de escopo + presença de template universal Seção 11 |
| **Estimated runtime** | ~5 seconds (grep) / ~10 min (manual review) |

---

## Sampling Rate

- **After every task commit:** Inspeção grep dos marcadores críticos por protocolo (NÃO COBRE, CSI, PNE, Seção 11.1)
- **After every plan wave:** Verificação completa das 8 questões de validade clínica (Seção 15) + diferenciação de escopo para cada par de alta sobreposição
- **Before `/gsd:verify-work`:** Três critérios de sucesso verificados: (1) P-02/P-12 sem duplicação substantiva; (2) todos os 6 protocolos com PNE e CSI conforme nível; (3) índice cruzado SHARED-FOUNDATION com 6 linhas preenchidas
- **Max feedback latency:** 5 seconds (grep) / 10 minutes (manual)

---

## Per-Task Verification Map

| Task ID | Plan | Wave | Requirement | Test Type | Automated Command | File Exists | Status |
|---------|------|------|-------------|-----------|-------------------|-------------|--------|
| 07-01-01 | 01 | 1 | PROT-13 | Inspeção Seção 1 | `grep -n "NÃO COBRE\|estenose\|claudicação neurogênica" protocols/P-02-*.md` | ❌ W1 | ⬜ pending |
| 07-01-02 | 01 | 1 | PROT-13 | Inspeção Seção 2 | `grep -n "CSI\|sensitiza\|Central Sensitization" protocols/P-02-*.md` | ❌ W1 | ⬜ pending |
| 07-01-03 | 01 | 1 | PROT-13 | Inspeção Seção 11 | `grep -n "11.1 Protocolo de Avaliação Pré-Sessão" protocols/P-02-*.md` | ❌ W1 | ⬜ pending |
| 07-01-04 | 01 | 1 | PROT-14 | Inspeção Seção 1 | `grep -n "NÃO COBRE\|claudicação\|estenose" protocols/P-09-*.md` | ❌ W1 | ⬜ pending |
| 07-02-01 | 02 | 1 | PROT-15 | Inspeção Seções 5-6 | `grep -n "PNE\|Módulo\|neurociência da dor\|tempo-contingente" protocols/P-12-*.md` | ❌ W1 | ⬜ pending |
| 07-02-02 | 02 | 1 | PROT-15 | Inspeção Seção 2 | `grep -n "CSI\|≥ 40\|sensibiliza" protocols/P-12-*.md` | ❌ W1 | ⬜ pending |
| 07-02-03 | 02 | 1 | PROT-15 | Inspeção Seção 1 | `grep -n "IASP\|Chronic Primary Pain\|ICD-11\|MG30" protocols/P-12-*.md` | ❌ W1 | ⬜ pending |
| 07-02-04 | 02 | 2 | PROT-16 | Inspeção Seções 1+5+6+7 | `grep -n "P-04\|Seção 5.2\|MODIFICADOR TRANSVERSAL" protocols/P-19-*.md` | ❌ W2 | ⬜ pending |
| 07-02-05 | 02 | 2 | PROT-16 | Inspeção Seção 9 | `grep -n "cauda equina\|retenção urinária\|anestesia perianal" protocols/P-19-*.md` | ❌ W2 | ⬜ pending |
| 07-03-01 | 03 | 2 | PROT-17 | Inspeção Seção 1 | `grep -n "NÃO COBRE\|impingement\|capsulite\|manguito" protocols/P-13-*.md` | ❌ W2 | ⬜ pending |
| 07-03-02 | 03 | 2 | PROT-18 | Inspeção Seção 1 | `grep -n "NÃO COBRE\|conservador\|P-01\|cirúrgico" protocols/P-20-*.md` | ❌ W2 | ⬜ pending |
| 07-03-03 | 03 | 2 | SC-3 | Inspeção SHARED-FOUNDATION 8.1 | `grep -c "P-02\|P-09\|P-12\|P-13\|P-19\|P-20" protocols/SHARED-FOUNDATION.md` | Verificar W2 | ⬜ pending |

*Status: ⬜ pending · ✅ green · ❌ red · ⚠️ flaky*

---

## Wave 0 Requirements

Nenhuma lacuna de infraestrutura — repositório de documentação. Gaps de conteúdo a resolver antes da implementação:

- [ ] Confirmar PMID de validação BR do CSI (Central Sensitization Inventory)
- [ ] Confirmar validação peer-reviewed BR para KOOS-BR e HOOS-BR — ou posicionar WOMAC-BR como primário em P-20
- [ ] Verificar PSFS-BR — citar com nota de cautela se não confirmado
- [ ] Verificar status de NICE NG261 (2024) — diretriz final vs. consulta pública
- [ ] Verificar AGS Beers 2025/2026 antes de seções de polifarmácia

*Existing infrastructure covers all phase requirements.*

---

## Manual-Only Verifications

| Behavior | Requirement | Why Manual | Test Instructions |
|----------|-------------|------------|-------------------|
| P-02/P-12 sem duplicação substantiva de conteúdo | SC-1 | Requer revisão clínica comparativa | Comparar Seções 1, 5, 6 de ambos protocolos — nenhum parágrafo idêntico, populações-alvo distintas |
| PNE com dosagem adequada por nível de integração | SC-2 | Requer avaliação clínica da dosagem | P-12: 3 módulos ≥30min; P-02/P-09/P-13: sessão adjunta; P-19/P-20: componente educacional |
| Índice cruzado SHARED-FOUNDATION completo | SC-3 | Requer avaliação de completude das interações | 6 linhas novas com interações bidirecionais documentadas |

---

## Validation Sign-Off

- [ ] All tasks have `<automated>` verify or Wave 0 dependencies
- [ ] Sampling continuity: no 3 consecutive tasks without automated verify
- [ ] Wave 0 covers all MISSING references
- [ ] No watch-mode flags
- [ ] Feedback latency < 10 min
- [ ] `nyquist_compliant: true` set in frontmatter

**Approval:** pending
