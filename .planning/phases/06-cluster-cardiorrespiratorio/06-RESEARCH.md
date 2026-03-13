# Phase 6: Cluster Cardiorrespiratório — Research

**Researched:** 2026-03-13
**Domain:** Reabilitação cardiorrespiratória geriátrica — DPOC (P-15) e Insuficiência Cardíaca (P-16), com retroactive update pass para seção universal de Precauções Cardiorrespiratórias
**Confidence:** HIGH (estrutura de protocolo, stack de avaliação, diretrizes ATS/ERS DPOC e AHA/ACC/HFSA IC) / MEDIUM (limiar SpO2 para suspensão: variação de prática entre 88–90%; termorregulação IC: mecanismo estabelecido, dados quantitativos de precaução clínica são inferidos de fisiopatologia) / LOW (equação de referência TC6M-BR em populações geriátricas com DPOC: Britto 2013 é referência adulta, cutoffs geriátricos específicos dependem de estimativa)

---

<phase_requirements>
## Phase Requirements

| ID | Descrição | Research Support |
|----|-----------|-----------------|
| PROT-11 | P-15 DPOC (reabilitação respiratória) — protocolo completo | Diretrizes ATS 2023 (PMID 37581410), GOLD 2024/2025, Diretriz Brasileira de Reabilitação Cardiovascular 2020; TC6M como instrumento primário com MCID estabelecido (25–30 m); SpO2 com limiar de início/parada operacional |
| PROT-12 | P-16 Insuficiência Cardíaca / Cardiopatias — protocolo completo | AHA/ACC/HFSA 2022 Guideline (CIR.0000000000001063); Diretriz Brasileira Reab. Cardiovascular 2020 (PMC8387006); RPE exclusivo por confundimento de FC por betabloqueadores documentado (PMC3990937); protocolo peso diário via ESC; termorregulação — AHA Circulation 2006 + PMC4042428 |
</phase_requirements>

---

## Summary

Esta fase produz dois protocolos do cluster cardiorrespiratório (P-15 DPOC e P-16 Insuficiência Cardíaca) e executa um passe retroativo adicionando a seção universal de Precauções Cardiorrespiratórias aos 10 protocolos já completados nas Fases 1–5. O sequenciamento é P-15 → P-16, porque P-15 (DPOC) estabelece o template da seção universal de Precauções Cardiorrespiratórias — incluindo protocolo de sinais vitais pré-sessão, monitoramento de SpO2, e critérios de suspensão — que P-16 herda e adapta (com modificadores específicos de IC), e que depois é retroativamente inserido nos 10 protocolos anteriores.

P-15 DPOC é um protocolo centrado na capacidade funcional aeróbica com restrição ventilatória como mecanismo primário de limitação. O instrumento de desfecho primário é o Teste de Caminhada de 6 Minutos (TC6M), referenciado pelo ATS/ERS e com valores normativos brasileiros disponíveis (Britto et al. 2013). O monitoramento de SpO2 durante o exercício é mandatório; a literatura apresenta variação de prática no limiar de parada (88% vs 90%), e este protocolo adotará 90% como limiar conservador alinhado ao contexto geriátrico. A escala de Borg modificada (dispneia) é o instrumento de intensidade de exercício, complementada pela mMRC para triagem de sintomas.

P-16 Insuficiência Cardíaca introduz dois modificadores de alta especificidade geriátrica ausentes em qualquer protocolo anterior: (1) o confundimento da FC por betabloqueadores, que torna a FC inutilizável como parâmetro de intensidade — RPE/Borg é o único monitor confiável; e (2) o comprometimento da termorregulação por IC + envelhecimento + betabloqueadores, que exige orientação explícita sobre temperatura ambiente e hidratação. O protocolo de monitoramento de peso diário (limiar ≥ 2 kg em 3 dias → alerta cardiologia) é a interface clínica entre reabilitação e cardiology care coordination.

**Recomendação primária:** P-15 primeiro (estabelece template cardiorrespiratório + SpO2 + critérios de parada), P-16 segundo (adapta template com modificadores IC-específicos), depois passe retroativo nos 10 protocolos com a seção universal padronizada.

---

## Standard Stack

### Instrumentos de Avaliação Primários

