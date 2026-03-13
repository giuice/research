# Protocolo P-08 — Sarcopenia / Fraqueza Muscular Generalizada

**Documento:** P-08-SARCOPENIA.md
**Versão:** 1.0
**Data:** 2026-03-13
**Condição-alvo:** Sarcopenia — redução de força muscular e massa muscular esquelética em idosos
**População:** Idosos ≥ 60 anos com sarcopenia provável ou confirmada (EWGSOP2 FACS)
**Setting:** Centro de reabilitação geriátrica ambulatorial ou hospitalar-dia
**Idioma:** Português Brasileiro
**Padrão de Relatório:** TIDieR (Template for Intervention Description and Replication) + CERT (Consolidated Standards of Reporting Trials — Exercise)
**Alinhamento de Diretrizes:**
- EWGSOP2 2019 — Cruz-Jentoft AJ et al. Age Ageing 2019;48(1):16-31. PubMed 30312372
- GLIS 2024 Conceptual Consensus — Kirk B et al. Age Ageing 2024. PMC11210221 (contextual apenas)
- ESPEN Protein Guidelines 2018 — Deutz NEP et al. Clin Nutr 2019. PubMed 30177463
- ACSM Position Stand — Resistance Training for Older Adults 2019. PubMed 30860922
- AGS Beers Criteria 2023 — verificar atualizações 2025/2026 antes da publicação definitiva

> **Nota EWGSOP2/GLIS 2024:** Os critérios operacionais usados neste protocolo são baseados em EWGSOP2 (2018), que permanece o padrão vigente. O GLIS 2024 (Kirk B et al., PMC11210221) estabeleceu uma definição conceitual global, mas afirmou explicitamente que "os critérios operacionais serão desenvolvidos em etapa subsequente." Nenhum cutoff numérico do GLIS foi publicado até março de 2026. Verificar Age Ageing journal para atualização antes de publicação definitiva deste protocolo.

> **Princípio Norteador:** "Start low, go slow, but reach the goal" — Todo exercício começa no limite inferior da faixa clínica aceitável para o nível de fragilidade do paciente, progride devagar com critérios funcionais objetivos, e visa metas funcionais individualizadas — não um número de sessões.

> **Protocolo Autossuficiente:** Este documento foi elaborado para ser completo e independente. O clínico pode utilizá-lo sem consultar qualquer outro documento. Elementos da Camada de Fundação Compartilhada (SHARED-FOUNDATION.md) são reproduzidos inline onde necessário.

> **Papel como Modificador Transversal:** Adicionalmente ao seu papel como protocolo clínico autossuficiente, este documento provê a tabela normativa de dosagem de exercício resistido estratificada por fragilidade para todos os 20 protocolos desta série. Ver Seção 6.3.

---

## Índice

