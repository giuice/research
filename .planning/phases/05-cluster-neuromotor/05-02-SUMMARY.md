---
phase: 05-cluster-neuromotor
plan: "02"
subsystem: protocols
tags: [parkinson, demencia, neuromotor, levodopa-timing, instrucao-adaptada, cuidadores]
dependency_graph:
  requires: ["05-01"]
  provides: ["P-06-PARKINSON.md", "P-18-DEMENCIA.md", "SHARED-FOUNDATION P-06/P-18 rows"]
  affects: ["SHARED-FOUNDATION.md", "Phase 6 cross-references"]
tech_stack:
  added: []
  patterns:
    - "Levodopa timing rule (45–60 min pós-dose) como regra estrutural de agendamento"
    - "Tabela ON/OFF para diferenciação de prescrição de exercício por estado clínico"
    - "Sistema de Instrução Adaptada ao MMSE-BR (4 estratos: ≥24, 20–23, <24, <18)"
    - "Política de HEP Pictográfico obrigatório para MMSE < 24"
    - "Treinamento de cuidadores como componente formal (3 sessões) em P-06 e P-18"
    - "Aprendizagem procedimental/implícita (Kalbe 2007) como fundação pedagógica de P-18"
    - "PAINAD-BR como instrumento primário de dor para MMSE < 18 (P-18) e MoCA < 18 (P-06)"
key_files:
  created:
    - protocols/P-06-PARKINSON.md
    - protocols/P-18-DEMENCIA.md
  modified:
    - protocols/SHARED-FOUNDATION.md
decisions:
  - "[05-02]: Treinamento de cuidadores integrado como componente FORMAL nas fases (não apêndice) em P-06 e P-18 — 3 sessões obrigatórias com conteúdo estruturado por fase"
  - "[05-02]: Tabela ON/OFF de P-06 cobre todos os domínios clínicos relevantes: rigidez, bradicinesia, equilíbrio, freezing, discinesias, tolerância, exercícios indicados, progressão de carga e hierarquia de equilíbrio"
  - "[05-02]: MMSE < 24 é o corte mandatório para HEP pictográfico — abaixo deste ponto, HEP textual padrão é contraindicado por comprometimento de memória episódica"
  - "[05-02]: Cuidador identificado é CRITÉRIO DE INCLUSÃO em P-18 (não recomendação) — sem cuidador identificado, o protocolo não pode ser aplicado com segurança"
  - "[05-02]: Abbey Pain Scale citada com BAIXA CONFIANÇA explícita — validação cultural BR não confirmada; PAINAD-BR permanece como instrumento primário"
metrics:
  duration_minutes: 15
  completed_date: "2026-03-13"
  tasks_completed: 2
  files_created: 2
  files_modified: 1
requirements_satisfied: [PROT-09, PROT-10]
---

# Phase 5 Plan 02: Cluster Neuromotor — P-06 Parkinson e P-18 Demência Summary

**One-liner:** P-06 com regra de timing de levodopa, tabela ON/OFF e treinamento formal de cuidadores (APTA CPG 2022); P-18 com sistema de instrução cognitiva estratificada por MMSE-BR, HEP pictográfico obrigatório e PAINAD-BR para pacientes não-verbais (Kalbe 2007 + NICE NG97).

---

## Completed Tasks

| Task | Name | Commit | Files |
|------|------|--------|-------|
| 1 | Criar P-06-PARKINSON.md e P-18-DEMENCIA.md | 56fa323 | protocols/P-06-PARKINSON.md (850 linhas), protocols/P-18-DEMENCIA.md (902 linhas) |
| 2 | Atualizar SHARED-FOUNDATION.md com linhas P-06 e P-18 | 3d5ae2a | protocols/SHARED-FOUNDATION.md (Seção 8.1) |

---

## What Was Built

### P-06 — Doença de Parkinson (850 linhas, 15 seções)

**Camada farmacológica adicionada ao cluster neuromotor:**