| Instrumento | Versão/Referência | Propósito | Por que padrão |
|-------------|------------------|-----------|----------------|
| TC6M (Teste de Caminhada de 6 Minutos) | ATS Statement 2002 + equação BR Britto et al. 2013 (J Pneumol) | Desfecho primário de capacidade funcional em DPOC; desfecho secundário em IC | Instrumento-padrão ATS/ERS para DPOC; MCID estabelecido (25–30 m); execução de baixo custo sem equipamento |
| Escala de Borg Modificada (dispneia 0–10) | Modified Borg Dyspnea Scale — Borg GA 1982 | Monitoramento de intensidade de esforço e dispneia durante sessão | Instrumento universal de PR; usado com TC6M; Borg dispneia e Borg RPE são escalas diferentes — usar dispneia (0–10) para DPOC, RPE (6–20) para IC |
| mMRC — Modified Medical Research Council Dyspnea Scale | Fletcher CM et al. 1952; usada em GOLD | Classificação de dispneia funcional basal; triagem de elegibilidade | Padrão GOLD para estadiamento sintomático; mMRC ≥ 2 = elegível para reabilitação pulmonar |
| CAT — COPD Assessment Test | Jones PW et al. Eur Respir J 2009 | Avaliação de impacto global de DPOC; triagem e reavaliação | Padrão GOLD para categorização AB; score ≥ 10 = alto impacto sintomático |
| Oxímetro de pulso (SpO2) | — | Monitoramento de dessaturação antes e durante exercício | Mandatório em DPOC; SpO2 < 90% em exercício = suspensão ou suplementação |
| Escala de Borg RPE (6–20) | Borg GA 1970 | Monitoramento de intensidade em IC quando FC confundida por betabloqueador | Único parâmetro confiável de intensidade em IC com betabloqueador |
| NYHA — New York Heart Association Functional Classification | AHA/ACC | Estadiamento funcional de IC; critério de inclusão/exclusão | Padrão universal para IC; NYHA I-III = elegível; NYHA IV = contraindicação relativa |
| MLHFQ — Minnesota Living with Heart Failure Questionnaire | Rector TS et al. 1987 | Qualidade de vida específica para IC | Instrumento de desfecho específico IC; MCID ≥ 5 pontos estabelecido |

### Instrumentos de Avaliação Secundários e Modificadores

| Instrumento | Propósito | Quando usar |
|-------------|-----------|-------------|
| Dinamometria Manual (Jamar) | Força de preensão — sarcopenia coexistente (alta prevalência em DPOC e IC) | Mandatório na bateria universal — ver SHARED-FOUNDATION Seção 1.3 |
| TUG | Mobilidade funcional — risco de queda | Mandatório na bateria universal |
| SPPB-BR | Desempenho físico global | Mandatório na bateria universal |
| Fenótipo de Fried | Classificação de fragilidade — tabela de dosagem | Mandatório — 3 categorias: Robusto / Pré-frágil / Frágil |
| Balança domiciliar calibrada | Monitoramento diário de peso em IC | Específico P-16: instrução de uso + limiar de alerta ≥ 2 kg em 3 dias |
| Esfigmomanômetro (PA) | PA basal pré-sessão | Universal — incluso no template de Precauções Cardiorrespiratórias |

### Diretrizes de Referência Primárias

| Diretriz | Ano | Escopo | Status |
|----------|-----|--------|--------|
| ATS Clinical Practice Guideline — Pulmonary Rehabilitation | 2023 (PMID 37581410) | Recomendação forte para DPOC estável e pós-exacerbação | Guideline mais atual; substitui posição conjunta ATS/ERS 2013 |
| GOLD 2025 Report | 2024/2025 (goldcopd.org) | Diagnóstico, estadiamento, manejo DPOC | Atualizado novembro 2024; usar para estadiamento ABCD e critérios de exercício |
| AHA/ACC/HFSA 2022 Heart Failure Guideline | 2022 (Circulation — CIR.0000000000001063) | Manejo completo de IC; exercício Classe I | Diretriz principal IC; exercício como recomendação Classe 1 independente de fração de ejeção |
| Diretriz Brasileira de Reabilitação Cardiovascular 2020 | 2020 (PMC8387006) | Reabilitação cardiovascular Brasil; IC, DAC | Diretriz brasileira vigente; abrange IC com FE reduzida e preservada |
| AHA Scientific Statement: Supervised Exercise for HFpEF | 2023 (Circulation — CIR.0000000000001122) | IC com FE preservada especificamente | Dado que IC geriátrica tem alta prevalência de HFpEF, este statement é necessário |

---

## Architecture Patterns

### Estrutura de Documentos da Fase