1. [Critérios Diagnósticos e de Inclusão](#1-critérios-diagnósticos-e-de-inclusão)
2. [Avaliação Inicial Mandatória](#2-avaliação-inicial-mandatória)
3. [Alinhamento com Diretrizes](#3-alinhamento-com-diretrizes)
4. [Estrutura de Fases](#4-estrutura-de-fases)
5. [Fase 1 — Adaptação e Condicionamento Inicial](#5-fase-1--adaptação-e-condicionamento-inicial)
6. [Fase 2 — Fortalecimento Progressivo](#6-fase-2--fortalecimento-progressivo)
7. [Fase 3 — Manutenção Funcional](#7-fase-3--manutenção-funcional)
8. [Monitoramento de Dor](#8-monitoramento-de-dor)
9. [Bandeiras Vermelhas e Escalonamento](#9-bandeiras-vermelhas-e-escalonamento)
10. [Interações com Polifarmácia](#10-interações-com-polifarmácia)
11. [Precauções Cardiorrespiratórias](#11-precauções-cardiorrespiratórias)
12. [Indicadores de Desfecho](#12-indicadores-de-desfecho)
13. [Rastreabilidade e Flags de Comorbidade](#13-rastreabilidade-e-flags-de-comorbidade)
14. [Referências por Nível de Evidência](#14-referências-por-nível-de-evidência)
15. [As 8 Questões de Validade Clínica](#15-as-8-questões-de-validade-clínica)

---

## 1. Critérios Diagnósticos e de Inclusão

### 1.1 Algoritmo EWGSOP2 FACS — Fluxo Diagnóstico Operacional

*Fonte: Cruz-Jentoft AJ et al. EWGSOP2. Age Ageing 2019;48(1):16-31. PubMed 30312372*

O diagnóstico de sarcopenia segue o algoritmo de 4 etapas FACS: **F**ind (Encontrar) → **A**ssess (Avaliar) → **C**onfirm (Confirmar) → **S**everity (Gravidade).

```
ETAPA F — ENCONTRAR (RASTREIO)
SARC-F ≥ 4 pontos?
  └─ NÃO → Vigilância anual (repetir SARC-F); orientar exercício preventivo
  └─ SIM → SARCOPENIA PROVÁVEL — avançar para Etapa A

ETAPA A — AVALIAR FORÇA
Força de preensão palmar (Jamar):
  └─ ≥ 27 kg (Masculino) / ≥ 16 kg (Feminino) → Sarcopenia improvável; monitorar
  └─ < 27 kg (Masculino) / < 16 kg (Feminino) → SARCOPENIA PROVÁVEL confirmada
       └─ Alternativa quando Jamar indisponível: Levantar-sentar 5× > 15 seg = baixa força
       └─ Avançar para Etapa C

ETAPA C — CONFIRMAR MASSA MUSCULAR
Massa muscular esquelética apendicular (ASM/h²) — DEXA ou BIA:
  └─ DEXA: ASM/h² ≥ 7,0 kg/m² (M) / ≥ 5,5 kg/m² (F) → Sarcopenia NÃO confirmada; tratar fraqueza
  └─ DEXA: ASM/h² < 7,0 kg/m² (M) / < 5,5 kg/m² (F) → SARCOPENIA CONFIRMADA
       └─ Avançar para Etapa S

ETAPA S — AVALIAR GRAVIDADE
Desempenho físico:
  └─ Velocidade de marcha 4m < 0,8 m/s        → SARCOPENIA GRAVE
  └─ SPPB-BR ≤ 8 pontos (alternativa)          → SARCOPENIA GRAVE
  └─ TUG > 20 segundos (alternativa)            → SARCOPENIA GRAVE
  └─ Nenhum dos critérios acima presentes       → SARCOPENIA CONFIRMADA (sem gravidade)
```

> **Nota Operacional:** O GLIS 2024 (PMC11210221) estabeleceu definição conceitual global de sarcopenia como "redução de função muscular e massa muscular esquelética" — porém, sem cutoffs operacionais revisados publicados até março de 2026. Este protocolo usa os cutoffs EWGSOP2 (2018) como padrão operacional vigente.

---

### 1.2 SARC-F — Instrumento de Rastreio (Etapa F do FACS)

*Fonte: Morley JE et al. J Am Med Dir Assoc 2013. Validado em múltiplas populações internacionais.*

| Pergunta | 0 pontos | 1 ponto | 2 pontos |
|----------|---------|---------|---------|
| **Força:** Quanta dificuldade você tem para levantar e carregar 4,5 kg? | Nenhuma | Alguma | Muita / incapaz |
| **Assistência para caminhar:** Quanta dificuldade você tem para caminhar por um cômodo? | Nenhuma | Alguma | Muita / usa aparelho / incapaz |
| **Levantar de cadeira:** Quanta dificuldade você tem para levantar de uma cadeira? | Nenhuma | Alguma | Muita / incapaz sem ajuda |
| **Subir escadas:** Quanta dificuldade você tem para subir 10 degraus? | Nenhuma | Alguma | Muita / incapaz |
| **Quedas:** Quantas vezes você caiu no último ano? | Nenhuma | 1–3 quedas | 4 ou mais quedas |

**Interpretação:** 0–3 = rastreio negativo; **≥ 4 = rastreio positivo — avançar para avaliação completa FACS**

---

### 1.3 Critérios de Inclusão neste Protocolo

| # | Critério |
|---|----------|
| 1 | Idade ≥ 60 anos |
| 2 | SARC-F ≥ 4 (rastreio positivo) |
| 3 | Força de preensão abaixo dos limiares EWGSOP2: Masculino < 27 kg; Feminino < 16 kg |
| 4 | Capacidade de compreender e executar a bateria de avaliação inicial mandatória (MoCA-BR ≥ 18 ou familiar/cuidador disponível) |
| 5 | Consentimento informado obtido |
| 6 | Capaz de deambular com ou sem dispositivo auxiliar de marcha |

---

### 1.4 Critérios de Exclusão

| # | Critério de Exclusão | Encaminhamento |
|---|---------------------|----------------|
| 1 | Doença neuromuscular primária (ELA, miopatia inflamatória ativa, distrofia muscular progressiva) | Neurologia / Reumatologia |
| 2 | Caquexia oncológica ativa (perda de peso > 5% nos últimos 6 meses por neoplasia ativa) | Oncologia / Cuidados Paliativos |
| 3 | Condição cardíaca instável (angina instável, IC descompensada, arritmia não controlada) | Cardiologista |
| 4 | Comprometimento cognitivo grave (MoCA-BR < 18 sem cuidador disponível) que impeça consentimento e compreensão das instruções | Geriatria / Neurologia |
| 5 | Fratura aguda ou fratura de stress não consolidada em membro inferior | Ortopedia |
| 6 | Infecção sistêmica ativa ou febre (> 37,8°C) | Clínico / Urgência |
| 7 | Dor muscular severa em repouso (NRS ≥ 8) sem diagnóstico etiológico — excluir rabdomiólise | Clínico / Urgência |

> **Nota:** Critérios de exclusão referem-se ao início imediato do protocolo. Após resolução da condição excludente, o paciente pode ser reavaliado para inclusão.

---

## 2. Avaliação Inicial Mandatória

> Esta bateria deve ser aplicada **antes de qualquer intervenção** e repetida a cada transição de fase. Os resultados determinam a classificação de fragilidade (Fenótipo de Fried) e a faixa de dosagem inicial.

### 2.1 TUG — Timed Up and Go

**Finalidade:** Avaliação de mobilidade funcional, marcha e risco de queda. Critério de gravidade EWGSOP2 quando > 20 seg.

**Equipamento:** Cronômetro; cadeira padrão (~46 cm de altura, com ou sem apoio de braços — registrar); fita métrica; marcador de 3 metros no chão.

**Procedimento Padronizado:**
1. Demonstrar o teste antes da execução
2. Permitir 1 ensaio de familiarização
3. Registrar a média de 2 tentativas (ou 3 se variação > 2 seg entre tentativas)
4. Calçado habitual; registrar uso de dispositivo auxiliar de marcha

**Instrução ao Paciente:** "Ao meu sinal, levante-se, caminhe até a marca no chão, vire e retorne para sentar o mais rápido que conseguir com segurança."

| Faixa Etária | Média (seg) | Interpretação Clínica |
|-------------|-------------|----------------------|
| 60–64 anos | ~8,1 | Referência comunitária |
| 71–75 anos | 9,5 ± 2,5 | Referência comunitária |
| 76–80 anos | 9,9 ± 3,0 | Atenção se > 12 seg |
| 81–85 anos | 11,2 ± 3,6 | Atenção se > 13,5 seg |
| 86–99 anos | 12,0 ± 3,8 | Alto risco se > 13,5 seg |

*Fonte: Ibrahim A et al. PLoS One 2017; PMC5626462*

**MCID:** 2,0–3,0 segundos | **Limiar de risco de queda:** > 13,5 seg | **Critério EWGSOP2 de gravidade:** > 20 seg

---

### 2.2 SPPB-BR — Short Physical Performance Battery (Versão Brasileira)

**Finalidade:** Avaliação de desempenho físico; critério de gravidade EWGSOP2 quando ≤ 8 pontos.

*Validação Brasileira: Nakano MM 2007. ICC = 0,83 (teste-reteste). Fonte: Guralnik JM et al. JAMA 1994; Pavasini R et al. PubMed 35341435*

**Subcomponentes (0–4 pontos cada; total 0–12):**

**1. Equilíbrio Estático (0–4 pontos):**
- Pés paralelos por 10 seg = 1 ponto; Semitândem por 10 seg = 1 ponto adicional; Tândem por 10 seg = 2 pontos adicionais

**2. Velocidade de Marcha 4m (0–4 pontos):**
- > 4,82 seg = 1 ponto; 3,82–4,82 = 2 pontos; 2,60–3,81 = 3 pontos; < 2,60 = 4 pontos

**3. Levantar-Sentar Repetido — 5× (0–4 pontos):**
- Incapaz ou > 60 seg = 0; 16,7–60 seg = 1; 13,7–16,6 = 2; 11,2–13,6 = 3; < 11,2 = 4

| Escore Total | Interpretação |
|-------------|---------------|
| 9–12 pontos | Desempenho preservado |
| 7–8 pontos | Limitação leve |
| 4–6 pontos | Limitação moderada a grave |
| 0–3 pontos | Comprometimento grave |

**MCID:** 0,5 pontos (pequena); 1,0 ponto (substancial) | **Critério EWGSOP2 de gravidade:** ≤ 8 pontos

---

### 2.3 Dinamometria Manual — Dinamômetro Jamar

**Finalidade:** Avaliação de força de preensão palmar — marcador primário de sarcopenia (EWGSOP2) e critério de diagnóstico na Etapa A do FACS.

*Fonte: Dodds RM et al. Age Ageing 2016; EWGSOP2 — Cruz-Jentoft AJ et al. Age Ageing 2019;48(1):16-31. PubMed 30312372*

**Procedimento Padronizado:**
1. Paciente sentado, ombro em adução, cotovelo fletido a 90°, antebraço neutro
2. Três tentativas na mão dominante com 60 segundos de intervalo
3. Registrar o maior valor das três tentativas (em kgf)
4. Registrar ajuste de alça utilizado e presença de dor durante o teste

| Sexo | Limiar EWGSOP2 (Baixa Força) | Faixa Normal (60–69 anos) | MCID |
|------|------------------------------|--------------------------|------|
| Masculino | < 27 kg | 35,0–40,0 kg | 5,0–6,5 kg |
| Feminino | < 16 kg | 19,0–24,0 kg | 2,7–5,0 kg |

> **Nota EWGSOP2:** Os limiares acima são baseados em EWGSOP2 (2018). Verificar publicação de EWGSOP3 antes de finalizar qualquer protocolo — se disponível, atualizar os limiares conforme nova edição.

---

### 2.4 Velocidade de Marcha 4m

**Finalidade:** Critério de gravidade EWGSOP2 na Etapa S do FACS; componente do SPPB-BR.

**Procedimento:** Paciente caminha 4 metros em linha reta ao passo confortável; cronometrar apenas os 4 metros centrais (excluindo aceleração/desaceleração se corredor > 4 metros disponível). Registrar em seg e calcular m/s.

| Velocidade | Interpretação EWGSOP2 |
|-----------|----------------------|
| < 0,8 m/s | Sarcopenia GRAVE — critério de gravidade |
| 0,8–1,0 m/s | Velocidade limítrofe — monitorar |
| > 1,0 m/s | Velocidade preservada |

---

### 2.5 MoCA-BR — Montreal Cognitive Assessment (Versão Brasileira)

**Finalidade:** Triagem cognitiva — fragilidade cognitiva é frequente em sarcopenia; avaliação prévia orienta estratégias de comunicação e autonomia.

*Validação: Memoria CM et al. Int Psychogeriatr 2013; PubMed 22368034*

| Escore (com ajuste) | Interpretação |
|--------------------|---------------|
| ≥ 26 | Função cognitiva preservada |
| < 26 | Rastreio positivo para CCL — adaptar estratégias de ensino e monitorar adesão |

> **Ajuste de Escolaridade (OBRIGATÓRIO):** Adicionar +1 ponto para pacientes com ≤ 12 anos de escolaridade formal. A população geriátrica brasileira tem alta prevalência de baixa escolaridade — aplicar o ajuste é essencial para evitar falsos positivos.

---

### 2.6 Classificação de Fragilidade — Fenótipo de Fried

*Fonte: Fried LP et al. J Gerontol A Biol Sci Med Sci 2001;56(3):M146-56*

Aplicar antes de selecionar a faixa de dosagem. Os 5 critérios de Fried:

| # | Critério | Definição Operacional |
|---|----------|----------------------|
| 1 | Perda de peso não intencional | ≥ 4,5 kg (ou ≥ 5% do peso corporal) no último ano |
| 2 | Exaustão/Fadiga autorrelatada | Resposta positiva a 2 itens da CES-D ≥ 3 dias/semana |
| 3 | Baixo nível de atividade física | < 383 kcal/sem (homens) ou < 270 kcal/sem (mulheres) |
| 4 | Lentidão de marcha | Velocidade < 0,8 m/s (ajustada por sexo e altura — limiares EWGSOP2) |
| 5 | Fraqueza muscular | Força de preensão abaixo dos limiares EWGSOP2: H < 27 kg, M < 16 kg |

| Pontuação | Classificação | Implicação Clínica |
|-----------|---------------|-------------------|
| 0 critérios | **Robusto** | Dosagem padrão (linha Robusto nas tabelas) |
| 1–2 critérios | **Pré-frágil** | Dosagem adaptada (linha Pré-frágil nas tabelas) |
| ≥ 3 critérios | **Frágil** | Dosagem conservadora (linha Frágil nas tabelas) |

> **Fluxo decisório:** Aplicar SPPB-BR → Se SPPB ≤ 9, aplicar Fenótipo de Fried completo → Classificar → Selecionar linha da tabela de dosagem.

---

## 3. Alinhamento com Diretrizes

| Diretriz | Versão | Papel neste Protocolo | PubMed / Referência |
|----------|--------|----------------------|---------------------|
| EWGSOP2 | 2018 (publicado 2019) | **Primária** — diagnóstico, algoritmo FACS, cutoffs operacionais | PubMed 30312372 |
| GLIS 2024 Conceptual Consensus | 2024 | **Contextual apenas** — definição conceitual; sem cutoffs operacionais publicados | PMC11210221 |
| ESPEN Protein Guidelines | 2018/2019 | **Primária** — recomendações de ingestão proteica para idosos | PubMed 30177463 |
| PROT-AGE Study Group | 2013 | **Primária** — proteína ≥ 1,2 g/kg/dia para idosos ativos | PubMed 23867520 |
| ACSM Resistance Training Position Stand | 2019 | **Primária** — parâmetros de treinamento resistido para idosos | PubMed 30860922 |
| AGS Beers Criteria | 2023 | Referência de segurança farmacológica em idosos | PubMed 37139824 |
| AGS Beers 2025 Alternatives List | 2025 | Recurso suplementar — não substitui Beers 2023 | — |

> **Declaração de Prioridade:** Na presença de conflito entre diretrizes, a hierarquia é: (1) EWGSOP2 para diagnóstico; (2) ESPEN + PROT-AGE para nutrição; (3) ACSM para parâmetros de exercício resistido; (4) SHARED-FOUNDATION para estratificação por fragilidade e formato de dosagem.

---

## 4. Estrutura de Fases

### 4.1 Visão Geral das 3 Fases

| Fase | Nome | Foco Principal | Critérios de Entrada | Critérios de Saída |
|------|------|---------------|---------------------|-------------------|
| **Fase 1** | Adaptação e Condicionamento Inicial | Mobilização, condicionamento neuromuscular, familiarização com exercício resistido de baixa carga | Sarcopenia confirmada (EWGSOP2) + avaliação inicial completa | Força de preensão ↑ ≥ 2 kg OU SPPB-BR ↑ ≥ 1 ponto + tolerância a exercício resistido sem evento adverso por 2 sessões consecutivas |
| **Fase 2** | Fortalecimento Progressivo | Exercício resistido progressivo como intervenção principal; abordagem multicomponente (resistência + aeróbico + equilíbrio) | Critérios de saída da Fase 1 atingidos | Força de preensão acima do limiar EWGSOP2 (H > 27 kg; M > 16 kg) OU velocidade de marcha > 0,8 m/s OU SPPB-BR ≥ 10 pontos |
| **Fase 3** | Manutenção Funcional | Manutenção dos ganhos, independência nas AVDs, prevenção de recidiva | Critérios de saída da Fase 2 atingidos | Metas funcionais individualizadas mantidas por ≥ 4 semanas; transição para programa de exercício comunitário independente |

> **Regra Crítica de Transição:** A progressão entre fases ocorre EXCLUSIVAMENTE por critérios funcionais — não por número de semanas decorridas. A duração mínima de cada fase é orientativa; o critério de saída é o determinante da transição.

---

### 4.2 Duração Orientativa por Fase

| Fase | Duração Mínima | Duração Típica | Duração Máxima |
|------|---------------|----------------|----------------|
| Fase 1 | 3 semanas | 4–6 semanas | 8 semanas |
| Fase 2 | 8 semanas | 12–16 semanas | 24 semanas |
| Fase 3 | Contínua (manutenção) | 12–24 semanas supervisionadas | Indefinida (transição para autocuidado) |

*Duração mínima para ganhos mensuráveis em sarcopenia: 12 semanas de treinamento resistido. Fonte: PMC12602684 (2025).*

---

## 5. Fase 1 — Adaptação e Condicionamento Inicial

### 5.1 Modalidade Terapêutica — Fase 1

#### Eletroterapia / Termoterapia — Modulação Inicial de Desconforto Muscular

**Calor superficial (compressas quentes / infravermelho):**
Nível de Evidência: C (CEBM Nível 4-5)
Referência primária: Baseado em prática clínica estabelecida; sem ECR específico para sarcopenia
Alinhamento: Consenso clínico geriátrico — uso sintomático para rigidez matinal

Aplicação: 10–15 minutos em musculatura-alvo (quadríceps, glúteos, paravertebrais) antes do exercício resistido; temperatura máxima tolerável sem queimadura; contraindicado sobre áreas com alteração de sensibilidade.

**Estimulação Elétrica Neuromuscular — NMES:**
Nível de Evidência: B (CEBM Nível 2-3)
Referência primária: Paillard T. Ann Phys Rehabil Med 2022 — revisão sistemática NMES em sarcopenia.
Alinhamento: Opção complementar quando exercício ativo é limitado por dor ou fadiga excessiva.

Indicação: Paciente Frágil com incapacidade de realizar contração voluntária suficiente; usar como adjuvante ao exercício ativo. Frequência 30–50 Hz; largura de pulso 200–350 µs; intensidade até contração visível sem dor. 15–20 min por grupo muscular; 2–3×/semana.

---

### 5.2 Terapia Manual — Fase 1

**Mobilização miofascial e massagem terapêutica (técnicas de tecido mole):**
Nível de Evidência: C (CEBM Nível 4-5)
Referência primária: Prática clínica — sem ECR de alta qualidade específico para sarcopenia.
Alinhamento: Uso adjuvante para redução de rigidez muscular e melhora da percepção de movimento.

Aplicação: Effleurage e petrissage em grupos musculares maiores (quadríceps, isquiotibiais, glúteos); 10–15 minutos por região; pressão tolerável pelo paciente; evitar contusão. Objetivo: preparação para exercício ativo, não intervenção primária.

**Mobilização articular passiva e ativa-assistida (amplitude de movimento):**
Nível de Evidência: C (CEBM Nível 4-5)
Referência primária: Prática clínica geriátrica estabelecida.
Alinhamento: Manutenção ou recuperação de amplitude funcional — pré-requisito para exercício resistido seguro.

Aplicação: Mobilização suave de tornozelo, joelho, quadril e ombro; ADM funcional — não forçar extremos; 10–15 repetições por articulação; bilateralmente.

---

### 5.3 Cinesioterapia — Fase 1

#### Exercício Resistido de Baixa Carga com Alto Volume — Adaptação Neuromuscular

Nível de Evidência: A (CEBM Nível 1)
Referência primária: Borde R et al. Eur Rev Aging Phys Act 2015; PMC4849457 — revisão sistemática de RT em idosos sarcopênicos.
Alinhamento: ACSM 2019; EWGSOP2 — resistência é a intervenção primária para sarcopenia.

**Tabela de Dosagem — Fase 1 (Adaptação)**

| Parâmetro | Robusto — Valor Rec. | Robusto — Faixa Aceitável | Pré-frágil — Valor Rec. | Pré-frágil — Faixa Aceitável | Frágil — Valor Rec. | Frágil — Faixa Aceitável |
|-----------|---------------------|--------------------------|------------------------|------------------------------|--------------------|-----------------------|
| Carga inicial | 40% 1RM | 30–50% 1RM | 30% 1RM | 20–40% 1RM | 20% 1RM | 10–30% 1RM |
| Séries | 2–3 | 1–3 | 2 | 1–2 | 1–2 | 1–2 |
| Repetições | 12–15 | 10–20 | 10–15 | 8–15 | 8–12 | 6–12 |
| Frequência | 3×/semana | 2–3×/semana | 2–3×/semana | 2×/semana | 2×/semana | 1–2×/semana |
| Progressão | +5% quando RPE < 12 por 2 sessões | — | +2,5–5% quando RPE < 13 | — | +2,5% quando RPE ≤ 12 | — |
| Duração da sessão | 30–40 min | 25–45 min | 25–35 min | 20–40 min | 20–30 min | 15–30 min |

*Nota Sarcopenia Grave em Frágil: Reduzir a carga inicial em 20% adicional. Ex.: se faixa Frágil indica 20% 1RM, iniciar em 16% 1RM. Aumentar frequência de supervisão para cada sessão.*

**Grupos musculares prioritários em Fase 1:** Quadríceps, glúteos, extensores de tronco, flexores plantares — priorizando a funcionalidade de transferência e marcha.

**Exercícios recomendados Fase 1:**
- Levantar-sentar da cadeira (cadeira com braços para apoio se necessário) — simula a tarefa funcional mais relevante
- Extensão de joelho sentado com resistência mínima (haltere leve ou faixa elástica leve)
- Abdução de quadril em decúbito lateral (sem carga ou com faixa elástica leve)
- Elevação de calcanhar em pé (com apoio bilateral)
- Mini-agachamento funcional com apoio (até 30° de flexão de joelho)

#### Treinamento de Equilíbrio — Fase 1

Nível de Evidência: A (CEBM Nível 1)
Referência primária: Sherrington C et al. Cochrane Database Syst Rev 2019 — prevenção de quedas em idosos.
Alinhamento: EWGSOP2 — equilíbrio é componente do desempenho físico; deteriorado em sarcopenia.

**Tabela de Dosagem — Equilíbrio Fase 1**

| Parâmetro | Robusto — Valor Rec. | Pré-frágil — Valor Rec. | Frágil — Valor Rec. |
|-----------|---------------------|------------------------|---------------------|
| Suporte | Bipodal com olhos abertos | Bipodal semitândem com apoio | Bipodal com apoio sólido |
| Duração por posição | 30 seg | 20 seg | 10–15 seg |
| Séries | 3 | 2–3 | 2 |
| Frequência | 3×/semana | 2–3×/semana | 2–3×/semana |

---

## 6. Fase 2 — Fortalecimento Progressivo

### 6.1 Modalidade Terapêutica — Fase 2

#### Hidroterapia (opção adjuvante)

Nível de Evidência: B (CEBM Nível 2-3)
Referência primária: Martínez-Carbonell Guillamón E et al. J Aging Phys Act 2019 — revisão sistemática aquática em idosos.
Alinhamento: Indicada quando há limitação ortopédica concomitante (OA, ATJ, ATQ) que restrinja exercício em solo.

Aplicação: Exercícios resistidos em piscina aquecida (28–32°C); resistência da água substitui pesos; extensão e flexão de membros inferiores; caminhada aquática; 30–45 min por sessão. Não substitui exercício resistido progressivo em terra quando este é tolerado.

---

### 6.2 Terapia Manual — Fase 2

**Técnicas de energia muscular e mobilização segmentar (se restrição articular presente):**
Nível de Evidência: C (CEBM Nível 4-5)
Referência primária: Prática clínica — adjuvante para manutenção de amplitude funcional.

Aplicação: Indicado quando rigidez articular limita a amplitude necessária para os exercícios da fase; não é intervenção primária em sarcopenia.

---

### 6.3 Cinesioterapia — Fase 2: Tabela de Dosagem de Exercício Resistido (MODIFICADOR TRANSVERSAL)

> **MODIFICADOR TRANSVERSAL — DOSAGEM DE EXERCÍCIO RESISTIDO**
> Esta tabela é a referência normativa de dosagem de resistência para todos os 20
> protocolos de reabilitação geriátrica desta série (P-01 a P-20). Qualquer protocolo
> que aborde exercício resistido em paciente com sarcopenia confirmada deve citar:
> *"Ajustar dosagem conforme P-08 — Tabela de Dosagem de Resistência Estratificada
> por Fragilidade (Seção 6.3)."*
> Protocolos que detectam sarcopenia durante avaliação inicial devem encaminhar
> clinicamente a P-08 como protocolo principal ou co-tratamento.

#### Exercício Resistido Progressivo — Intervenção Principal

Nível de Evidência: A (CEBM Nível 1)
Referência primária: Repositório meta-analítico — PMC12602684 (Aging Clin Exp Res 2025, 24 ECRs, 951 participantes); PMC12288929 (nutrição + exercício em sarcopenia); EWGSOP2 (Cruz-Jentoft AJ 2019, PubMed 30312372).
Estratificação de fragilidade: Fenótipo de Fried (2001) — herdado de SHARED-FOUNDATION.md.
Alinhamento: EWGSOP2 — exercício resistido é a intervenção com maior resposta em sarcopenia; ACSM 2019.

### Tabela de Dosagem de Exercício Resistido — Modificador Transversal (P-08)

*Fonte: Meta-análise Aging Clin Exp Res 2025 (Springer, doi 10.1007/s40520-025-03235-w); PMC12288929; EWGSOP2 (Cruz-Jentoft AJ 2019). Estratificação de fragilidade: Fried (2001).*

| Parâmetro | Robusto — Valor Rec. | Robusto — Faixa Aceitável | Pré-frágil — Valor Rec. | Pré-frágil — Faixa Aceitável | Frágil — Valor Rec. | Frágil — Faixa Aceitável |
|-----------|---------------------|--------------------------|------------------------|------------------------------|--------------------|-----------------------|
| Carga inicial | 65% 1RM | 50–75% 1RM | 50% 1RM | 40–65% 1RM | 35% 1RM | 25–50% 1RM |
| Séries | 3 | 2–4 | 2–3 | 1–3 | 2 | 1–3 |
| Repetições | 8–12 | 6–15 | 8–12 | 6–12 | 6–10 | 5–12 |
| Frequência | 3×/semana | 2–4×/semana | 2–3×/semana | 2–3×/semana | 2×/semana | 1–3×/semana |
| Duração mínima | 12 semanas | — | 12 semanas | — | 12 semanas | — |
| Sessão | 50–60 min | 40–60 min | 45–55 min | 30–55 min | 30–45 min | 20–45 min |
| Progressão | +5% quando RPE < 12 | — | +2,5–5% quando RPE < 13 | — | +2,5% quando RPE ≤ 12 | — |

> **Nota Sarcopenia Grave (EWGSOP2):** Paciente Frágil com sarcopenia grave (velocidade de marcha < 0,8 m/s ou SPPB ≤ 8 ou TUG > 20 seg) → iniciar na faixa Frágil com redução adicional de 20% na carga inicial. Aumentar frequência de supervisão (presença do fisioterapeuta em cada sessão das primeiras 4 semanas). Ex.: faixa Frágil indica 35% 1RM → iniciar com 28% 1RM.

> **Nota sobre Betabloqueadores:** Em pacientes em uso de betabloqueadores, a frequência cardíaca não é indicador confiável de intensidade. Usar exclusivamente RPE (Borg 6-20) como parâmetro de intensidade.

> **Nota de Estratificação:** A tabela usa o Fenótipo de Fried (Robusto/Pré-frágil/Frágil) como estratificador — não o grau de sarcopenia EWGSOP2 (Provável/Confirmada/Grave). A gravidade da sarcopenia fornece contexto clínico adicional dentro de cada faixa de fragilidade. Um paciente Robusto com sarcopenia Grave inicia na faixa Robusto (não na faixa Frágil), mas com a nota de redução de 20% quando sarcopenia Grave está presente.

**Grupos musculares e exercícios recomendados — Fase 2:**
- Leg press bilateral e unilateral (carga progressiva)
- Extensão de joelho em cadeira extensora
- Flexão de joelho em cadeira flexora
- Agachamento com barra / peso corporal progressivo
- Supino ou Press de ombros (membros superiores — função integral)
- Remada sentada (extensores dorsais)
- Plantar-flexão com carga unilateral (panturrilha — força essencial para marcha)

**Critério de estimativa de 1RM (quando teste direto não é recomendado):**
Utilizar tabela de conversão reps-to-1RM ou fórmula de Brzycki (Brzycki M. Strength Cond J 1993):
1RM estimado = Carga (kg) / [1,0278 − (0,0278 × Nº repetições)]
Utilizar 8–12 repetições para estimativa mais confiável.

#### Treino Aeróbico — Componente Adjuvante Multicomponente (Fase 2)

Nível de Evidência: A (CEBM Nível 1)
Referência primária: Liao C-D et al. J Clin Med 2019 — meta-análise multicomponente para sarcopenia.
Alinhamento: EWGSOP2 recomenda abordagem multicomponente; ACSM 2019.

**Tabela de Dosagem — Aeróbico Fase 2**

| Parâmetro | Robusto — Valor Rec. | Pré-frágil — Valor Rec. | Frágil — Valor Rec. |
|-----------|---------------------|------------------------|---------------------|
| Modalidade | Caminhada rápida / bicicleta ergométrica / esteira | Caminhada em piso plano / bicicleta estacionária | Caminhada supervisionada / ergômetro de braço |
| Intensidade (RPE Borg) | 13–14 | 12–13 | 11–12 |
| Duração por sessão | 20–30 min | 15–25 min | 10–20 min |
| Frequência | 3×/semana | 2–3×/semana | 2×/semana |

> **Integração com resistência:** Sessões multicomponente — realizar exercício resistido ANTES do aeróbico (prioridade ao recrutamento de fibras de alto limiar quando não fatigadas).

#### Treinamento de Equilíbrio — Fase 2

Nível de Evidência: A (CEBM Nível 1)
Referência primária: Sherrington C et al. Cochrane 2019.

| Parâmetro | Robusto — Valor Rec. | Pré-frágil — Valor Rec. | Frágil — Valor Rec. |
|-----------|---------------------|------------------------|---------------------|
| Suporte | Unipodal / olhos fechados | Semitândem / superfície instável leve | Bipodal com apoio / tândem |
| Duração por posição | 30 seg | 20–30 seg | 15–20 seg |
| Séries | 3 | 2–3 | 2–3 |
| Frequência | 3×/semana | 2–3×/semana | 2–3×/semana |

---

## 7. Fase 3 — Manutenção Funcional

### 7.1 Modalidade Terapêutica — Fase 3

**Orientação para programas comunitários de exercício:**
Nível de Evidência: B (CEBM Nível 2-3)
Referência primária: Sherrington C et al. Cochrane 2019 — programas comunitários de exercício para prevenção de quedas.
Alinhamento: EWGSOP2 — manutenção a longo prazo é essencial; sarcopenia recidiva sem atividade contínua.

Orientar paciente para: academia / CRAS / UBS com programa de exercício supervisionado; Tai Chi Chuan para equilíbrio; ioga adaptado; natação / hidroginástica.

---

### 7.2 Terapia Manual — Fase 3

Terapia manual não é intervenção prioritária na Fase 3. Uso pontual para manutenção de amplitude articular se rigidez se instalar durante o programa de manutenção.

---

### 7.3 Cinesioterapia — Fase 3: Manutenção Multicomponente

Nível de Evidência: A (CEBM Nível 1)
Referência primária: PMC12602684 — manutenção após 12 semanas de RT; PMC12288929.

**Tabela de Dosagem — Manutenção (Fase 3)**

| Parâmetro | Robusto — Valor Rec. | Pré-frágil — Valor Rec. | Frágil — Valor Rec. |
|-----------|---------------------|------------------------|---------------------|
| Carga resistida | 60–70% 1RM | 50–65% 1RM | 35–50% 1RM |
| Séries | 2–3 | 2–3 | 2 |
| Repetições | 8–12 | 8–12 | 8–10 |
| Frequência resistida | 2×/semana | 2×/semana | 1–2×/semana |
| Frequência aeróbica | 3×/semana | 2–3×/semana | 2×/semana |
| Duração mínima (supervisão) | Transição após 4 sem de metas mantidas | Transição após 8 sem de metas mantidas | Supervisão continuada recomendada |

> **Regra de Manutenção:** A carga de manutenção (60–70% 1RM) mantém os ganhos adquiridos na Fase 2. Reduzir frequência (2×/semana) sem reduzir carga é a estratégia mais eficaz para manutenção a longo prazo. Fonte: ACSM 2019.

**Programa Domiciliar de Exercício (HEP — Home Exercise Program):**
- Exercícios com faixa elástica (resistência equivalente à Fase 2 ao nível de fragilidade)
- Caminhada diária de 20–30 min
- Exercícios de equilíbrio: tândem / unipodal (nível de fragilidade)
- Fichas visuais com fotografias / pictogramas — adaptar à escolaridade e cognição do paciente
- Reavaliar HEP a cada 30 dias nas primeiras 3 reavaliações

---

## 8. Monitoramento de Dor

### 8.1 Limiares NRS por Fase

*Base: Prática clínica estabelecida em RCTs de exercício para reabilitação geriátrica; alinhado com recursos educacionais IASP sobre dor em idosos.*

| Fase | Limiar de Interrupção Imediata | Limiar de Modificação | Dor Aceitável Durante Exercício |
|------|-------------------------------|----------------------|---------------------------------|
| Fase 1 (Adaptação) | NRS ≥ 5 | NRS 3–4 → reduzir carga 25% | NRS ≤ 3 (leve, esperada) |
| Fase 2 (Fortalecimento) | NRS ≥ 6 | NRS 4–5 → reduzir carga 20% | NRS ≤ 4 |
| Fase 3 (Manutenção) | NRS ≥ 7 | NRS 5–6 → reduzir carga 15% | NRS ≤ 5 |

**Regra Pós-Exercício:**
> Dor muscular pós-exercício que excede a dor pré-exercício em mais de 2 pontos na NRS e persiste por mais de 24 horas = sobrecarga. Reduzir volume na sessão seguinte.

### 8.2 Diferenciação: Dor Muscular de Início Tardio (DMIT/DOMS) vs. Dor Patológica

| Característica | DMIT (Esperada) | Dor Patológica (Investigar) |
|---------------|-----------------|----------------------------|
| Início | 12–72h pós-exercício | Durante ou imediatamente após |
| Localização | Difusa, no músculo exercitado | Localizada, articular, óssea |
| Qualidade | Peso, sensibilidade ao toque | Aguda, em facada, lancinante |
| Resolução | 72h sem intervenção | Persistente > 72h sem melhora |
| Intensidade | Leve a moderada (NRS ≤ 4) | Qualquer intensidade NRS ≥ 5 |
| Ação | Continuar exercício; reduzir carga 10% se NRS ≥ 3 | Suspender; investigar; encaminhar |

> **Atenção ao Idoso com Sarcopenia:** Limiares de dor podem estar alterados em idosos frágeis com comprometimento cognitivo. Observar sinais comportamentais: recusa do exercício, expressão facial de desconforto, proteção do segmento. Usar Pain Assessment in Advanced Dementia Scale (PAINAD) se MoCA-BR < 18.

---

## 9. Bandeiras Vermelhas e Escalonamento

### 9.1 Tabela de Bandeiras Vermelhas — Gerais e Específicas para Sarcopenia

| Sinal / Sintoma | Ação Imediata | Destino de Encaminhamento |
|-----------------|---------------|--------------------------|
| **Dor articular aguda de novo, sem trauma identificado** | Suspender sessão | Reumatologista |
| **Inchaço articular súbito com calor e eritema** | Suspender sessão | Reumatologista / urgência |
| **Febre associada a dor muscular ou articular (> 37,8°C)** | Suspender sessão | Clínico / urgência |
| **Dor irradiada com déficit neurológico novo (fraqueza súbita, parestesia)** | Suspender sessão | Neurocirurgia / urgência |
| **Dor em repouso noturna progressiva (suspeita oncológica)** | Não iniciar exercício | Oncologista / clínico |
| **Dispneia súbita e desproporcional ao esforço** | Suspender sessão | Cardiologista / urgência |
| **Hipotensão ortostática sintomática (queda PA sistólica > 20 mmHg)** | Suspender sessão | Clínico |
| **Dor torácica, pressão precordial ou irradiação para braço/mandíbula** | Suspender — acionar emergência | SAMU 192 / urgência cardiológica |
| **Palpitações com tontura ou síncope** | Suspender sessão | Cardiologista / urgência |
| **Saturação O₂ < 90% durante exercício** | Suspender sessão | Cardiologista / pneumologista |
| **Confusão mental aguda ou desorientação súbita** | Suspender sessão | Neurologia / urgência |
| **Perda de peso involuntária rápida (≥ 2 kg em 2 semanas) durante o protocolo** | Suspender intensificação; investigar | Clínico / Nutricionista (urgência alta) |
| **Queda durante sessão de exercício** | Interromper exercício; avaliar lesão | Urgência se suspeita de fratura; registrar ocorrência |
| **Dor muscular aguda intensa durante exercício (suspeita de rabdomiólise)** | Suspender exercício imediatamente | Urgência — solicitar CK sérica |
| **Fraqueza muscular súbita unilateral nova (crise hipocalêmica em uso de diuréticos)** | Suspender exercício | Clínico / urgência — eletrólitos |

### 9.2 Critérios de Pausa Temporária do Protocolo (não descontinuação)

| Situação | Duração da Pausa | Retorno |
|----------|-----------------|---------|
| Doença aguda intercorrente (infecção, gripe) | Até resolução + 48h afebril | Retomar na Fase 1 se pausa > 2 semanas |
| Procedimento cirúrgico eletivo (não ortopédico) | Conforme clearance médico | Retomar 1 fase abaixo da última completada |
| Hospitalização | Conforme liberação médica | Reavaliação completa antes de retomar |

---

## 10. Interações com Polifarmácia

### 10.1 Classes Farmacológicas da SHARED-FOUNDATION (Base Herdada)

*Referência: SHARED-FOUNDATION.md Seção 7.3 — Polifarmácia. Base: Lancet Healthy Longevity 2025; AGS Beers Criteria 2023 (PubMed 37139824)*

| Classe Farmacológica | Implicação para o Exercício | Modificação Prescritiva |
|---------------------|----------------------------|------------------------|
| **AINEs** (AAS, ibuprofeno, naproxeno, diclofenaco) | Mascaramento da dor → risco de sobrecarga; risco cardiovascular e renal | Reforçar monitoramento NRS; evitar alta intensidade sem supervisão |
| **Corticosteroides** (uso crônico > 3 meses) | Miopatia corticoesteroide, perda óssea → fragilidade muscular | Reduzir cargas de impacto; priorizar fortalecimento de baixa carga; considerar densitometria |
| **Betabloqueadores** (propranolol, atenolol, metoprolol) | FC embotada — frequência cardíaca não confiável como indicador de intensidade | Usar exclusivamente RPE (Borg 6-20) como indicador; nunca usar % FC máx como parâmetro |
| **Vasodilatadores e diuréticos tiazídicos** (anlodipino, hidroclorotiazida) | Risco de hipotensão ortostática pós-exercício | Resfriamento obrigatório ≥ 10 min; monitorar PA pré e pós-sessão; hidratação adequada |
| **Anticoagulantes** (varfarina, rivaroxabana, apixabana) | Risco aumentado de sangramento em contusões | Evitar exercícios de contato; monitorar equimoses; comunicar equipe médica após qualquer queda |
| **Benzodiazepínicos e sedativos** (diazepam, clonazepam, zolpidem) | Sonolência residual, risco de queda aumentado | Agendar sessões longe do pico de ação; enfatizar supervisão de equilíbrio e marcha |

---

### 10.2 Extensão para Sarcopenia — Classes Adicionais (além da base SHARED-FOUNDATION)

*Referência: Kuzuya M et al. Drug-related sarcopenia. PMC11503558 (2024); Cruz-Jentoft AJ EWGSOP2 2019.*

| Classe Farmacológica | Mecanismo de Risco em Sarcopenia | Implicação Prescritiva |
|---------------------|----------------------------------|------------------------|
| **Estatinas** (sinvastatina > 40 mg/dia, atorvastatina, rosuvastatina) | Miotoxicidade direta; inibição de coenzima Q10; associação causal confirmada com sarcopenia por análise de randomização mendeliana | Monitorar CK se fadiga muscular incomum ou dor muscular inexplicada; comunicar clínico/cardiologista; avaliar com SARC-F após início de estatina; não suspender sem orientação médica |
| **Inibidores de aromatase** (anastrozol, letrozol — mulheres pós-menopausa com Ca de mama) | Perda de massa muscular e óssea acelerada; interação sinérgica com sarcopenia e osteoporose | Combinar P-08 (resistência muscular) + P-04 (osso); aumentar frequência de avaliação de força; coordenar com oncologia |
| **Diuréticos de alça** (furosemida, bumetanida) | Hipocalemia → fraqueza muscular; hipomagnesemia secundária; potencializa perda muscular | Monitorar eletrólitos antes de intensificar exercício; sessões mais curtas na fase de ajuste de dose; consultar clínico se fraqueza súbita |
| **Corticosteroides crônicos** (> 3 meses — além do item base) | Miopatia corticoesteroide: atrofia preferencial de fibras tipo II (exatamente as recrutadas no exercício resistido de alta carga); perda óssea acelerada (conecta com P-04) | Carga de impacto reduzida; fortalecimento de baixa carga prioritário; densitometria antes de aumentar carga; comunicar ortopedista; progressão mais lenta (+2,5% a cada 3 semanas vs. padrão) |
| **Antidepressivos ISRS** (fluoxetina, sertralina, paroxetina) | Associados a perda de massa muscular em uso crônico; risco de hiponatremia (síndrome da secreção inapropriada de ADH) | Monitorar função muscular (SARC-F repetido em uso > 6 meses); vigilância de sinais de hiponatremia (confusão, fraqueza, náusea); comunicar clínico |

> **Total de classes cobertas: 11** (6 base SHARED-FOUNDATION + 5 específicas de sarcopenia) — cumprindo requisito de ≥ 9 classes.

---

### 10.3 Coordenação Proteína-Exercício e Via de Encaminhamento Nutricional

*Nível de Evidência: A (CEBM Nível 1) — PMC12288929; PROT-AGE Study Group (PubMed 23867520)*

**Alvo de ingestão proteica:** ≥ 1,2 g/kg de peso corporal/dia para idosos em exercício resistido ativo. Meta de 1,5 g/kg/dia em sarcopenia grave confirmada (EWGSOP2).

**Timing pós-exercício:** Ingestão de 20–25 g de proteína de alto valor biológico (proteína do soro do leite / proteína animal de alta qualidade) nas 2 horas após cada sessão de exercício resistido maximiza a síntese proteica muscular pós-exercício.

**Vitamina D:** Alvo sérico 25-OH-D: 50–75 nmol/L. Suplementação 800–2.000 UI/dia em pacientes com níveis abaixo do alvo — confirmar com equipe médica. Nota: fisioterapeuta identifica deficiência suspeita e encaminha; não prescreve suplemento.

**Via de Encaminhamento ao Nutricionista — Critérios de Acionamento:**

| Critério | Prioridade | Ação |
|----------|-----------|------|
| Ingestão proteica autorrelatada < 1,0 g/kg/dia | Moderada | Encaminhar ao nutricionista |
| IMC < 22 kg/m² | Moderada | Encaminhar ao nutricionista |
| Sarcopenia Grave confirmada (EWGSOP2) | Alta | Encaminhar ao nutricionista |
| Perda de peso involuntária ≥ 4,5 kg em 12 meses | Alta | Encaminhar ao nutricionista + clínico |
| Incapacidade de preparar ou ingerir refeições adequadas (AVDs) | Alta | Encaminhar ao nutricionista + assistente social |

> **Nota de Escopo Profissional:** A prescrição dietética (tipo, quantidade e fonte de proteína) é responsabilidade exclusiva do nutricionista. O fisioterapeuta registra os critérios de encaminhamento na evolução clínica e comunica à equipe multidisciplinar. **Não prescrever dieta — apenas identificar, registrar e encaminhar.**

---

## 11. Precauções Cardiorrespiratórias

### 11.1 Avaliação Pré-Participação

Todo paciente idoso deve ter avaliação cardiovascular documentada antes de iniciar exercício de intensidade moderada a intensa. Verificar e registrar:
- PA basal (repouso sentado, após 5 minutos)
- FC de repouso
- História de ICC, DPOC, arritmias, angina, infarto prévio
- Saturação O₂ basal (se disponível — especialmente em suspeita de DPOC)
- Medicamentos cardiovasculares em uso (ver Seção 10.1)

> **Atenção Especial em Sarcopenia:** O monitoramento de RPE é particularmente importante em pacientes com sarcopenia em uso de betabloqueadores. A FC não reflete adequadamente a intensidade do esforço — usar Borg 6-20 exclusivamente.

### 11.2 Indicadores de Parada Imediata

| Indicador | Limiar |
|-----------|--------|
| Dor torácica, pressão precordial ou irradiação | Qualquer ocorrência |
| Dispneia súbita e desproporcional ao esforço | Qualquer ocorrência |
| Palpitações com tontura ou síncope | Qualquer ocorrência |
| PA sistólica durante exercício | > 200 mmHg |
| Queda de PA sistólica durante esforço progressivo | > 10 mmHg |
| Saturação O₂ (se oximetria disponível) | SpO₂ < 90% |
| Fadiga muscular extrema súbita (suspeita de rabdomiólise) | Qualquer ocorrência + dor muscular NRS ≥ 7 |

### 11.3 Adaptações para Pacientes com ICC ou DPOC Conhecida

- Iniciar na faixa **Frágil** independentemente do escore de fragilidade obtido
- Sessões mais curtas: 15–20 minutos, com maior frequência semanal (3–5×/semana se tolerado)
- RPE ≤ 13 (Borg 6-20) como limite superior de esforço
- Sessões supervisionadas obrigatórias nas primeiras 4 semanas
- Oximetria de pulso durante exercício se disponível

### 11.4 Considerações Específicas: Sarcopenia + Comorbidades Cardiorrespiratórias

A sarcopenia coexiste frequentemente com ICC e DPOC (síndrome do déficit muscular global). O protocolo deve ser interpretado à luz de P-15 (DPOC) e P-16 (IC) quando essas comorbidades estiverem presentes:

- **Sarcopenia + DPOC:** Exercício resistido é fortemente indicado (maior nível de evidência que em DPOC isolada). RPE ≤ 13 como teto. Broncodilatador de ação curta disponível na sessão.
- **Sarcopenia + ICC:** Exercício resistido de moderada intensidade é seguro e indicado. Monitorar PA e FC (mesmo com betabloqueador). Sessões mais curtas com períodos de repouso intercalados.

---

## 12. Indicadores de Desfecho

### 12.1 Desfechos Primários

| Desfecho | Instrumento | MCID | Frequência de Avaliação |
|----------|-------------|------|------------------------|
| **Força muscular** | Dinamometria Manual (Jamar) | H: 5,0–6,5 kg; F: 2,7–5,0 kg | Pré-tratamento; a cada 6 semanas; pós-tratamento |
| **Desempenho físico** | SPPB-BR (0–12 pontos) | 0,5–1,0 pontos | Pré-tratamento; a cada 6 semanas; pós-tratamento |
| **Velocidade de marcha** | Marcha em 4m (m/s) | 0,1 m/s | Pré-tratamento; a cada 6 semanas; pós-tratamento |
| **Mobilidade funcional** | TUG (segundos) | 2,0–3,0 seg | Pré-tratamento; a cada 6 semanas; pós-tratamento |

### 12.2 Desfechos Secundários

| Desfecho | Instrumento | Frequência |
|----------|-------------|------------|
| Rastreio de sarcopenia | SARC-F (0–10) | Início e a cada 12 semanas |
| Cognição | MoCA-BR (0–30) | Início e anualmente |
| Massa muscular (se disponível) | DEXA ou BIA — ASM/h² | Início e anualmente (se disponível) |
| Qualidade de vida | EuroQol EQ-5D-5L ou SF-36 | Início e a cada 12 semanas |

### 12.3 Metas Funcionais Definidoras de Sucesso

| Meta | Critério Objetivo |
|------|------------------|
| Saída da categoria "sarcopenia grave" | Velocidade de marcha > 0,8 m/s E SPPB-BR > 8 pontos |
| Saída da categoria "sarcopenia" | Força de preensão ≥ 27 kg (M) ou ≥ 16 kg (F) |
| Risco de queda reduzido | TUG < 13,5 seg |
| Desempenho físico preservado | SPPB-BR ≥ 10 pontos |

### 12.4 Cronograma de Reavaliação

| Avaliação | Momento |
|----------|---------|
| Avaliação inicial completa (bateria + Fried + SARC-F) | Antes da 1ª sessão |
| Reavaliação de transição (entrada Fase 2) | Semana 4–8 (quando critérios de saída Fase 1 atingidos) |
| Reavaliação de transição (entrada Fase 3) | Semana 12–16 (quando critérios de saída Fase 2 atingidos) |
| Reavaliação de manutenção | A cada 6 semanas durante Fase 3 |
| Reavaliação anual | 12 meses após alta do protocolo supervisionado |

---

## 13. Rastreabilidade e Flags de Comorbidade

### 13.1 Interações Clínicas Conhecidas com Outros Protocolos

| Protocolo Relacionado | Condição | Natureza da Interação | Instrução Clínica |
|----------------------|----------|----------------------|-------------------|
| **P-04 — Osteoporose** | T-score ≤ -2,5 coexistindo com sarcopenia | Osteosarcopenia — condição de muito alto risco | Aplicar restrições de carga óssea P-04 + dosagem resistida P-08; ver P-04 Seção [Modificador Transversal] |
| **P-01 — Osteoartrite** | OA de joelho ou quadril + sarcopenia | Fraqueza muscular potencializa carga articular | Priorizar fortalecimento de quadríceps e glúteos per P-08; respeitar NRS de P-01 durante exercício de cadeia fechada |
| **P-05 — Fratura de Fêmur** | Pós-operatório tardio + sarcopenia pré-existente | Sarcopenia retarda reabilitação pós-fratura | Iniciar P-08 após clearance ortopédico; coordenar progressão com P-05 |
| **P-07 — Quedas** | Síndrome pós-queda + sarcopenia | Sarcopenia é o principal fator de risco muscular para quedas | P-07 encaminha para P-08 como protocolo de fortalecimento; equilíbrio integrado em P-08 Fases 1 e 2 |
| **P-10 — Artroplastia Total de Joelho** | Pós-ATJ + sarcopenia | Sarcopenia prolonga recuperação funcional pós-ATJ | Coordenar: P-10 para protocolo pós-cirúrgico; P-08 para dosagem de resistência após clearance cirúrgico |
| **P-11 — Artroplastia Total de Quadril** | Pós-ATQ + sarcopenia | Sarcopenia prolonga recuperação funcional pós-ATQ | Coordenar: P-11 para protocolo pós-cirúrgico; P-08 para dosagem de resistência após clearance cirúrgico |

### 13.2 Flags de Comorbidade para Prontuário

Ao incluir paciente neste protocolo, registrar no prontuário:

```
[P-08-FLAG] Sarcopenia: [Provável | Confirmada | Grave] — EWGSOP2 FACS
Força de preensão: ___ kg (M/F); Limiar EWGSOP2: < 27 kg / < 16 kg
ASM/h²: ___ kg/m² (se DEXA/BIA disponível)
Velocidade de marcha: ___ m/s; TUG: ___ seg; SPPB-BR: ___ pontos
Fragilidade (Fried): [Robusto | Pré-frágil | Frágil] — ___ critérios
Comorbidades com interação P-08: [P-04 / P-01 / P-05 / P-07 / P-10 / P-11]
Encaminhamento nutricional acionado: [Sim / Não] — critério: ___
```

---

## 14. Referências por Nível de Evidência

### 14.1 Nível A — Revisões Sistemáticas e ECRs de Alta Qualidade (CEBM Nível 1)

1. **Cruz-Jentoft AJ et al.** Sarcopenia: revised European consensus on definition and diagnosis. Age Ageing 2019;48(1):16-31. **PubMed 30312372** — EWGSOP2: diagnóstico, algoritmo FACS, critérios operacionais.

2. **PMC12602684** — Revisão sistemática (Aging Clin Exp Res 2025): parâmetros ótimos de exercício resistido para sarcopenia; 24 ECRs, 951 participantes; 3×/semana, 50–70% 1RM, ≥ 12 semanas como padrão.

3. **PMC12288929** — Revisão nutrição e exercício em sarcopenia (2025): sinergismo proteína + treinamento resistido; proteína 1,5 g/kg/dia em sarcopenia ativa; vitamina D como adjuvante.

4. **Sherrington C et al.** Exercise for preventing falls in older people living in the community. Cochrane Database Syst Rev 2019. — Treinamento de equilíbrio para prevenção de quedas em sarcopenia.

5. **PROT-AGE Study Group** — Bauer J et al. Evidence-based recommendations for optimal dietary protein intake in older people. J Am Med Dir Assoc 2013. **PubMed 23867520** — Proteína ≥ 1,2 g/kg/dia para idosos ativos; base para encaminhamento nutricional.

6. **Liao C-D et al.** Effects of protein supplementation combined with resistance exercise on body composition and physical function. Nutrients 2019. — Meta-análise multicomponente (resistência + nutrição) em sarcopenia; evidência para abordagem integrada.

### 14.2 Nível B — Estudos Controlados e Revisões de Menor Nível (CEBM Nível 2-3)

7. **Kirk B et al.** Towards a global definition of sarcopenia: GLIS conceptual consensus. Age Ageing 2024. **PMC11210221** — Definição conceitual global; critérios operacionais NOT publicados; uso contextual apenas neste protocolo.

8. **Kuzuya M et al.** Drug-related sarcopenia: mechanisms and management. PMC11503558 (2024). — Estatinas, corticosteroides, antidepressivos ISRS como medicamentos causalmente associados a sarcopenia.

9. **Borde R, Hortobágyi T, Granacher U.** Dose–response relationships of resistance training in healthy old adults. Eur Rev Aging Phys Act 2015. **PMC4849457** — Resposta dose-efeito do treinamento resistido em idosos; base para dosagem Fase 1.

10. **Morley JE et al.** A simple frailty questionnaire (SARC-F) predicts outcomes in middle aged African Americans. J Nutr Health Aging 2012. — Validação do SARC-F como instrumento de rastreio para sarcopenia.

11. **Paillard T.** Neuromuscular electrical stimulation (NMES) and resistance training in the management of sarcopenia. Ann Phys Rehabil Med 2022. — NMES como adjuvante em sarcopenia; evidência de nível B.

### 14.3 Nível C — Consenso Especializado e Séries de Casos (CEBM Nível 4-5)

12. **Memoria CM et al.** Brief screening for mild cognitive impairment: validation of the Brazilian version of the Montreal Cognitive Assessment. Int Psychogeriatr 2013. **PubMed 22368034** — Validação brasileira do MoCA-BR.

13. **Nakano MM.** Versão brasileira da Short Physical Performance Battery (SPPB). 2007. — Validação SPPB-BR; ICC = 0,83.

14. **Ibrahim A et al.** Reference values of the timed up and go test in healthy adults. PLoS One 2017. **PMC5626462** — Valores normativos do TUG por faixa etária.

15. **Dodds RM et al.** Grip strength across the life course: normative data from twelve British studies. PLoS One 2014. — Valores normativos de força de preensão por sexo e idade; base para limiares EWGSOP2.

16. **Fried LP et al.** Frailty in older adults: evidence for a phenotype. J Gerontol A Biol Sci Med Sci 2001;56(3):M146-56. — Fenótipo de Fried; sistema primário de classificação de fragilidade herdado de SHARED-FOUNDATION.

---

## 15. As 8 Questões de Validade Clínica

> **Finalidade:** Este checklist foi estabelecido em P-01 como template replicável para todos os 20 protocolos desta série. Um protocolo clinicamente válido deve responder às 8 questões com informação localizada e imediatamente aplicável.

---

### Q1: Quem qualifica para este protocolo?

**Resposta:** Idoso ≥ 60 anos com SARC-F ≥ 4 + força de preensão abaixo dos limiares EWGSOP2 (H < 27 kg; F < 16 kg) + capacidade de compreender a bateria de avaliação + consentimento informado. Exclusões: doença neuromuscular primária, caquexia oncológica ativa, condição cardíaca instável, comprometimento cognitivo grave sem cuidador, fratura aguda, infecção sistêmica ativa.

**Seção de referência:** Seção 1.3 (Inclusão) e Seção 1.4 (Exclusão)

---

### Q2: Quando parar ou suspender o tratamento?

**Resposta imediata (suspender a sessão):** NRS ≥ limiar da fase (5 em Fase 1, 6 em Fase 2, 7 em Fase 3); qualquer bandeira vermelha da Tabela 9.1 (dor torácica, dispneia súbita, palpitações com síncope, PA > 200 mmHg, SpO₂ < 90%, queda durante sessão, dor muscular aguda intensa suspeitando rabdomiólise).

**Pausa temporária:** Doença aguda intercorrente, procedimento cirúrgico, hospitalização — retomar após resolução conforme critérios da Tabela 9.2.

**Seção de referência:** Seção 8.1 (NRS) e Seção 9.1 (Bandeiras Vermelhas)

---

### Q3: Onde começar no protocolo (qual fase)?

**Resposta:** Todos os pacientes iniciam na Fase 1 (Adaptação), independentemente do grau de sarcopenia. O nível de fragilidade (Fenótipo de Fried) determina a linha da tabela de dosagem (Robusto / Pré-frágil / Frágil) — não a fase de entrada. Exceção: ICC ou DPOC conhecida → iniciar na faixa Frágil dentro da Fase 1, mesmo que Fenótipo de Fried classifique Robusto ou Pré-frágil.

**Seção de referência:** Seção 4.1 (Estrutura de Fases) e Seção 11.3 (ICC/DPOC)

---

### Q4: O que prescrever em cada fase?

**Fase 1:** Exercício resistido de baixa carga (20–40% 1RM; conforme fragilidade), mobilização miofascial, treinamento de equilíbrio básico, familiarização com exercício.

**Fase 2:** Exercício resistido progressivo (35–65% 1RM; conforme fragilidade) como intervenção PRINCIPAL; aeróbico adjuvante (RPE 11–14); equilíbrio avançado; abordagem multicomponente.

**Fase 3:** Manutenção (60–70% 1RM; 2×/semana); aeróbico regular; HEP domiciliar com fichas visuais; transição para programa comunitário.

**Em todas as fases:** Coordenação proteína-exercício (identificar e encaminhar ao nutricionista conforme critérios Seção 10.3).

**Seção de referência:** Seções 5, 6, e 7 (intervenções por fase)

---

### Q5: Quanto prescrever (dosagem)?

**Resposta:** Utilizar as tabelas de dosagem estratificadas por fragilidade em cada fase:
- Fase 1: Tabela Seção 5.3 (20–40% 1RM; 1–3 séries; 8–15 reps; 2–3×/semana)
- Fase 2: Tabela MODIFICADOR TRANSVERSAL Seção 6.3 (35–65% 1RM; 2–3 séries; 6–12 reps; 2–4×/semana — conforme fragilidade)
- Fase 3: Tabela Seção 7.3 (35–70% 1RM; 2–3 séries; 8–12 reps; 1–2×/semana para resistência)

**Nota Sarcopenia Grave + Frágil:** Reduzir carga inicial em 20% adicional em relação à faixa Frágil.

**Seção de referência:** Seção 6.3 (Tabela Modificador Transversal) e tabelas de cada fase

---

### Q6: Como progredir (velocidade de progressão)?

**Resposta:**
- **Robusto:** Progredir +5% de carga quando RPE (Borg 6-20) < 12 por 2 sessões consecutivas
- **Pré-frágil:** Progredir +2,5–5% quando RPE < 13 por 2 sessões consecutivas
- **Frágil:** Progredir +2,5% quando RPE ≤ 12 por 2 sessões consecutivas

**Progressão de fase:** Somente por critérios funcionais (Seção 4.1) — nunca por número de semanas.

**Anti-padrão:** Nunca progredir por calendário. Nunca manter mesma carga indefinidamente sem critério de reavaliação. Nunca avançar de fase sem atingir os critérios funcionais de saída.

**Seção de referência:** Seção 4.1 (critérios de transição) e tabelas de dosagem por fase

---

### Q7: Como medir o progresso?

**Resposta:** Reavaliar com bateria completa (TUG + SPPB-BR + Dinamometria Manual + Velocidade de marcha) a cada 6 semanas e a cada transição de fase. MCIDs:
- Força de preensão: H ≥ 5,0 kg; F ≥ 2,7 kg
- SPPB-BR: ≥ 0,5 pontos (pequena); ≥ 1,0 ponto (substancial)
- Velocidade de marcha: ≥ 0,1 m/s
- TUG: ≥ 2,0–3,0 seg de melhora

**Metas de saída de sarcopenia:** Força ≥ 27 kg (M) / ≥ 16 kg (F); velocidade marcha > 0,8 m/s; SPPB ≥ 9 pontos.

**Seção de referência:** Seção 12 (Indicadores de Desfecho) — Tabelas 12.1, 12.3 e 12.4

---

### Q8: Por que estas escolhas? (Justificativa das decisões clínicas)

**Resposta:**

| Escolha | Justificativa |
|---------|---------------|
| EWGSOP2 como padrão diagnóstico | Algoritmo FACS mais validado internacionalmente; GLIS 2024 é apenas conceitual sem cutoffs | PubMed 30312372 |
| SARC-F como gate de rastreio | Instrumento de 5 itens validado; sensível e rápido; primeiro passo do FACS | Morley 2012 |
| Fenótipo de Fried para estratificação de dosagem | Consistência com SHARED-FOUNDATION; todos os 20 protocolos usam a mesma estratificação; não usar gravidade EWGSOP2 para isso | SHARED-FOUNDATION Seção 2 |
| Exercício resistido como intervenção primária | Maior volume de evidência de nível A; 24 ECRs mostram ganho de força e massa; EWGSOP2 recomenda como tratamento | PMC12602684 |
| Abordagem multicomponente (resistência + aeróbico + equilíbrio) | Maior efeito que modalidade isolada em múltiplos desfechos | Liao C-D et al.; EWGSOP2 |
| Proteína ≥ 1,2 g/kg/dia com encaminhamento | Sinergismo proteína+exercício é Nível A; prescrição dietética está fora do escopo da fisioterapia | PROT-AGE; ESPEN 2018 |
| Duração mínima 12 semanas | Meta-análise 2025: duração < 12 sem não produz ganhos mensuráveis e clinicamente relevantes | PMC12602684 |
| Corticosteroides/Estatinas em seção específica | Associação causal com sarcopenia confirmada; fisioterapeuta deve monitorar e comunicar | PMC11503558 |

---

*Documento gerado em: 2026-03-13*
*Responsável pela elaboração: Especialista em Validação de Protocolos de Reabilitação Geriátrica*
*Baseado em: EWGSOP2 (2018), ESPEN 2018/2019, ACSM 2019, PROT-AGE 2013, Meta-análises 2024-2025*
*Próxima revisão recomendada: 2026-09-13; exceções: GLIS operational criteria (verificar mensalmente — publicação esperada)*
