---
phase: 06
slug: cluster-cardiorrespiratorio
status: draft
nyquist_compliant: false
wave_0_complete: false
created: 2026-03-13
---

# Phase 06 — Validation Strategy

> Per-phase validation contract for feedback sampling during execution.

---

## Test Infrastructure

| Property | Value |
|----------|-------|
| **Framework** | Não aplicável — repositório de documentação clínica sem suite de testes automatizados |
| **Config file** | none |
| **Quick run command** | Inspeção manual de estrutura + contagem de seções obrigatórias por protocolo |
| **Full suite command** | Verificação de 8 questões de validade clínica (Seção 15 de cada protocolo) + checklist de seção universal |
| **Estimated runtime** | ~2 minutes (grep-based inspection) |

---

## Sampling Rate

- **After every task commit:** Inspeção de grep dos marcadores críticos listados abaixo
- **After every plan wave:** Verificação de 8 questões de validade clínica (Seção 15) + todas as seções obrigatórias presentes (1–15)
- **Before `/gsd:verify-work`:** Full checklist de 3 critérios de sucesso + documentação do passe retroativo
- **Max feedback latency:** ~30 seconds

---

## Per-Task Verification Map

| Task ID | Plan | Wave | Requirement | Test Type | Automated Command | File Exists | Status |
|---------|------|------|-------------|-----------|-------------------|-------------|--------|
| 06-01-01 | 01 | 1 | PROT-11 | grep inspection | `grep -n "SpO2\|90%\|88%" protocols/P-15-DPOC.md` | ❌ W1 | ⬜ pending |
| 06-01-01 | 01 | 1 | PROT-11 | grep inspection | `grep -n "TC6M\|MCID\|25 m\|30 m" protocols/P-15-DPOC.md` | ❌ W1 | ⬜ pending |
| 06-01-01 | 01 | 1 | PROT-11 | grep inspection | `grep -n "ATS\|ERS\|37581410" protocols/P-15-DPOC.md` | ❌ W1 | ⬜ pending |
| 06-01-02 | 01 | 1 | PROT-12 | grep inspection | `grep -n "RPE\|Borg\|betabloqueador\|FC embotada" protocols/P-16-INSUFICIENCIA-CARDIACA.md` | ❌ W1 | ⬜ pending |
| 06-01-02 | 01 | 1 | PROT-12 | grep inspection | `grep -n "peso diário\|2 kg\|cardiologista" protocols/P-16-INSUFICIENCIA-CARDIACA.md` | ❌ W1 | ⬜ pending |
| 06-01-02 | 01 | 1 | PROT-12 | grep inspection | `grep -n "termorregula\|temperatura\|calor\|hidrata" protocols/P-16-INSUFICIENCIA-CARDIACA.md` | ❌ W1 | ⬜ pending |
| 06-02-01 | 02 | 2 | SC-3 | grep inspection | `grep -c "Precauções Cardiorrespiratórias" protocols/P-*.md` | ❌ W2 | ⬜ pending |

*Status: ⬜ pending · ✅ green · ❌ red · ⚠️ flaky*

---

## Wave 0 Requirements

Nenhuma lacuna de infraestrutura — repositório de documentação não tem suite de testes.

Gaps específicos de conteúdo a resolver durante execução:
- [ ] Verificar citação BR validada para MLHFQ (Minnesota Living with Heart Failure Questionnaire)
- [ ] Verificar citação BR validada para CAT (COPD Assessment Test)
- [ ] Confirmar status de ATS/ERS 2023 Guideline (adendo/corrigendum 2024–2026)

*Existing infrastructure covers all phase requirements.*

---

## Manual-Only Verifications

| Behavior | Requirement | Why Manual | Test Instructions |
|----------|-------------|------------|-------------------|
| Seção 15 — 8 questões de validade clínica | PROT-11, PROT-12 | Clinical content review cannot be automated | Ler Seção 15 de P-15 e P-16; confirmar que todas as 8 questões têm resposta inequívoca |
| Template universal aplicado consistentemente | SC-3 | Cross-protocol content consistency review | Comparar Seção 11 de todos os 10 protocolos com template; verificar limiares idênticos |

---

## Validation Sign-Off

- [ ] All tasks have `<automated>` verify or Wave 0 dependencies
- [ ] Sampling continuity: no 3 consecutive tasks without automated verify
- [ ] Wave 0 covers all MISSING references
- [ ] No watch-mode flags
- [ ] Feedback latency < 30s
- [ ] `nyquist_compliant: true` set in frontmatter

**Approval:** pending