```
protocols/
├── P-15-DPOC.md               # Protocolo completo P-15 (~750–900 linhas, 15 seções)
├── P-16-INSUFICIENCIA-CARDIACA.md  # Protocolo completo P-16 (~750–900 linhas, 15 seções)
└── [atualização retroativa dos 10 protocolos existentes — Seção 11]

.planning/phases/06-cluster-cardiorrespiratorio/
├── 06-RESEARCH.md             # Este arquivo
├── 06-01-PLAN.md              # Plano: P-15 + P-16 + template universal
└── 06-02-PLAN.md              # Plano: passe retroativo + verificação
```

### Padrão: Sequência de Construção de Template

```
Plano 06-01:
1. Pesquisar e redigir P-15 DPOC (protocolo completo, 15 seções)
2. Extrair da Seção 11 de P-15 o TEMPLATE UNIVERSAL de Precauções Cardiorrespiratórias
   (Avaliação pré-sessão + sinais vitais + SpO2 + critérios de parada)
3. Pesquisar e redigir P-16 IC (protocolo completo, 15 seções)
   — P-16 Seção 11 = template universal + modificadores IC-específicos

Plano 06-02:
4. Para cada um dos 10 protocolos Fases 1–5:
   — Ler Seção 11 existente (Precauções Cardiorrespiratórias)
   — Verificar se já possui protocolo pré-sessão, SpO2, critérios de parada
   — Adicionar seção universal padronizada onde ausente ou incompleto
5. Documentar passe retroativo no SHARED-FOUNDATION Seção 7.4
```

### Estrutura de Seção Universal — Precauções Cardiorrespiratórias

A Seção 11 de todos os protocolos seguirá este template após o passe retroativo:

```
## 11. Precauções Cardiorrespiratórias

### 11.1 Protocolo de Sinais Vitais Pré-Sessão (UNIVERSAL)
- PA em repouso sentado (5 min)
- FC de repouso
- SpO2 basal
- Critérios de não-início: [tabela com limiares]

### 11.2 Monitoramento Durante a Sessão
- SpO2 contínua ou intermitente (a cada 5 min em DPOC)
- RPE ou Borg dispneia a cada 10 min
- Critérios de parada imediata: [tabela]

### 11.3 Adaptações por Comorbidade Cardiorrespiratória
- ICC coexistente: [adaptações específicas]
- DPOC coexistente: [adaptações específicas]

### 11.4 Especificidades [nome do protocolo]
- [Modificadores únicos ao diagnóstico primário]
```

### Anti-Padrões a Evitar

- **Usar FC como parâmetro de intensidade em P-16:** Betabloqueadores embotam a FC; prescrever intensidade por FC-alvo é clinicamente perigoso em IC. Usar RPE Borg 6–20 exclusivamente.
- **Omitir SpO2 em DPOC:** Dessaturação silenciosa é comum em DPOC moderada-grave; SpO2 apenas sintomática é insuficiente.
- **Confundir Borg RPE (6–20) com Borg Dispneia (0–10):** São escalas diferentes. DPOC usa dispneia 0–10; IC usa RPE 6–20. Ambas podem coexistir em pacientes com comorbidade.
- **Ignorar peso diário em IC:** Ganho de ≥ 2 kg em 3 dias indica retenção hídrica e contraindicação à sessão de exercício até avaliação médica.
- **Classificar NYHA IV como contraindicação absoluta sem contexto:** NYHA IV com compensação recente pode iniciar mobilização leve supervisionada; a contraindicação é à reabilitação formal não monitorada.
- **Seção de Precauções Cardiorrespiratórias genérica demais:** Cada protocolo deve ter especificidades da condição primária além do template universal.

---

## Don't Hand-Roll

| Problema | Não construir | Usar em vez disso | Por que |
|----------|--------------|-------------------|---------|
| Estadiamento funcional IC | Sistema de classificação próprio | NYHA I–IV (AHA/ACC) | Universal, validado, usado para critérios de elegibilidade em todos os trials |
| Estadiamento DPOC | Classificação obstrutiva proprietária | GOLD ABCD (FEV1 + mMRC ou CAT) | Standard mundial; define risco de exacerbação e elegibilidade PR |
| Escala de esforço percebido | Criar escala numérica interna | Borg RPE 6–20 (intensidade) + Borg Dispneia 0–10 (dispneia) | Ambas validadas, em uso clínico universal, sem custo |
| Instrumento de QV para IC | Questionário interno de impacto | MLHFQ (Minnesota Living with Heart Failure Questionnaire) | Instrumento de desfecho específico IC com MCID estabelecido |
| Instrumento de impacto DPOC | Questionário sintomático próprio | CAT — COPD Assessment Test | Padrão GOLD; 8 itens; score 0–40; MCID ≥ 2 pontos |
| Referência normativa TC6M | Calcular percentuais por grupo etário manual | Equação Britto et al. 2013 (J Pneumol) para população brasileira | Única equação de referência validada em população brasileira adulta |
| Intensidade aeróbica em IC | % FC máxima predita por idade | RPE 11–14 (Borg 6–20) + verificação FC se disponível | FC embotada por betabloqueador; RPE é o único indicador confiável |