- **Regra de timing de levodopa (45–60 min pós-dose):** Declarada na Seção 1 (admissão) e detalhada na Seção 5. É regra estrutural do protocolo — todas as sessões agendadas nesta janela.
- **Tabela ON/OFF (Seção 5.2):** 11 domínios clínicos com diferenciação completa de prescrição por estado clínico. O único protocolo da série com prescrição bidirecional (sessão no estado on vs. protocolo alternativo no estado off).
- **Protocolo de sessão em estado OFF (Seção 5.3):** Procedimento de 9 etapas para quando o paciente chega na sessão no estado off — carga reduzida 30%, exercícios sentados, sem progressão, documentação obrigatória.
- **Cueing externo (Seção 5.4):** Hierarquia de 4 tipos (visual, auditivo, tátil, mental/interno) com progressão de 6 semanas.
- **HIRT — High Intensity Resistance Training (Seção 6.2):** Per APTA CPG 2022 — recomendação grau A; tabela de dosagem por fragilidade via P-08 Seção 6.3.
- **LSVT BIG adaptado (Seção 6.3):** Princípios de amplitude exagerada com feedback visual; exercícios prioritários definidos.
- **Treinamento de cuidadores — 3 sessões formais:**
  - Sessão 1 (Fase 1, 30 min): Reconhecer estados ON/OFF, segurança básica, quando acionar PT vs. emergência
  - Sessão 2 (Fase 2, 45 min): Cueing para freezing, posicionamento correto de suporte de marcha, segurança ambiental
  - Sessão 3 (Fase 3, 30 min): Supervisão de HEP, reconhecimento de declínio, calendário de manutenção
- **Dupla tarefa (Seção 7.2):** TEMPLATE CLUSTER NEUROMOTOR — P-03 Seção 7.2, com adaptações P-06: ON obrigatório, reduzir complexidade se approaching-off, sem progressão em estado off.

### P-18 — Demência / Alzheimer (902 linhas, 15 seções)

**Camada cognitiva adicionada ao cluster neuromotor:**

- **Sistema de Instrução Adaptada (Seção 5.3):** 4 estratos por MMSE-BR com técnicas diferenciadas — o instrumento pedagógico central do protocolo:
  - MMSE ≥ 24: verbal + demonstração, HEP até 5 exercícios com imagem + texto
  - MMSE 20–23: demonstração primária, 1 comando verbal, HEP máx. 3 exercícios pictográfico
  - MMSE < 24: mão-sobre-mão, vanishing cues, sem instrução verbal multi-passo, HEP 2–3 exercícios pictográfico
  - MMSE < 18: mão-sobre-mão contínuo, tarefas em contexto funcional, HEP 2 exercícios, cuidador em TODAS as sessões
- **6 técnicas de instrução procedimental (Seção 5.3):** Mão-sobre-mão, vanishing cues, espelhamento, contexto funcional, ritmo musical, repetição idêntica.
- **Política de HEP Pictográfico (Seção 7.3):** Especificações técnicas detalhadas (imagem, nome 3 palavras, símbolo de frequência), limites por estrato MMSE, exemplos por estrato, instrução do cuidador como parte da política.
- **PAINAD-BR como instrumento primário (Seção 8.1):** Para MMSE < 18 ou comunicação verbal comprometida. Tabela completa dos 5 domínios + limiares de ação. Abbey Pain Scale com nota de baixa confiança explícita (validação BR não confirmada).
- **Dupla tarefa (Seção 7.2):** TEMPLATE CLUSTER NEUROMOTOR — P-03 Seção 7.2, com adaptações P-18: tarefa cognitiva FAMILIAR e PROCEDIMENTAL; aritmética e fluência verbal CONTRAINDICADOS para MMSE < 20.
- **Cuidador como co-terapeuta (Seções 5.9, 6.7, 7.7):** Critério de inclusão + 3 sessões formais + treinamento de instrução mão-sobre-mão + comunicação sobre expectativas realistas de desfecho.
- **Comunicação com família (Seção 7.9):** Template estruturado de comunicação de expectativas — desfecho funcional como primário, cognitivo como secundário, exercício crônico como padrão.
- **Padrão de documentação em prontuário (Seção 13.3):** 8 campos obrigatórios específicos para P-18.

