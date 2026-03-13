---
phase: 06-cluster-cardiorrespiratorio
plan: "01"
subsystem: protocols
tags: [DPOC, insuficiencia-cardiaca, reabilitacao-pulmonar, reabilitacao-cardiaca, SpO2, RPE, template-universal]
dependency_graph:
  requires:
    - protocols/SHARED-FOUNDATION.md
    - protocols/P-08-SARCOPENIA.md (Section 6.3 — resistance dosing cross-reference)
    - protocols/P-07-QUEDAS.md (Section 7.2 — balance hierarchy cross-reference)
    - protocols/P-04-OSTEOPOROSE.md (Section 5.2 — bone load cross-reference)
  provides:
    - protocols/P-15-DPOC.md (complete DPOC rehabilitation protocol)
    - protocols/P-16-INSUFICIENCIA-CARDIACA.md (complete IC rehabilitation protocol)
    - SHARED-FOUNDATION.md Section 7.4 (universal Cardiorespiratory Precautions template)
    - SHARED-FOUNDATION.md Section 8.1 P-15 and P-16 rows
  affects:
    - All 10 prior protocols (Phases 1-5) — retroactive Section 11 update in Plan 06-02
tech_stack:
  added: []
  patterns:
    - Universal Cardiorespiratory Precautions template (11.1-11.5 structure)
    - SpO2 decision ladder for DPOC (90%/88% thresholds)
    - RPE Borg 6-20 exclusive intensity for IC with beta-blockers
    - Daily weight monitoring protocol with cardiology pathway
    - Thermoregulation guidance (22/26/30C limits)
    - IC-FEr vs IC-FEp differentiation with AHA 2023 Scientific Statement
key_files:
  created:
    - protocols/P-15-DPOC.md
    - protocols/P-16-INSUFICIENCIA-CARDIACA.md
  modified:
    - protocols/SHARED-FOUNDATION.md
decisions:
  - "[06-01]: SpO2 90% como limiar conservador de NÃO-INÍCIO e 88% como limiar de parada imediata em DPOC — variação de prática documentada (85–92%); adotado valor conservador para contexto geriátrico"
  - "[06-01]: Borg Dispneia 0–10 para DPOC e Borg RPE 6–20 para IC — distinção explícita e obrigatória; anti-pattern de confundir as escalas documentado em Research"
  - "[06-01]: IC-FEp e IC-FEr com mesma estrutura de exercício — AHA Scientific Statement 2023 (CIR.0000000000001122) como base para IC-FEp; progressão ligeiramente mais rápida quando tolerada"
  - "[06-01]: Template universal Seção 11 estabelecido em P-15 com 5 subseções (11.1 pré-sessão universal, 11.2 parada imediata universal, 11.3 monitoramento específico, 11.4 adaptações por comorbidade, 11.5 especificidades do diagnóstico primário)"
  - "[06-01]: MLHFQ-BR — validação peer-reviewed BR não confirmada; protocolo adota MLHFQ com nota explícita de cautela de validação cultural (padrão análogo ao estabelecido para outros instrumentos)"
  - "[06-01]: CAT-BR — mesmo status que MLHFQ-BR — nota de cautela de validação cultural adicionada ao protocolo P-15"
metrics:
  duration_minutes: 15
  completed_date: "2026-03-13"
  tasks_completed: 2
  files_created: 2
  files_modified: 1
---

# Phase 6 Plan 01: Cluster Cardiorrespiratório — DPOC e Insuficiência Cardíaca — Summary

**One-liner:** P-15 DPOC com SpO2 mandatório e TC6M como desfecho primário + P-16 IC com RPE Borg 6-20 exclusivo, protocolo de peso diário e termorregulação; template universal de Precauções Cardiorrespiratórias (Seção 11) estabelecido para passe retroativo nos 10 protocolos das Fases 1-5.

---

## What Was Built

### Task 1: P-15-DPOC.md e P-16-INSUFICIENCIA-CARDIACA.md

**P-15 DPOC** (813 linhas, 15 seções):
- Critérios diagnósticos por espirometria (FEV1/FVC < 0,70 pós-BD), GOLD II+, mMRC ≥ 2 ou CAT ≥ 10, estabilidade ≥ 28 dias
- SpO2 como parâmetro central: ≤ 90% = não iniciar; < 88% = parada imediata; monitoramento a cada 5 min durante exercício aeróbico; protocolo de suplementação de O2 com escada de decisão (Seção 11.5)
- TC6M como desfecho primário: MCID 25–30 m, equação Britto 2013 BR (com nota de limitação geriátrica), protocolo ATS 2002
- Borg Dispneia 0–10 como instrumento de intensidade (alvo 4–6)
- GOLD 2025 + ATS CPG 2023 (PMID 37581410) como diretrizes primárias
- Tabelas de dosagem frailty-stratified (Robusto/Pré-frágil/Frágil) × 3 fases com critérios de progressão funcionais
- Template Universal Seção 11 (11.1–11.5) estabelecido para reuso em todos os 20 protocolos