---

## Common Pitfalls

### Pitfall 1: Limiar de SpO2 — 88% vs 90% vs 85%
**O que dá errado:** A literatura apresenta variação real de prática nos limiares de parada por SpO2 em exercício em DPOC (estudos reportam de 79–92% como limiares usados em PR). Adotar o limiar errado gera subnotificação de risco (muito baixo) ou interrupções desnecessárias (muito alto).
**Por que acontece:** Diferentes diretrizes usam limiares diferentes para repouso vs. exercício; confusão entre limiar de suplementação de O2 e limiar de suspensão.
**Como evitar:** Adotar 90% como limiar conservador para início e parada de exercício em contexto geriátrico. SpO2 < 88% em qualquer momento = suspensão imediata. SpO2 ≤ 90% no início da sessão = não iniciar exercício aeróbico sem suplementação. Documentar e justificar explicitamente no protocolo.
**Sinais de alerta:** Paciente relata dispneia subjetiva mas SpO2 ainda ≥ 90% — monitorar ambos; SpO2 pode dessaturar com delay após início de exercício.

### Pitfall 2: FC como Parâmetro de Intensidade em IC com Betabloqueador
**O que dá errado:** Clínico prescreve exercício a 60–70% FC máxima. Paciente em betabloqueador não atinge FC calculada mesmo com esforço moderado-alto. Resultado: subintensidade crônica ou — pior — tentativa de aumentar esforço até atingir FC-alvo com risco de sobrecarga.
**Por que acontece:** Currículo padrão de prescrição de exercício foca em % FC máxima; betabloqueador não é sempre documentado no prontuário de reabilitação.
**Como evitar:** P-16 declara explicitamente: "FC como parâmetro de intensidade é CONTRAINDICADO em pacientes com betabloqueador. Usar RPE Borg 6–20 exclusivamente; alvo RPE 11–14 (moderado)." Verificar lista de medicamentos na admissão — documentar betabloqueador como modificador na Seção 10 (Polifarmácia).
**Sinais de alerta:** FC de repouso ≤ 50 bpm; FC máxima durante esforço submáximo ≤ 80 bpm = betabloqueador ativo.

### Pitfall 3: Peso Diário — Não Instruído ou Não Integrado ao Protocolo
**O que dá errado:** Fisioterapeuta não inclui instrução de peso diário no componente educacional; paciente não monitora e apresenta ganho de 4–5 kg antes da próxima sessão com sinais de descompensação.
**Por que acontece:** Monitoramento de peso é frequentemente percebido como responsabilidade da cardiologia, não da fisioterapia. Falta de interface protocolar clara.
**Como evitar:** P-16 inclui seção explícita de Monitoramento Domiciliar com: instrução de pesagem (mesma balança, manhã, após micção, antes de comer), limiar de alerta (≥ 2 kg em 3 dias ou ≥ 1,5 kg em 24h), e pathway de comunicação com cardiologista. Reforçar na primeira sessão e a cada 2 semanas.
**Sinais de alerta:** Edema de tornozelo progressivo na chegada à sessão; dispneia em repouso; ganho de peso relatado > 1 kg desde a sessão anterior = não iniciar exercício, contatar médico assistente.

### Pitfall 4: Termorregulação em IC — Orientação Omitida
**O que dá errado:** Paciente com IC faz sessão em ambiente quente (> 28°C) ou vai caminhando para a clínica em dia quente. Vasodilatação cutânea em IC já está comprometida (redução de ~50% comparado a controles — AHA Circulation 2005). Risco de hipertermia e colapso circulatório.
**Por que acontece:** Impacto da termorregulação em IC é pouco lembrado no currículo de reabilitação cardíaca. Betabloqueadores agravam adicionalmente a resposta sudorífica.
**Como evitar:** P-16 inclui subseção de Termorregulação com: temperatura-alvo do ambiente de sessão (≤ 22°C ideal, máx 26°C), orientação de hidratação pré-sessão (200 mL água 30 min antes se sem restrição hídrica), instrução ao paciente sobre risco em dias quentes, suspensão de sessão se temperatura ambiente > 30°C sem climatização.