### SHARED-FOUNDATION.md — Seção 8.1

- **Linha P-06:** 9 interações de comorbidade, regra de timing de levodopa, tabela ON/OFF, treinamento de cuidadores, HIRT, TEMPLATE, escopo, instrumentos
- **Linha P-18:** 9 interações de comorbidade, sistema de instrução cognitiva, HEP pictográfico, PAINAD-BR, cuidador como co-terapeuta, TEMPLATE, escopo, instrumentos
- **Cluster neuromotor completo:** P-03, P-06 e P-18 têm linhas populadas na Seção 8.1

---

## Deviations from Plan

None — plan executed exactly as written.

---

## Verification Results

**P-06 PARKINSON:**
1. protocols/P-06-PARKINSON.md — 850 linhas, 15 seções — PASS (>= 800 required)
2. Seção 1 contém levodopa timing rule (45–60 min) e NÃO COBRE — PASS
3. Seção 2 contém MDS-UPDRS III, Hoehn e Yahr, Registro de Horários — PASS
4. Seção 5 contém tabela ON/OFF com 11 domínios de diferenciação — PASS
5. Treinamento de cuidadores formal: 3 sessões (Seções 5.9, 6.7, 7.7) — PASS
6. Fase 3 referencia P-03 Seção 7.2 TEMPLATE CLUSTER NEUROMOTOR — PASS
7. Seção 13 contém P-07 5.2, P-07 7.2, P-08 6.3, P-04 5.2, P-03 7.2 — PASS
8. APTA CPG 2022 (PMC9046970) citado como diretriz primária — PASS

**P-18 DEMÊNCIA:**
9. protocols/P-18-DEMENCIA.md — 902 linhas, 15 seções — PASS (>= 900 required)
10. Seção 1 contém MMSE ≥ 10 / CDR 0.5–2 e cuidador identificado como critério — PASS
11. Seção 2 contém MMSE-BR E MoCA-BR obrigatórios, PAINAD-BR na admissão — PASS
12. Tabela de estratificação de instrução: ≥ 24, 20–23, < 24, < 18 — PASS
13. Política HEP pictográfico com limite 2–3 exercícios para MMSE < 24 — PASS
14. Seção 8 contém PAINAD-BR como primário para MMSE < 18, Abbey Pain Scale LOW confidence — PASS
15. Fase 3 referencia P-03 Seção 7.2 com adaptação (sem aritmética MMSE < 20) — PASS
16. Seção 13 contém P-07, P-08, P-04, P-03 com seções específicas — PASS
17. Seção 15 contém 8 questões + Questão Aberta sobre Abbey Pain Scale — PASS

**AMBOS:**
18. Tabelas de dosagem bidimensionais (fragilidade × parâmetro) em todas as fases — PASS
19. Documentos integralmente em português brasileiro — PASS
20. 8 questões de validade clínica respondidas na Seção 15 — PASS

**SHARED-FOUNDATION:**
21. Linha P-06 com ≥ 9 interações de comorbidade — PASS
22. Linha P-18 com ≥ 9 interações de comorbidade — PASS
23. P-03, P-06 e P-18 têm linhas populadas (cluster neuromotor completo) — PASS

---

## Self-Check: PASSED

| Item | Status |
|------|--------|
| protocols/P-06-PARKINSON.md exists | FOUND |
| protocols/P-18-DEMENCIA.md exists | FOUND |
| .planning/phases/05-cluster-neuromotor/05-02-SUMMARY.md exists | FOUND |
| Commit 56fa323 (Task 1 — P-06 + P-18) | FOUND |
| Commit 3d5ae2a (Task 2 — SHARED-FOUNDATION) | FOUND |