**P-16 IC** (858 linhas, 15 seções):
- Diferenciação IC-FEr/IC-FEm/IC-FEp com FEVE e referência AHA Scientific Statement 2023 (CIR.0000000000001122)
- Declaração crítica redundante: "FC CONTRAINDICADO como parâmetro em IC com betabloqueador" — no cabeçalho, nas tabelas de dosagem e na Seção 10 (mecanismo de cronotropia negativa explicado com evidência PMC3990937)
- RPE Borg 6–20 como único parâmetro de intensidade (alvo 11–13 Robusto; 10–11 Frágil/NYHA III)
- Protocolo de peso diário (manhã, mesma balança) com limiares: ≥ 1,5 kg/24h e ≥ 2,0 kg/3 dias = SUSPENDER + contatar médico (ESC Guidelines 2021)
- Termorregulação completa: ≤ 22°C ideal, máx 26°C, > 30°C sem AC = suspender; 200 mL hidratação pré-sessão (AHA Circulation 2006)
- Proibição de Valsalva explícita em todos os exercícios resistidos (3 ocorrências nas tabelas de dosagem)
- MLHFQ como desfecho primário (MCID ≥ 5 pontos); TC6M como desfecho secundário

### Task 2: SHARED-FOUNDATION.md

- **Seção 8.1 — P-15 row:** 10 interações de comorbidade com modificadores específicos (SpO2 mandatório, Borg Dispneia 0–10, template universal, TC6M, GOLD/ATS), precauções específicas (dessaturação silenciosa, exacerbação, cadeia de modificadores)
- **Seção 8.1 — P-16 row:** 10 interações de comorbidade com modificadores específicos (RPE exclusivo, FC contraindicada, peso diário, termorregulação, IC-FEr/FEp), precauções específicas (Valsalva proibido, AINEs contraindicados, descompensação)
- **Seção 7.4 expandida:** Template Universal de Precauções Cardiorrespiratórias com subseções 11.1 (pré-sessão universal), 11.2 (parada imediata universal), estrutura 11.3–11.5 para especificidades por diagnóstico; regras de aplicação do template; distinção obrigatória Borg Dispneia vs RPE
- **Status atualizado:** Linhas preenchidas na matriz 20×20 agora incluem P-15 e P-16; questão aberta nº 5 (ATS 2023) marcada como resolvida

---

## Commits

| Task | Commit | Descrição |
|------|--------|-----------|
| Task 1 | 615ec8e | feat(06-01): create P-15 DPOC and P-16 Insuficiencia Cardiaca protocols |
| Task 2 | b4653b4 | feat(06-01): update SHARED-FOUNDATION with P-15 and P-16 rows and universal Section 11 template |

---

## Verification Results

### P-15 DPOC
- Linhas: 813 (alvo 750–900) — PASS
- Seções: 18 headers (15 principais + subseções) — PASS
- SpO2 90%/88% thresholds: confirmados — PASS
- TC6M como desfecho primário com MCID 25–30 m: confirmado — PASS
- ATS CPG 2023 (PMID 37581410): confirmado — PASS
- Borg Dispneia 0–10 para intensidade: confirmado — PASS
- Template Universal Seção 11 (11.1–11.5): confirmado — PASS
- Frailty-stratified dosage tables (todas as fases): confirmado — PASS

### P-16 IC
- Linhas: 858 (alvo 750–900) — PASS
- Seções: 18 headers (15 principais + subseções) — PASS
- RPE Borg 6–20 exclusivo com declaração de betabloqueador: confirmado — PASS
- FC como parâmetro contraindicado: declarado no cabeçalho, Seção 10, tabelas — PASS
- Protocolo de peso diário com limiares (1,5 kg/24h, 2 kg/3 dias): confirmado — PASS
- Termorregulação (22/26/30°C): confirmado — PASS
- IC-FEr/IC-FEp differentiation com AHA 2023: confirmado — PASS
- Proibição de Valsalva: confirmada em todas as tabelas de dosagem — PASS

### SHARED-FOUNDATION
- P-15 row em Section 8.1 com ≥ 9 interações: 10 interações — PASS
- P-16 row em Section 8.1 com ≥ 9 interações: 10 interações — PASS
- Template universal Seção 7.4 documentado para uso retroativo: PASS

---

## Deviations from Plan

None — plan executed exactly as written.

**Anti-patterns evitados:**
1. FC NÃO usada como parâmetro de intensidade em P-16 (declarado explicitamente 3x)
2. Borg RPE 6–20 vs Borg Dispneia 0–10 distinguidos explicitamente em ambos os protocolos
3. SpO2 monitoramento mandatório em P-15 (não apenas sintomático)
4. Peso diário com protocolo completo em P-16 (não apenas menção)
5. NYHA IV diferenciado (contraindicação relativa, não absoluta) — protocolo de NYHA IV compensada em Seção 1.4 de P-16
6. IC-FEr/IC-FEp explicitamente diferenciados com referência AHA 2023

---

## Open Questions Resolved

- **ATS/ERS 2023 Pulmonary Rehabilitation Statement:** ATS CPG 2023 (PMID 37581410) adotado como diretriz primária. Nota de verificação de adendos 2024–2026 incluída no protocolo.

## Open Questions Remaining

- **MLHFQ-BR:** Validação peer-reviewed em amostra brasileira não confirmada — nota de cautela adicionada em P-16 Seção 2.2. A confirmar antes de publicação definitiva.
- **CAT-BR:** Mesmo status — nota de cautela adicionada em P-15 Seção 2.2.
- **EWGSOP3:** Continua pendente — usando EWGSOP2 (2018).

---

## Self-Check: PASSED

- protocols/P-15-DPOC.md: EXISTS (813 lines)
- protocols/P-16-INSUFICIENCIA-CARDIACA.md: EXISTS (858 lines)
- protocols/SHARED-FOUNDATION.md: MODIFIED (P-15/P-16 rows + Section 7.4 template)
- Commit 615ec8e: FOUND
- Commit b4653b4: FOUND