### Pitfall 5: Retroactive Update — Inconsistência de Formato entre Protocolos
**O que dá errado:** Passe retroativo adiciona seção de Precauções Cardiorrespiratórias com texto diferente em cada protocolo — limiares inconsistentes, tabelas com colunas distintas, terminologia variável.
**Por que acontece:** Cada protocolo já tem uma Seção 11 com conteúdo próprio. Sem um template fixo, a adaptação manual gera variação.
**Como evitar:** 06-02 começa lendo a Seção 11 de P-15 e P-16 para extrair o template UNIVERSAL fixo antes de qualquer edição retroativa. Aplicar o template verbatim para a subseção 11.1 (protocolo pré-sessão universal) e adaptar apenas 11.3 e 11.4 para especificidades de cada protocolo. Verificar consistência de limiares (SpO2 90%, PA > 180/110, FC > 120 em repouso) em todos os 10 arquivos após edição.

### Pitfall 6: Diferenciação IC-FEr vs IC-FEp Omitida
**O que dá errado:** P-16 prescreve da mesma forma para IC com fração de ejeção reduzida (IC-FEr, ≤ 40%) e IC com fração de ejeção preservada (IC-FEp, ≥ 50%) — população geriátrica tem alta prevalência de IC-FEp (50–70% nos ≥ 70 anos).
**Por que acontece:** Trials históricos de reabilitação cardíaca focaram em IC-FEr. IC-FEp é mais difícil de diagnosticar e menos estudada.
**Como evitar:** P-16 inclui declaração de escopo diferenciando IC-FEr e IC-FEp, com referência ao AHA Scientific Statement de IC-FEp (Circulation 2023 — CIR.0000000000001122) para a subpopulação geriátrica dominante. Não re-derivar toda a lógica de IC-FEp — citar o statement e adaptar dosagem conservadoramente.

---

## Code Examples

Padrões verificados a partir de diretrizes e protocolos existentes nesta série:

### Template: Protocolo de Sinais Vitais Pré-Sessão (Universal)

```markdown
### 11.1 Protocolo de Avaliação Pré-Sessão (UNIVERSAL — SHARED-FOUNDATION Seção 7.4)

**Registrar antes de cada sessão:**

| Parâmetro | Procedimento | Critério de NÃO-INÍCIO |
|-----------|-------------|----------------------|
| PA sistólica/diastólica | Repouso sentado, 5 min, braço direito | > 180/110 mmHg = aguardar + contatar médico |
| FC de repouso | Pulso radial ou monitor | > 120 bpm em repouso = não iniciar |
| SpO2 basal | Oxímetro de pulso, dedo indicador, 2 min repouso | ≤ 90% = não iniciar exercício aeróbico sem avaliação |
| Dispneia em repouso | Borg 0–10 | ≥ 5 em repouso = não iniciar |
| Edema de tornozelo | Inspeção bilateral | Novo edema ou piora aguda = contatar médico antes |
```

### Template: Critérios de Parada Imediata (Universal)

```markdown
### 11.2 Indicadores de Parada Imediata

| Indicador | Limiar |
|-----------|--------|
| Dor torácica, pressão precordial ou irradiação | Qualquer ocorrência |
| Dispneia súbita desproporcional ao esforço | Qualquer ocorrência |
| Palpitações com tontura ou síncope | Qualquer ocorrência |
| PA sistólica durante exercício | > 200 mmHg |
| Queda de PA sistólica durante esforço progressivo | > 10 mmHg |
| SpO2 durante exercício | < 90% |
| Cianose perioral ou periférica | Qualquer ocorrência |
| Confusão mental de início agudo | Qualquer ocorrência |
```

### Template: Prescrição de Intensidade — DPOC (Borg Dispneia)

```markdown
**Alvo de intensidade aeróbica P-15:**
- Borg Dispneia (0–10): alvo 4–6 (dispneia moderada, controlável, permite fala)
- Equivalência: 60–80% da capacidade máxima ao TC6M
- Faixa Frágil: iniciar Borg 3–4; progredir apenas com Borg < 4 ao final da sessão
- Interromper se Borg Dispneia ≥ 7 (dispneia muito intensa) ou SpO2 < 90%
```

### Template: Prescrição de Intensidade — IC (RPE Borg 6–20)

```markdown
**Alvo de intensidade aeróbica P-16:**
- RPE Borg (6–20): alvo 11–14 (esforço leve a moderado)
- FC NÃO usar como parâmetro se betabloqueador em uso (registrar na Seção 10)
- RPE 10–11 ≈ limiar ventilatório 1 (LV1) — alvo inicial para IC-FEr
- RPE 13–14 ≈ limiar ventilatório 2 (LV2) — teto máximo; nunca exceder
- Faixa Frágil / NYHA III: iniciar RPE 10–11; nunca exceder RPE 12
```

### Padrão: Diferenciação de Escopo — DPOC (o que NÃO cobre)

```markdown
> **NÃO COBRE este protocolo:**
> - Asma brônquica não-DPOC → protocolo específico não incluído nesta série
> - DPOC com instabilidade aguda (exacerbação em curso) → cuidado hospitalar agudo
> - Insuficiência Cardíaca como diagnóstico primário → P-16
> - Hipertensão Pulmonar severa (PAP sistólica > 55 mmHg) → avaliação cardiológica antes
> - Necessidade de oxigenoterapia domiciliar contínua com SpO2 ≤ 88% em repouso → coordenação médica antes do início de PR
```

### Padrão: Seção de Monitoramento de Peso Diário — IC

```markdown
### [Seção] Monitoramento Domiciliar — Protocolo de Peso Diário

**Instrução ao paciente:**
- Pesagem diária: mesma balança, pela manhã, após urinar, antes de comer
- Registrar em diário de sintomas (modelo fornecido na Seção de Educação)

**Limiar de alerta — contatar cardiologista/médico assistente:**
| Ganho de peso | Ação |
|---------------|------|
| ≥ 1,5 kg em 24 horas | Contato urgente com médico — SUSPENDER sessão de exercício |
| ≥ 2,0 kg em 3 dias | Contato com médico — SUSPENDER sessão até avaliação |
| ≥ 2,5 kg em 7 dias | Contato com médico — SUSPENDER sessão até avaliação |

> **Nota:** Limiar de 2 kg/3 dias — referência: ESC Heart Failure Guidelines 2021 (recomendação de auto-monitoramento para detecção precoce de descompensação).
```

---

## State of the Art

| Abordagem Antiga | Abordagem Atual | Mudança | Impacto |
|-----------------|----------------|---------|---------|
| PR apenas para DPOC moderada-grave (GOLD III-IV) | PR recomendada para DPOC desde GOLD II (FEV1 50–80%) com sintomas | ATS 2023 Guideline | Expandir critérios de elegibilidade em P-15 além de GOLD III-IV |
| FC-alvo (% FCmáx) para prescrição em IC | RPE Borg exclusivo em IC com betabloqueador | Reconhecimento explícito de cronotropia negativa | Modificador mandatório em P-16 — FC proibida como indicador único |
| Reabilitação cardíaca apenas para IC-FEr | IC-FEp: exercício Classe I (AHA 2023 Scientific Statement) | Equilíbrio das evidências IC-FEr vs IC-FEp | P-16 precisa cobrir ambas as subformas com diferenciação |
| SpO2 monitorada apenas se sintomática | SpO2 contínua/intermitente mandatória em DPOC durante exercício | Evidência de dessaturação silenciosa em DPOC | Monitoramento ativo independente de dispneia subjetiva |
| PR apenas presencial | PR presencial OU telerreabilitação (escolha do paciente) | ATS 2023 (recomendação condicional) | P-15 pode mencionar telerreabilitação como opção; foco permanece no presencial geriátrico |

**Itens desatualizados/depreciados:**
- FC como monitor primário de intensidade em IC: substituído por RPE em pacientes com betabloqueador
- Restrição de exercício para NYHA III: AHA/ACC 2022 recomenda exercício supervisionado em NYHA III estável como Classe I
- ATS/ERS Position Statement 2013 de Reabilitação Pulmonar: substituído pelo ATS Clinical Practice Guideline 2023 (PMID 37581410)

---

## Open Questions

1. **Status final da ATS/ERS 2023 Pulmonary Rehabilitation Guideline**
   - O que sabemos: PMID 37581410 (Aug 2023) confirmado. Recomendação forte para DPOC estável.
   - O que está pendente: Verificar se há adendo ou corrigendum publicado entre set/2023 e mar/2026 antes de citar como definitivo.
   - Recomendação: Verificar PubMed com filtro 2024–2026 por "pulmonary rehabilitation guidelines" antes de finalizar P-15.

2. **Equação de referência TC6M para população brasileira geriátrica com DPOC**
   - O que sabemos: Britto et al. 2013 (J Pneumol) fornece equação para adultos saudáveis 20–80 anos no Brasil. Dados de idosos com DPOC chineses (PMC10258361) mostram DTC6 médio de 215–305 m por faixa etária.
   - O que está pendente: Equação de referência específica para idosos brasileiros com DPOC — pode não existir. Usar equação Britto 2013 + ajuste clínico pelo GOLD stage.
   - Recomendação: P-15 usa Britto 2013 como referência com nota de limitação; MCID de 25–30 m é o threshold clínico prioritário.

3. **Versão brasileira validada do MLHFQ e do CAT**
   - O que sabemos: MLHFQ tem tradução e uso no Brasil; CAT tem versão BR no GOLD.
   - O que está pendente: Citações de validação peer-reviewed específicas em PT-BR para MLHFQ e CAT (análogo ao padrão estabelecido para WOMAC-BR e SPPB-BR).
   - Recomendação: Buscar PubMed "Minnesota Living Heart Failure Portuguese Brazil" + "COPD Assessment Test validation Brazil" antes de citar como ferramentas validadas BR.

4. **Retroactive Update — Seção 11 nos 10 protocolos existentes**
   - O que sabemos: Todos os 10 protocolos têm uma Seção 11 com algum conteúdo de precauções cardiorrespiratórias (variando de básico a moderado — P-03 e P-06 têm conteúdo mais robusto).
   - O que está pendente: Identificar o nível exato de completude em cada protocolo antes do passe retroativo.
   - Recomendação: Plano 06-02 deve começar lendo e tabelando o status atual da Seção 11 de todos os 10 protocolos antes de editar qualquer um.

---

## Validation Architecture

> nyquist_validation está habilitado no config.json (workflow.nyquist_validation: true).

### Test Framework

| Property | Value |
|----------|-------|
| Framework | Não aplicável — repositório de documentação clínica sem suite de testes automatizados |
| Config file | none |
| Quick run command | Inspeção manual de estrutura + contagem de seções obrigatórias por protocolo |
| Full suite command | Verificação de 8 questões de validade clínica (Seção 15 de cada protocolo) + checklist de seção universal |

### Phase Requirements → Test Map

| Req ID | Comportamento | Tipo de Teste | Comando / Método | Existe? |
|--------|---------------|---------------|-----------------|---------|
| PROT-11 | P-15 DPOC: SpO2 com limiares de início/parada operacionais presentes | Inspeção manual da Seção 11 | `grep -n "SpO2\|90%\|88%" protocols/P-15-DPOC.md` | Arquivo a criar na Wave 1 |
| PROT-11 | P-15 DPOC: TC6M como desfecho primário com MCID documentado | Inspeção da Seção 12 | `grep -n "TC6M\|MCID\|25 m\|30 m" protocols/P-15-DPOC.md` | Arquivo a criar na Wave 1 |
| PROT-11 | P-15 DPOC: referência ATS/ERS declarada no cabeçalho | Inspeção do cabeçalho | `grep -n "ATS\|ERS\|37581410" protocols/P-15-DPOC.md` | Arquivo a criar na Wave 1 |
| PROT-12 | P-16 IC: RPE-only declarado com justificativa de betabloqueador | Inspeção Seções 10 + 11 | `grep -n "RPE\|Borg\|betabloqueador\|FC embotada" protocols/P-16-INSUFICIENCIA-CARDIACA.md` | Arquivo a criar na Wave 1 |
| PROT-12 | P-16 IC: protocolo de peso diário com limiares e pathway cardiologia | Inspeção da seção de monitoramento | `grep -n "peso diário\|2 kg\|cardiologista" protocols/P-16-INSUFICIENCIA-CARDIACA.md` | Arquivo a criar na Wave 1 |
| PROT-12 | P-16 IC: orientação de termorregulação presente | Inspeção da Seção 11 | `grep -n "termorregula\|temperatura\|calor\|hidrata" protocols/P-16-INSUFICIENCIA-CARDIACA.md` | Arquivo a criar na Wave 1 |
| SC-3 (Phase 6) | Todos 10 protocolos Fases 1–5 têm Seção 11 com template universal | Inspeção retroativa | `grep -c "11.1 Protocolo de Avaliação Pré-Sessão\|Protocolo.*Pré-Sessão" protocols/P-*.md` | Verificação no Wave 2 |

### Sampling Rate

- **Por commit de tarefa:** Inspeção de grep dos marcadores críticos listados acima
- **Por wave merge:** Verificação de 8 questões de validade clínica (Seção 15) + todas as seções obrigatórias presentes (1–15)
- **Phase gate:** Checklist de 3 critérios de sucesso + documentação do passe retroativo antes de `/gsd:verify-work`

### Wave 0 Gaps

Nenhuma lacuna de infraestrutura — repositório de documentação não tem suite de testes.
Gaps específicos de conteúdo a resolver antes da implementação:
- [ ] Verificar citação BR validada para MLHFQ (Minnesota Living with Heart Failure Questionnaire)
- [ ] Verificar citação BR validada para CAT (COPD Assessment Test)
- [ ] Confirmar status de ATS/ERS 2023 Guideline (adendo/corrigendum 2024–2026)

---

## Sources

### Primary (HIGH confidence)
- PubMed 37581410 — ATS Clinical Practice Guideline: Pulmonary Rehabilitation for Adults with Chronic Respiratory Disease (2023) — recomendações para DPOC estável e pós-exacerbação, confirmado publicado American Journal of Respiratory and Critical Care Medicine
- AHA Circulation DOI 10.1161/CIR.0000000000001063 — 2022 AHA/ACC/HFSA Guideline for Management of Heart Failure — exercício Classe I para IC independente de fração de ejeção
- PMC8387006 — Diretriz Brasileira de Reabilitação Cardiovascular 2020 (Arq Bras Cardiol) — protocolo brasileiro de reabilitação em IC, NYHA, Borg, medicamentos com efeito cronotrópico negativo
- PMC3990937 — "Perceived Exertion as Exercise Intensity Indicator in Chronic Heart Failure Patients on Beta-Blockers" — evidência para RPE como único indicador confiável em IC com betabloqueador
- GOLD 2025 Report (goldcopd.org — publicado nov 2024) — estadiamento ABCD, mMRC, CAT, elegibilidade para reabilitação pulmonar

### Secondary (MEDIUM confidence)
- AHA Circulation 2006 (DOI 10.1161/circulationaha.105.540773) — Effects of Heat Stress on Thermoregulatory Responses in Congestive Heart Failure — vasodilatação cutânea reduzida ~50% em IC
- PMC4042428 — Cardiovascular responses to heat stress in chronic heart failure — confirma comprometimento termorregulador em IC
- Britto RR et al. 2013 (Jornal Brasileiro de Pneumologia) — "Six-minute walk test: reference values for healthy adults in Brazil" — equação de referência BR para TC6M (adultos saudáveis; não específica para DPOC geriátrico)
- AHA Circulation DOI 10.1161/CIR.0000000000001122 — AHA Scientific Statement: Supervised Exercise Training for HFpEF 2023 — base para cobertura de IC-FEp em P-16
- PMC10258361 — Decline with age for 6MWT in Chinese older adults with COPD — dados normativos DTC6 por faixa etária em DPOC (215–305 m); população chinesa, aplicar com cautela no contexto BR

### Tertiary (LOW confidence)
- ESC Heart Failure Guidelines 2021 — limiar de peso diário ≥ 2 kg em 3 dias como alerta de descompensação — citado em literatura secundária; verificar citação primária ESC antes de uso definitivo
- PMC10847087 — Practical Guidelines for Exercise Prescription in CHF (2024) — RPE alvo 11–14 para IC; texto confirma RPE 10–11 ≈ LV1 e RPE 13–14 ≈ LV2
- Tandfonline COPD-200050527 — Minimal Clinically Important Differences in 6MWT — MCID de 25–35 m em DPOC (baixa certeza — estimativas variam 25–80 m na literatura)

---

## Metadata

**Confidence breakdown:**
- Standard stack (instrumentos, diretrizes): HIGH — ATS 2023, AHA/ACC/HFSA 2022, Diretriz BR 2020 confirmados; instrumentos universalmente estabelecidos
- Architecture patterns (sequência P-15 → P-16 → retroativo): HIGH — lógica de dependência interna ao projeto; estrutura de template derivada de protocolos existentes
- Pitfalls (FC em IC, SpO2 limiares, termorregulação): MEDIUM-HIGH — fisiopatologia bem estabelecida; limiares operacionais têm variação real de prática documentada
- MCID TC6M em DPOC geriátrico: MEDIUM — MCID 25–30 m mais conservador é consenso ERS; limites superiores (54–80 m) são estimativas distribucional
- Validação BR para MLHFQ e CAT: LOW — não confirmada com citação peer-reviewed específica; a confirmar durante execução

**Research date:** 2026-03-13
**Valid until:** 2026-06-13 (estável — diretrizes principais são de 2022–2023; próxima revisão GOLD prevista para nov 2025, já incorporado como GOLD 2025)
