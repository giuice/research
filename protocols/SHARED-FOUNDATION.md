# Camada de Fundação Compartilhada — Padrões Universais para Protocolos de Reabilitação Geriátrica

**Documento:** SHARED-FOUNDATION.md
**Versão:** 1.0
**Data:** 2026-03-12
**Domínio:** Fisioterapia Geriátrica com Prática Baseada em Evidências (PBE)
**Idioma:** Português Brasileiro
**Escopo:** Referência universal herdada por todos os 20 protocolos de reabilitação geriátrica (P-01 a P-20)

> **Nota:** Este documento é a âncora arquitetural. Nenhum protocolo individual deve redefinir os padrões aqui estabelecidos. Qualquer protocolo que divergir desta base deve justificar explicitamente a razão clínica da divergência.

---

## Índice

1. [Bateria Universal de Avaliação Inicial](#1-bateria-universal-de-avaliação-inicial)
2. [Sistema de Classificação de Fragilidade](#2-sistema-de-classificação-de-fragilidade)
3. [Princípio de Progressão](#3-princípio-de-progressão)
4. [Padrão de Graduação de Evidência (Oxford CEBM)](#4-padrão-de-graduação-de-evidência-oxford-cebm)
5. [Padrão de Formato de Dosagem](#5-padrão-de-formato-de-dosagem)
6. [Registro de Ferramentas de Desfecho em Português Brasileiro](#6-registro-de-ferramentas-de-desfecho-em-português-brasileiro)
7. [Arquitetura de Segurança (Templates)](#7-arquitetura-de-segurança-templates)
8. [Esqueleto do Índice de Referência Cruzada](#8-esqueleto-do-índice-de-referência-cruzada)

---

## 1. Bateria Universal de Avaliação Inicial

Todos os protocolos desta série exigem a aplicação desta bateria como avaliação inicial mandatória antes do início de qualquer intervenção. Os resultados norteiam a classificação de fragilidade (Seção 2) e a seleção da faixa de dosagem (Seção 5).

### 1.1 TUG — Timed Up and Go

**Descrição do Protocolo:**
O TUG avalia mobilidade funcional, marcha e risco de queda. O paciente parte da posição sentada em cadeira padrão (altura de assento ~46 cm), levanta-se sem uso dos braços (se possível), caminha 3 metros, vira, retorna e senta-se novamente. O tempo é cronometrado do comando "vai" até o retorno completo à posição sentada. Calçado habitual; pode usar dispositivo auxiliar de marcha se habitual — registrar qual.

**Equipamento:** Cronômetro, cadeira padrão sem apoio de braços (ou registrar se com braços), fita métrica, marcador de 3 metros no chão.

**Procedimento padronizado:**
1. Demonstrar o teste antes da execução
2. Permitir 1 ensaio de familiarização
3. Registrar a média de 2 tentativas (ou 3 se houver variação > 2 seg entre tentativas)
4. Registrar dispositivo auxiliar utilizado (se algum)

**Valores Normativos por Faixa Etária — Idosos da Comunidade:**

| Faixa Etária | Média (seg) | Desvio Padrão | Interpretação Clínica |
|-------------|-------------|--------------|----------------------|
| 60–64 anos | ~8,1 | — | Referência comunitária |
| 71–75 anos | 9,5 | ±2,5 | Referência comunitária |
| 76–80 anos | 9,9 | ±3,0 | Atenção se > 12 seg |
| 81–85 anos | 11,2 | ±3,6 | Atenção se > 13,5 seg |
| 86–99 anos | 12,0 | ±3,8 | Alto risco se > 13,5 seg |

*Fonte: Ibrahim A et al. PLoS One 2017; PMC5626462*

**Limiar de Risco de Queda:** > 13,5 segundos = risco aumentado de queda em idosos da comunidade.
*Fonte: Podsiadlo D, Richardson S. J Am Geriatr Soc 1991.*

**MCID (Diferença Mínima Clinicamente Importante):** 2,0–3,0 segundos (estimativa clínica baseada em prática estabelecida em RCTs de referência).

**Interpretação:**
- ≤ 10 seg: Mobilidade funcional preservada, risco de queda baixo
- 10–13,5 seg: Risco moderado — avaliar marcha e equilíbrio com SPPB
- > 13,5 seg: Risco aumentado — considerar programa de prevenção de quedas
- > 20 seg: Alta dependência para AVDs externas

---

### 1.2 SPPB-BR — Short Physical Performance Battery (Versão Brasileira)

**Descrição do Protocolo:**
O SPPB-BR avalia desempenho físico em três domínios: equilíbrio estático, velocidade de marcha e força de membros inferiores (levantar-sentar repetido). Cada domínio é pontuado de 0 a 4; total máximo = 12 pontos.

**Validação Brasileira:** Nakano MM (2007) — tradução e adaptação transcultural para o português brasileiro. Confiabilidade teste-reteste: ICC = 0,83.
*Verificar também: Brucki SMD et al. para validação de propriedades psicométricas adicionais.*

**Equipamento:** Cronômetro, cadeira com encosto e sem braços (altura ~46 cm), fita métrica (4 metros), espaço plano de pelo menos 5 metros.

**Subcomponentes:**

**1. Equilíbrio Estático (0–4 pontos):**
- Posição de pés paralelos por 10 seg = 1 ponto
- Posição semitândem por 10 seg = 1 ponto adicional
- Posição tândem por 10 seg = 2 pontos adicionais (total = 4)
- Falha em qualquer posição = pontuação da posição anterior

**2. Velocidade de Marcha em 4 metros (0–4 pontos):**
- > 4,82 seg = 1 ponto
- 3,82–4,82 seg = 2 pontos
- 2,60–3,81 seg = 3 pontos
- < 2,60 seg = 4 pontos

**3. Levantar-Sentar Repetido — 5 vezes (0–4 pontos):**
- Incapaz ou > 60 seg = 0 pontos
- 16,7–60 seg = 1 ponto
- 13,7–16,6 seg = 2 pontos
- 11,2–13,6 seg = 3 pontos
- < 11,2 seg = 4 pontos

**Valores Normativos e Interpretação:**

| Escore Total | Interpretação |
|-------------|---------------|
| 9–12 pontos | Desempenho preservado (função intacta) |
| 7–8 pontos | Limitação leve |
| 4–6 pontos | Limitação moderada a grave |
| 0–3 pontos | Comprometimento grave |

*Fonte: Guralnik JM et al. JAMA 1994; Pavasini R et al. Eur Heart J Acute Cardiovasc Care 2016; PubMed 35341435*

**MCID:** 0,5 pontos (mudança pequena); 1,0 ponto (mudança substancial).
*Fonte: Perera S et al. J Am Geriatr Soc 2006; Pavasini R et al. 2016.*

**Limiar de Fragilidade:** SPPB ≤ 9 = alta probabilidade de fragilidade (sensibilidade: 81% em amostra brasileira).
*Fonte: RehabMeasures SPPB; dados de validação na amostra brasileira conforme Nakano 2007.*

---

### 1.3 Dinamometria Manual — Dinamômetro Jamar

**Descrição do Protocolo:**
A dinamometria manual avalia força de preensão palmar como marcador de força muscular global. É componente do critério de fragilidade (EWGSOP2) e da avaliação de sarcopenia.

**Equipamento:** Dinamômetro Jamar calibrado (posição 2 da alça como padrão — ajustar para mãos menores se necessário), cadeira sem apoio de braços.

**Procedimento padronizado:**
1. Paciente sentado, ombro em adução, cotovelo fletido a 90°, antebraço em posição neutra
2. Três tentativas em mão dominante com intervalo de 60 segundos entre tentativas
3. Registrar a maior das três tentativas (em kgf)
4. Repetir em mão não dominante se clinicamente indicado
5. Registrar mão avaliada, ajuste de alça utilizado e se houve dor durante o teste

**Valores Normativos por Sexo e Faixa Etária:**

| Sexo | Faixa Etária | Faixa Normal (kg) | Limiar Baixa Força (EWGSOP2) |
|------|-------------|-------------------|------------------------------|
| Masculino | 60–69 anos | 35,0–40,0 kg | < 27 kg |
| Feminino | 60–69 anos | 19,0–24,0 kg | < 16 kg |

*Fonte: Dodds RM et al. Age Ageing 2016; EWGSOP2 — Cruz-Jentoft AJ et al. Age Ageing 2019;48(1):16-31*

**MCID (Diferença Mínima Clinicamente Importante):**
- Masculino: 5,0–6,5 kg
- Feminino: 2,7–5,0 kg

*Fonte: Dodds RM et al. 2016*

> **Nota EWGSOP2/EWGSOP3:** Os pontos de corte acima são baseados em EWGSOP2 (2018). Verificar publicação de EWGSOP3 antes de finalizar qualquer protocolo — se disponível, atualizar os limiares conforme nova edição.

**Interpretação Clínica:**
- Força abaixo do limiar EWGSOP2: indica provável sarcopenia — aprofundar investigação com velocidade de marcha (< 0,8 m/s) e/ou SPPB
- Registrar junto ao escore de fragilidade para determinar faixa de dosagem (Seção 2 e 5)

---

## 2. Sistema de Classificação de Fragilidade

> **Instrução para o Clínico:** Esta seção deve ser consultada ANTES de selecionar qualquer linha da tabela de dosagem (Seção 5). A classificação de fragilidade determina diretamente a faixa prescritiva do exercício.

### 2.1 Como Classificar o Paciente

Utilizar preferencialmente o **Fenótipo de Fried** como instrumento primário de classificação. O **CFS (Clinical Frailty Scale)** pode ser utilizado como instrumento rápido de triagem clínica ou em contextos com tempo limitado de avaliação. O **SPPB-BR** complementa a classificação com dados funcionais objetivos.

---

### 2.2 Fenótipo de Fried (Instrumento Primário)

*Fonte: Fried LP et al. J Gerontol A Biol Sci Med Sci. 2001;56(3):M146-56*

**Os 5 critérios de fragilidade de Fried:**

| # | Critério | Definição Operacional |
|---|----------|----------------------|
| 1 | **Perda de peso não intencional** | ≥ 4,5 kg (ou ≥ 5% do peso corporal) no último ano |
| 2 | **Exaustão/Fadiga autorrelatada** | Resposta positiva a 2 itens da CES-D: "sentia que tudo exigia esforço" ou "não conseguia continuar" ≥ 3 dias/semana |
| 3 | **Baixo nível de atividade física** | Gasto energético semanal < 383 kcal/sem (homens) ou < 270 kcal/sem (mulheres) — equivalente a < 3 caminhadas leves/semana |
| 4 | **Lentidão de marcha** | Velocidade < 0,8 m/s (ajustada por sexo e altura — limiares EWGSOP2) |
| 5 | **Fraqueza muscular** | Força de preensão abaixo dos limiares EWGSOP2: H < 27 kg, M < 16 kg |

**Classificação pela pontuação total:**

| Pontuação (critérios presentes) | Classificação | Implicação Clínica |
|--------------------------------|---------------|--------------------|
| 0 critérios | **Robusto** | Dosagem padrão (linha Robusto nas tabelas) |
| 1–2 critérios | **Pré-frágil** | Dosagem adaptada (linha Pré-frágil nas tabelas) |
| ≥ 3 critérios | **Frágil** | Dosagem conservadora (linha Frágil nas tabelas) |

---

### 2.3 Clinical Frailty Scale — CFS (Instrumento de Triagem Rápida)

*Fonte: Rockwood K et al. CMAJ 2005; versão de 9 níveis amplamente utilizada em contextos clínicos*

| Escore CFS | Descrição Clínica | Classificação Equivalente (Fried) |
|-----------|-------------------|-----------------------------------|
| 1 | Muito saudável | Robusto |
| 2 | Bem | Robusto |
| 3 | Bem — com doença controlada | Robusto |
| 4 | Vulnerável (sem dependência funcional) | Pré-frágil |
| 5 | Levemente frágil (com alguma dependência) | Pré-frágil |
| 6 | Moderadamente frágil (dependência em AVDs instrumentais e básicas) | Frágil |
| 7 | Severamente frágil (totalmente dependente) | Frágil |
| 8 | Muito severamente frágil (próximo do fim de vida) | Frágil |
| 9 | Terminalidade | Fora do escopo deste protocolo |

**Mapeamento resumido:**
- CFS 1–3 = Robusto
- CFS 4–5 = Pré-frágil
- CFS 6–9 = Frágil (CFS 9: encaminhar para cuidados paliativos)

---

### 2.4 Vinculação com SPPB-BR

O escore SPPB complementa a classificação de fragilidade:

| SPPB-BR | Indicação Clínica |
|---------|-------------------|
| ≤ 9 pontos | Alta probabilidade de fragilidade — verificar critérios de Fried; iniciar na faixa Frágil se confirmado |
| 7–8 pontos | Limitação leve — reavaliar com Fried para confirmar Pré-frágil vs. Frágil |
| ≥ 10 pontos | Sugere ausência de fragilidade, mas não exclui — confirmar com Fried |

> **Fluxo decisório:** Aplicar SPPB → Se SPPB ≤ 9, aplicar Fenótipo de Fried completo → Classificar → Selecionar linha da tabela de dosagem.

---

## 3. Princípio de Progressão

### 3.1 Definição Operacional: "Start Low, Go Slow, But Reach the Goal"

Este princípio orienta TODA prescrição de exercício nesta série de protocolos. Não é uma recomendação de cautela genérica — é uma estrutura prescritiva com três componentes operacionais:

**Componente 1 — "Start Low" (Começar Baixo):**
A sessão inicial começa sempre no **limite inferior da faixa clínica aceitável** para o nível de fragilidade do paciente.

| Nível de Fragilidade | Primeira Sessão — Referência de Carga |
|---------------------|---------------------------------------|
| Robusto | Limite inferior da faixa Robusto |
| Pré-frágil | Limite inferior da faixa Pré-frágil |
| Frágil | Limite inferior da faixa Frágil |
| Com ICC/DPOC conhecida | Iniciar na faixa Frágil independentemente do escore de fragilidade |

**Justificativa:** A carga inicial máxima tolerável de um idoso em nova intervenção é desconhecida. O limite inferior garante segurança na primeira exposição e permite avaliação da resposta cardiorrespiratória, musculoesquelética e cognitiva.

---

**Componente 2 — "Go Slow" (Progredir Devagar):**
A progressão de carga só ocorre quando os critérios de RPE (Escala de Borg) estão satisfeitos **por pelo menos 2 sessões consecutivas**.

| Nível de Fragilidade | Critério de Progressão de Carga | Taxa de Incremento |
|---------------------|--------------------------------|-------------------|
| Robusto | RPE < 12 (Borg 6-20) por 2 sessões consecutivas | +5% da carga |
| Pré-frágil | RPE < 13 (Borg 6-20) por 2 sessões consecutivas | +2,5–5% da carga |
| Frágil | RPE ≤ 12 (Borg 6-20) por 2 sessões consecutivas | +2,5% da carga |

> **Nota sobre betabloqueadores:** Em pacientes em uso de betabloqueadores, a frequência cardíaca não é indicador confiável de intensidade. Usar exclusivamente RPE (Borg 6-20) como parâmetro de intensidade (ver Seção 7 — Polifarmácia).

---

**Componente 3 — "Reach the Goal" (Atingir a Meta):**
O objetivo final é **funcional, não temporal**. A progressão continua até que o paciente atinja metas funcionais definidas — não até que um número de sessões seja atingido.

**Lógica de definição de metas funcionais:**

| Categoria de Meta | Exemplo Operacional |
|------------------|---------------------|
| Mobilidade | TUG < 13,5 seg (sair da faixa de risco de queda) |
| Força | Força de preensão acima do limiar EWGSOP2 (H > 27 kg, M > 16 kg) |
| Desempenho funcional | SPPB ≥ 10 pontos |
| AVDs específicas | Subir escadas sem apoio, caminhar 400 metros, transferir-se independentemente |
| Condição específica | Definida no protocolo individual (P-01 a P-20) |

**Anti-Padrões a Evitar:**
- Nunca progredir com base apenas em número de sessões ou semanas
- Nunca manter a mesma carga indefinidamente por "segurança" sem critério de reavaliação
- Nunca avançar de fase sem atingir os critérios funcionais de saída da fase atual

---

## 4. Padrão de Graduação de Evidência (Oxford CEBM)

### 4.1 Tabela de Níveis Oxford CEBM 2011

*Fonte: OCEBM Levels of Evidence Working Group. "The Oxford 2011 Levels of Evidence." Oxford Centre for Evidence-Based Medicine. cebm.ox.ac.uk*

| Nível CEBM | Tipo de Evidência | Mapeamento Nesta Série |
|-----------|-------------------|------------------------|
| **Nível 1** | Revisões sistemáticas de ECRs; ECRs individuais com IC estreito | **Nível A** |
| **Nível 2** | Revisões sistemáticas de estudos de coorte; estudos de coorte individuais; ECRs de baixa qualidade | **Nível B** |
| **Nível 3** | Revisões sistemáticas de estudos caso-controle; estudos caso-controle individuais | **Nível B** |
| **Nível 4** | Séries de casos; coortes e caso-controle de baixa qualidade | **Nível C** |
| **Nível 5** | Raciocínio por mecanismo (experiência especializada não sistematizada) | **Nível C** |

### 4.2 Mapeamento Consolidado: Nível A / B / C

| Nível Clínico | Equivalência Oxford CEBM | Descrição |
|--------------|--------------------------|-----------|
| **Nível A** | CEBM Nível 1 | Baseado em revisões sistemáticas de ECRs ou ECRs de alta qualidade. Recomendação forte — implementar sem restrição salvo contraindicação individual. |
| **Nível B** | CEBM Nível 2–3 | Baseado em estudos controlados, coortes ou revisões de menor nível. Recomendação moderada — implementar com monitoramento de resposta. |
| **Nível C** | CEBM Nível 4–5 | Baseado em séries de casos ou consenso especializado. Recomendação fraca — usar quando não há alternativa de nível A/B; justificar explicitamente. |

### 4.3 Fontes de Evidência (Tríade por EVID-03)

Toda busca de evidências para os protocolos desta série deve ser conduzida na seguinte tríade:

| Base de Dados | Uso Principal | Acesso |
|--------------|---------------|--------|
| **PubMed** | Literatura primária — ECRs, revisões sistemáticas, meta-análises | pubmed.ncbi.nlm.nih.gov |
| **Cochrane Library** | Revisões sistemáticas e meta-análises de alta qualidade | cochranelibrary.com |
| **PEDro** | ECRs de exercício com pontuação PEDro | pedro.org.au |

### 4.4 Formato de Anotação de Evidência por Intervenção

**Padrão obrigatório:** Cada intervenção recebe anotação de evidência na primeira menção em qualquer protocolo.

**Formato:**
```
[Nome da Intervenção] ([Categoria: Cinesioterapia | Terapia Manual | Modalidade Terapêutica])
Nível de Evidência: [A | B | C] (CEBM Nível [1-5])
Referência primária: [Autor et al. Título abreviado. Periódico Ano. PMID/DOI | PEDro score se ECR]
Alinhamento: [Diretriz principal — ex: OARSI 2019 | ACR 2022 | EWGSOP2]
```

**Exemplo:**
```
Exercício resistido progressivo (Cinesioterapia)
Nível de Evidência: A (CEBM Nível 1)
Referência primária: Fransen M et al. Exercise for osteoarthritis of the knee.
  Cochrane Database Syst Rev. 2015. PEDro score: 8/10
Alinhamento: OARSI 2019 (Bannuru et al.) — Tratamento Central, sem restrição de comorbidade
```

**Anti-Padrões a Evitar:**
- Nunca declarar "Nível A" sem a referência primária ao lado
- Nunca citar OARSI 2024 como "nova diretriz" — o artigo "Year in Review 2024" não substitui OARSI 2019 (ver nota abaixo)
- Nunca usar nível de evidência genérico para o protocolo inteiro — cada intervenção precisa de anotação individual

> **Nota OARSI 2024:** A revisão de 2024 publicada em Osteoarthritis and Cartilage acrescenta nuances sobre magnitude de efeito na reabilitação, mas não constitui atualização de diretriz e não substitui as recomendações de OARSI 2019 (Bannuru et al., PubMed 31278997). Qualquer sentença que comece com "As diretrizes OARSI de 2024 recomendam..." está incorreta. Citar OARSI 2019 como diretriz vigente e mencionar a revisão de 2024 apenas como contexto suplementar.

---

## 5. Padrão de Formato de Dosagem

### 5.1 Especificação do Formato de Duas Colunas

Todo parâmetro de exercício nos protocolos desta série deve ser apresentado no formato de duas colunas por nível de fragilidade:

**Colunas:** `Valor Recomendado | Faixa Clínica Aceitável`

- **Valor Recomendado:** O ponto ótimo baseado na melhor evidência disponível
- **Faixa Clínica Aceitável:** O intervalo dentro do qual o fisioterapeuta pode adaptar conforme resposta individual do paciente

**Estrutura da Tabela:**

```
| Parâmetro | Robusto                         | Pré-frágil                      | Frágil                          |
|           | Valor Rec. | Faixa Aceitável     | Valor Rec. | Faixa Aceitável     | Valor Rec. | Faixa Aceitável     |
```

> **Anti-padrão crítico:** Nunca prescrever dose única sem faixa de adaptação clínica. Nunca escrever apenas "3 séries × 10 repetições" sem a faixa e sem estratificação por fragilidade.

---

### 5.2 Template de Tabela de Dosagem com Estratificação por Fragilidade

Exemplo aplicável a exercício resistido de membros inferiores (adaptável para qualquer intervenção cinesiológica):

| Parâmetro | Robusto — Valor Rec. | Robusto — Faixa Aceitável | Pré-frágil — Valor Rec. | Pré-frágil — Faixa Aceitável | Frágil — Valor Rec. | Frágil — Faixa Aceitável |
|-----------|---------------------|--------------------------|------------------------|------------------------------|--------------------|-----------------------|
| Carga inicial | 60% 1RM | 50–70% 1RM | 40% 1RM | 30–60% 1RM | 30% 1RM | 20–40% 1RM |
| Séries | 3 | 2–4 | 2–3 | 1–3 | 2 | 1–3 |
| Repetições | 10–12 | 8–15 | 8–10 | 6–12 | 6–8 | 5–10 |
| Frequência | 3×/semana | 2–4×/semana | 2–3×/semana | 2–3×/semana | 2×/semana | 1–3×/semana |
| Progressão (carga) | +5% quando RPE < 12 | — | +2,5–5% quando RPE < 13 | — | +2,5% quando RPE ≤ 12 | — |

*Este template deve ser reproduzido e preenchido para cada intervenção de exercício em cada protocolo individual.*

---

### 5.3 Instruções de Uso do Template

1. **Aplicar a bateria universal (Seção 1)** para obter TUG, SPPB e força de preensão
2. **Classificar fragilidade (Seção 2)** usando Fenótipo de Fried ± CFS ± SPPB
3. **Selecionar a coluna correspondente** ao nível de fragilidade classificado
4. **Iniciar no Valor Recomendado** (ou no limite inferior da faixa na primeira sessão — Seção 3)
5. **Progressão:** Aguardar cumprimento dos critérios de RPE por 2 sessões consecutivas antes de incrementar
6. **Reavaliação:** Repetir bateria universal conforme cadência definida no protocolo individual

---

## 6. Registro de Ferramentas de Desfecho em Português Brasileiro

> **Regra de Citação:** Todo instrumento de desfecho deve aparecer com o sufixo "-BR" e sua citação de validação brasileira. Nunca citar "SPPB", "WOMAC", "MoCA" ou "ODI" sem o sufixo e a referência.

### 6.1 SPPB-BR — Short Physical Performance Battery (Versão Brasileira)

| Propriedade | Valor |
|------------|-------|
| **Citação de Validação** | Nakano MM. Versão brasileira da Short Physical Performance Battery (SPPB). 2007 |
| **Confiabilidade** | ICC = 0,83 (teste-reteste) |
| **MCID** | 0,5 pontos (mudança pequena); 1,0 ponto (mudança substancial) |
| **Limiar de Fragilidade** | ≤ 9 pontos = alta probabilidade de fragilidade (sensibilidade: 81% em amostra brasileira) |
| **Escore Máximo** | 12 pontos |
| **Domínios** | Equilíbrio estático (0–4), Velocidade de marcha (0–4), Força de MMII / levantar-sentar (0–4) |
| **Interpretação** | 9–12: intacto; 7–8: leve; 4–6: moderado/grave; 0–3: grave |

*Fontes: Nakano (2007); Guralnik JM et al. JAMA 1994; Pavasini R et al. PubMed 35341435*

---

### 6.2 WOMAC-BR — Western Ontario and McMaster Universities Osteoarthritis Index (Versão Brasileira)

| Propriedade | Valor |
|------------|-------|
| **Citação de Validação (Primária Peer-Reviewed)** | Oliveira AM et al. BMC Musculoskelet Disord 2022; PMC9673866 |
| **Citação de Validação (Tradução Original)** | Fernandes MI. Tradução e validação do questionário de qualidade de vida específico para osteoartrose WOMAC. UNIFESP, 2003 (dissertação de mestrado — usar com citação secundária peer-reviewed) |
| **Validade Adicional** | ELSA-Brasil Musculoskeletal cohort; PubMed 31858210 |
| **Domínios** | Dor (5 itens); Rigidez (2 itens); Função física (17 itens) |
| **Total de itens** | 24 itens |
| **Confiabilidade** | Adequada — validação de constructo confirmada por Oliveira et al. 2022 |
| **Escala de Resposta** | Likert 5 pontos (0–4) por item; escore total: 0 (sem sintomas) a 96 (sintomas máximos) |
| **Uso Primário** | Desfecho específico para osteoartrite (dor, rigidez e função) |

> **Anti-padrão:** Nunca citar apenas Fernandes (2003) como validação única — é dissertação de mestrado, não artigo peer-reviewed. Usar Oliveira et al. (2022, PMC9673866) como validação primária e Fernandes (2003) como fonte da tradução original.

---

### 6.3 MoCA-BR — Montreal Cognitive Assessment (Versão Brasileira)

| Propriedade | Valor |
|------------|-------|
| **Citação de Validação** | Memoria CM et al. Int Psychogeriatr 2013; PubMed 22368034 |
| **Sensibilidade** | 81% para CCL (Comprometimento Cognitivo Leve) no ponto de corte 25 |
| **Especificidade** | 77% para CCL no ponto de corte 25 |
| **AUC** | 0,82 |
| **Escore Máximo** | 30 pontos |
| **Ajuste por Escolaridade** | +1 ponto para pacientes com ≤ 12 anos de escolaridade formal |
| **Interpretação (com ajuste)** | ≥ 26: normal; < 26: rastreio positivo para CCL |
| **Uso Primário** | Triagem cognitiva para CCL em idosos |

> **Anti-padrão crítico — Ajuste de Escolaridade:** Nunca aplicar o ponto de corte fixo (25 ou 26) sem verificar escolaridade. A população geriátrica brasileira tem alta prevalência de baixa escolaridade formal — aplicar +1 ponto para ≤ 12 anos de estudo é clinicamente essencial para evitar falsos positivos. Qualquer protocolo que cite MoCA-BR sem a nota de ajuste de escolaridade está incompleto.

---

### 6.4 ODI-BR — Oswestry Disability Index (Versão Brasileira)

| Propriedade | Valor |
|------------|-------|
| **Citação de Validação** | Vigatto R, Alexandre NMC, Correa Filho HR. Spine 2007; PubMed 17304141 |
| **Validação Adicional** | Mancin S et al. 2008; PMC2518761 (responsividade confirmada) |
| **Alfa de Cronbach** | 0,87 |
| **ICC** | 0,99 (excelente confiabilidade teste-reteste) |
| **Correlação com Dor** | r = 0,66 (correlação moderada) |
| **Domínios** | 10 seções: intensidade da dor, cuidados pessoais, levantamento de peso, caminhada, sentar, ficar de pé, dormir, vida sexual, vida social, viagem |
| **Escore** | 0–100% (0–20%: incapacidade mínima; 21–40%: moderada; 41–60%: grave; 61–80%: muito grave; 81–100%: máxima incapacidade ou exageração) |
| **Uso Primário** | Desfecho de incapacidade funcional em lombalgia |

---

## 7. Arquitetura de Segurança (Templates)

### 7.1 Monitoramento de Dor (NRS 0-10) — Limiares por Fase

*Base: prática clínica estabelecida em RCTs de exercício para reabilitação geriátrica; alinhado com recursos educacionais IASP sobre dor em idosos*

| Fase | Limiar de Interrupção Imediata | Limiar de Modificação | Dor Aceitável Durante Exercício |
|------|-------------------------------|----------------------|---------------------------------|
| **Fase 1 (Aguda/Protegida)** | NRS ≥ 5 | NRS 3–4 → reduzir carga 25% | NRS ≤ 3 (leve, esperada) |
| **Fase 2 (Subaguda/Fortalecimento)** | NRS ≥ 6 | NRS 4–5 → reduzir carga 20% | NRS ≤ 4 |
| **Fase 3 (Avançada/Funcional)** | NRS ≥ 7 | NRS 5–6 → reduzir carga 15% | NRS ≤ 5 |

> **Nota de Fonte:** Os limiares NRS acima são baseados em prática clínica estabelecida e parâmetros de segurança de RCTs de referência em reabilitação musculoesquelética geriátrica. Um documento IASP específico para limiares de parada durante exercício não foi confirmado na literatura — verificar com RCTs primários de OA/reabilitação antes de publicação definitiva.

**Regra Geral (pós-exercício):**
> Dor pós-exercício que excede a dor pré-exercício em mais de 2 pontos na NRS e persiste por mais de 24 horas = sobrecarga. Reduzir volume na sessão seguinte.

---

### 7.2 Bandeiras Vermelhas — Escalonamento Imediato

| Sinal / Sintoma | Ação Imediata | Destino de Encaminhamento |
|-----------------|---------------|--------------------------|
| Dor articular aguda de novo, sem trauma identificado | Suspender sessão | Reumatologista |
| Inchaço articular súbito com calor e eritema | Suspender sessão | Reumatologista / urgência |
| Febre associada a dor articular (> 37,8°C) | Suspender sessão | Clínico / urgência |
| Dor irradiada com déficit neurológico novo (fraqueza, parestesia) | Suspender sessão | Neurocirurgia / urgência |
| Dor em repouso noturna progressiva (suspeita oncológica) | Não iniciar exercício | Oncologista / clínico |
| Dispneia súbita e desproporcional ao esforço | Suspender sessão | Cardiologista / urgência |
| Hipotensão ortostática sintomática (queda PA sistólica > 20 mmHg) | Suspender sessão | Clínico |
| Dor torácica, pressão precordial ou irradiação para braço/mandíbula | Suspender sessão — acionar emergência | SAMU 192 / urgência cardiológica |
| Palpitações com tontura ou síncope | Suspender sessão | Cardiologista / urgência |
| Saturação O₂ < 90% durante exercício | Suspender sessão | Cardiologista / pneumologista |
| Confusão mental aguda ou desorientação súbita | Suspender sessão | Neurologia / urgência |

> **Instrução:** Esta tabela deve ser reproduzida integralmente em cada protocolo individual. Acrescentar bandeiras específicas da condição clínica (ex: sinais de infecção de prótese para P-10/P-11).

---

### 7.3 Interações com Polifarmácia

*Base: Lancet Healthy Longevity 2025 (ScienceDirect pii/S2666756825000820); ACR 2022; literatura específica por classe farmacológica*
*Referência de segurança: AGS Beers Criteria 2023 — verificar atualizações AGS Beers para 2025/2026 antes de publicação definitiva*

| Classe Farmacológica | Implicação para o Exercício | Modificação Prescritiva |
|---------------------|----------------------------|------------------------|
| **AINEs** (AAS, ibuprofeno, naproxeno, diclofenaco) | Mascaramento da dor → risco de sobrecarga; risco cardiovascular e renal em exercício intenso; risco de sangramento GI | Reforçar monitoramento NRS; evitar exercício de alta intensidade sem supervisão; comunicar equipe médica se uso crônico |
| **Corticosteroides** (uso crônico > 3 meses) | Miopatia corticoesteroide, perda óssea acelerada → fragilidade muscular e risco aumentado de fratura por estresse | Reduzir cargas de impacto; priorizar fortalecimento de baixa carga; considerar densitometria antes de exercício de alta carga; comunicar ortopedista |
| **Anti-hipertensivos — betabloqueadores** (propranolol, atenolol, metoprolol) | FC embotada — frequência cardíaca não é indicador confiável de intensidade do exercício | Usar exclusivamente RPE (Borg 6-20) como indicador de intensidade; nunca usar % FC máx como parâmetro isolado |
| **Anti-hipertensivos — vasodilatadores e diuréticos** (anlodipino, furosemida, hidroclorotiazida) | Risco de hipotensão ortostática, especialmente no período pós-exercício | Período de resfriamento obrigatório (mínimo 10 min); orientar levantar lentamente; monitorar PA pré e pós-sessão; hidratação adequada |
| **Anticoagulantes** (varfarina, rivaroxabana, apixabana, heparina) | Risco aumentado de sangramento em contusões e traumas leves | Evitar exercícios de contato; adaptar superfícies e ambientes; monitorar equimoses; comunicar equipe médica sobre qualquer queda ou trauma |
| **Benzodiazepínicos e sedativos** (diazepam, clonazepam, zolpidem) | Sonolência residual, aumento do risco de queda, comprometimento cognitivo transitório | Agendar sessões longe do pico de ação do medicamento; enfatizar supervisão de equilíbrio e marcha; avaliar com MoCA-BR se há suspeita de comprometimento cognitivo aumentado |

> **AGS Beers Criteria 2023:** Verificar atualizações AGS Beers para 2025/2026 antes de qualquer publicação definitiva de protocolo. Os benzodiazepínicos e AINEs figuram como medicamentos potencialmente inapropriados para idosos nas edições vigentes.

---

### 7.4 Precauções Cardiorrespiratórias — Template Universal

> **Template Universal Estabelecido em Fase 6 (P-15 + P-16):** Esta seção define o template de Precauções Cardiorrespiratórias padronizado que todos os 20 protocolos desta série adotam em sua Seção 11 após o passe retroativo da Fase 6 (Plano 06-02). As subseções 11.1 e 11.2 são IDÊNTICAS em todos os protocolos; as subseções 11.3–11.5 são adaptadas ao diagnóstico primário de cada protocolo.

#### 7.4.1 Subseção 11.1 — Protocolo de Avaliação Pré-Sessão (UNIVERSAL)

**Registrar antes de CADA sessão:**

| Parâmetro | Procedimento | Critério de NÃO-INÍCIO |
|-----------|-------------|----------------------|
| **PA sistólica/diastólica** | Repouso sentado, 5 min, braço direito | > 180/110 mmHg = aguardar 10 min + reavaliar; se mantida = contatar médico |
| **FC de repouso** | Pulso radial ou monitor, 60 s | > 120 bpm em repouso = não iniciar exercício aeróbico |
| **SpO₂ basal** | Oxímetro de pulso, dedo indicador, 2 min repouso | ≤ 90% = não iniciar exercício aeróbico sem avaliação |
| **Dispneia em repouso** | Borg Dispneia 0–10 | ≥ 5 em repouso = não iniciar |
| **Edema de tornozelo** | Inspeção bilateral | Novo edema ou piora aguda desde última sessão = contatar médico antes |

> **Nota de expansão por diagnóstico:** Protocolos com IC (P-16) adicionam verificação de peso diário nesta tabela. Protocolos com DPOC (P-15) adicionam verificação de sinais de exacerbação.

#### 7.4.2 Subseção 11.2 — Indicadores de Parada Imediata (UNIVERSAL)

| Indicador | Limiar |
|-----------|--------|
| **Dor torácica, pressão precordial ou irradiação** | Qualquer ocorrência — SAMU 192 |
| **Dispneia súbita desproporcional ao esforço** | Qualquer ocorrência |
| **Palpitações com tontura ou síncope** | Qualquer ocorrência — SAMU 192 |
| **PA sistólica durante exercício** | > 200 mmHg |
| **Queda de PA sistólica durante esforço progressivo** | > 10 mmHg |
| **SpO₂ durante exercício** | < 90% (P-15 DPOC: parada imediata se < 88%) |
| **Cianose perioral ou periférica** | Qualquer ocorrência — SAMU 192 |
| **Confusão mental de início agudo** | Qualquer ocorrência — SAMU 192 |

#### 7.4.3 Estrutura das Subseções 11.3–11.5 (Específicas por Protocolo)

| Subseção | Conteúdo | Notas |
|----------|---------|-------|
| **11.3 Monitoramento Durante a Sessão** | SpO₂ e/ou RPE conforme diagnóstico primário | DPOC: SpO₂ a cada 5 min + Borg Dispneia a cada 10 min. IC: RPE Borg 6–20 a cada 10 min (FC apenas observacional) |
| **11.4 Adaptações por Comorbidade Coexistente** | Modificadores quando DPOC/IC coexiste com diagnóstico primário diferente | DPOC coexistente em IC = P-15 como comodificador. IC coexistente em DPOC = P-16 como comodificador |
| **11.5 Especificidades do Diagnóstico Primário** | Modificadores únicos ao diagnóstico principal | DPOC: dessaturação silenciosa + suplementação O₂. IC: peso diário + termorregulação + edema |

#### 7.4.4 Regras de Aplicação do Template Universal

1. **Retroativo:** Plano 06-02 insere este template em todos os 10 protocolos das Fases 1–5
2. **Consistência obrigatória:** Limiares na Subseção 11.1 e 11.2 são idênticos em todos os protocolos — não alterar valores sem revisar TODOS os protocolos
3. **Escala de Borg — distinção obrigatória:**
   - **Borg Dispneia 0–10:** diagnóstico primário DPOC (P-15) e como segundo instrumento em outros protocolos
   - **Borg RPE 6–20:** diagnóstico primário IC (P-16) e em qualquer protocolo com betabloqueador ativo
4. **SpO₂ ≤ 90% em qualquer protocolo:** NÃO iniciar exercício aeróbico — regra universal
5. **FC com betabloqueador:** RPE exclusivamente — regra universal para todos os protocolos quando betabloqueador documentado

#### 7.4.5 Passe Retroativo — Precauções Cardiorrespiratórias (Fase 6, Plano 06-02)

> **Data do passe retroativo:** 2026-03-13
> **Executor:** Plano 06-02 — Cluster Cardiorrespiratório
> **Fonte do template:** P-15-DPOC.md Seção 11.1 + 11.2 (template canônico)

**Status de cada protocolo da série:**

| Protocolo | Condição | Status | Subseção 11.4 Adicionada |
|-----------|----------|--------|--------------------------|
| **P-01** | Osteoartrite | ATUALIZADO — Plano 06-02 (2026-03-13) | Risco cardiovascular em sedentário + AINEs |
| **P-03** | AVC (fase crônica) | ATUALIZADO — Plano 06-02 (2026-03-13) | FA + anticoagulação + disfunção autonômica pós-AVC |
| **P-04** | Osteoporose | ATUALIZADO — Plano 06-02 (2026-03-13) | Valsalva + bifosfonatos + corticosteroides |
| **P-05** | Fratura de Fêmur | ATUALIZADO — Plano 06-02 (2026-03-13) | TEV + anemia pós-op + hipotensão ortostática pós-imobilização |
| **P-06** | Parkinson | ATUALIZADO — Plano 06-02 (2026-03-13) | Disautonomia autonômica + comprometimento respiratório + levodopa |
| **P-07** | Quedas | ATUALIZADO — Plano 06-02 (2026-03-13) | HO como fator de risco de queda + PBT precauções + STOPPFall |
| **P-08** | Sarcopenia | ATUALIZADO — Plano 06-02 (2026-03-13) | HIRT cardiovascular screening + Valsalva em alta carga |
| **P-10** | ATJ | ATUALIZADO — Plano 06-02 (2026-03-13) | TEV pós-ATJ + estresse de torniquete + hipotensão ortostática |
| **P-11** | ATQ | ATUALIZADO — Plano 06-02 (2026-03-13) | TEV pós-ATQ + risco cardiovascular cirúrgico + hipotensão ortostática |
| **P-15** | DPOC | ORIGINAL — template criado em Plano 06-01 (2026-03-13) | Dessaturação silenciosa + suplementação O₂ + broncodilatador |
| **P-16** | Insuficiência Cardíaca | ORIGINAL — template criado em Plano 06-01 (2026-03-13) | Peso diário + termorregulação + RPE exclusivo |
| **P-18** | Demência | ATUALIZADO — Plano 06-02 (2026-03-13) | Capacidade limitada de autorrelato + tabela de sinais comportamentais |

**Valores canônicos de limiar (referência única — não alterar individualmente):**

| Parâmetro | Limiar de NÃO-INÍCIO | Limiar de PARADA IMEDIATA |
|-----------|----------------------|--------------------------|
| PA sistólica/diastólica | > 180/110 mmHg (aguardar 10 min + reavaliar) | > 200 mmHg durante exercício |
| FC de repouso | > 120 bpm | Queda de PA sistólica > 10 mmHg durante esforço |
| SpO₂ basal | ≤ 90% (sem avaliação/suplementação) | < 90% durante exercício (P-15 DPOC: < 88%) |
| Borg Dispneia (0–10) em repouso | ≥ 5 | ≥ 8 durante exercício |
| Edema de tornozelo | Novo ou piora aguda | — |

**Instrução para protocolos das Fases 7–8:**
- Protocolos futuros (P-02, P-09, P-12, P-13, P-14, P-17, P-19, P-20) devem incluir o template universal em sua Seção 11 **no momento da criação** — não aguardar passe retroativo
- Subseções 11.1 e 11.2 devem ser copiadas verbatim desta seção 7.4
- Subseção 11.3 deve incluir adaptações por ICC/DPOC coexistente com referência a P-15 e P-16
- Subseção 11.4 deve incluir especificidades cardiorrespiratórias do diagnóstico primário do novo protocolo

---

## 8. Esqueleto do Índice de Referência Cruzada

> **Status:** 20/20 — COMPLETO. Todas as linhas preenchidas. Última atualização: 2026-03-14 (Fase 8 — P-17 Neuropatia Periférica Diabética e P-14 Disfunção do Assoalho Pélvico — Protocolos Especializados). Índice de Referência Cruzada completo — corpus de 20 protocolos navegável.

### 8.1 Matriz de Interação entre Protocolos (Shell 20×20)

| Protocolo | Condição | Interações Conhecidas | Modificadores Compartilhados | Precauções Específicas |
|-----------|----------|----------------------|------------------------------|------------------------|
| **P-01** | Osteoartrite / Artrose | P-04 (Osteoporose), P-07 (Quedas), P-08 (Sarcopenia), P-10 (ATJ), P-11 (ATQ), P-20 (Gonalgia/Coxalgia) | Fragilidade, corticosteroides, AINEs, anticoagulantes | ICC/DPOC: iniciar na faixa Frágil; Corticosteroides crônicos: consultar P-04 antes de exercício de impacto; Sarcopenia confirmada: ajustar dosagem conforme P-08 |
| **P-02** | Lombalgia Crônica e Estenose de Canal | P-04 (Osteoporose — restrições de carga óssea P-04 Seção 5.2 quando T-score ≤ -2,5; NUNCA flexão de coluna com carga em osteoporose); P-07 (Quedas — P-07 Seção 5.2 protocolo de sessão quando TUG > 13,5 seg; P-07 Seção 7.2 hierarquia de equilíbrio; FES-I-BR ≥ 23 = ativar P-07 completo); P-08 (Sarcopenia — dosagem de resistência P-08 Seção 6.3 quando dinamometria < EWGSOP2); P-09 (diagnóstico diferencial — espondilose sem claudicação neurogênica); P-12 (diagnóstico diferencial — DLC inespecífica quando substrato não explica carga de dor) | Fragilidade (Fried); opioides e gabapentinoides (alto risco de queda + mascaramento de dor — STOPPFall); corticosteroides (perda óssea acelerada + miopatia — ativar P-04); AINEs crônicos (risco GI/renal); betabloqueadores (usar RPE exclusivo) | **Síndrome de cauda equina:** SAMU 192 + NÃO MOBILIZAR (retenção urinária + anestesia em sela + fraqueza MMII bilateral = emergência cirúrgica absoluta). **Bias de flexão:** extensão lombar CONTRAINDICADA em todas as fases — diferença terapêutica fundamental em relação a P-09 (inversão terapêutica). **Claudicação neurogênica vs. vascular:** diagnóstico diferencial obrigatório com tabela ITB + posição de alívio antes de iniciar P-02. **CSI-BR ≥ 40:** progressão tempo-contingente; NRS deixa de ser critério de progressão; TUG + SPPB + distância de claudicação governam avanço. **PNE:** adjunto (2–3 sessões); foco em mecanismo de estenose e por que posição importa. **Cadeia de modificadores:** P-04 Seção 5.2 (carga óssea) → P-08 Seção 6.3 (resistência) → P-07 Seções 5.2+7.2 (sessão + equilíbrio). |
| **P-03** | AVC/AVE (fase crônica) | P-01 (OA coexistente — dor articular governa carga), P-04 (Osteoporose — restrições de carga óssea via P-04 Seção 5.2 quando T-score ≤ -2,5), P-05 (Fratura de fêmur prévia — CFS na admissão + precauções de carga), P-06 (Parkinson coexistente — cluster neuromotor paralelo; freezing de marcha afeta TEMPLATE), P-07 (Quedas — P-07 Seção 5.2 protocolo de sessão OBRIGATÓRIO para todos; P-07 Seção 7.2 hierarquia de equilíbrio governa Fases 1–3), P-08 (Sarcopenia — dosagem de resistência via P-08 Seção 6.3 quando dinamometria < limiar EWGSOP2), P-10 (ATJ — se coexistente; precauções de ROM de joelho), P-11 (ATQ — se coexistente; precauções de luxação), P-18 (Comprometimento cognitivo além do pós-AVC — cluster neuromotor; MoCA-BR governa adaptações de instrução e TEMPLATE) | **Fase crônica > 6 meses** (nunca aguda/subaguda). **Fundação neuroplástica:** 10 princípios Kleim & Jones 2008 (PMID 18230848) governam progressão de fases. **TEMPLATE CLUSTER NEUROMOTOR** (Seção 7.2): criado em P-03, referenciado por P-06 e P-18; BBS-BR ≥ 40 + TUG < 20 como critérios de entrada; 4 níveis DT-1 a DT-4. **Adaptação de instrução para afasia/apraxia** (Seção 5.3): hierarquia de 5 modos (demonstração física → mão-sobre-mão → feedback visual → palavra-chave → verbal completo). **PAINAD-BR** (Seção 8.2, PubMed 25993063): instrumento primário de dor quando afasia grave torna NRS inválida. Instrumentos de avaliação: TUG, SPPB-BR, Dinamometria, BBS-BR (PubMed 15334208), FES-I-BR (PubMed 20730369), MoCA-BR (PubMed 22368034), Ashworth Modificada, FMA-MMII. Diretrizes primárias: AHA/ASA 2016 (PubMed 27145936) + VA/DoD 2024 (PubMed 39832369). NÃO COBRE: AVC agudo/subagudo, TCE, lesão medular. | **Recorrência de AVC:** Novo déficit neurológico focal = SAMU 192 imediatamente (protocolo FAST). Cefaleia súbita intensa = possível hemorragia recorrente — emergência. **Anticoagulação:** INR instável (varfarina) contraindica início; verificar INR < 30 dias. **Fibrilação atrial:** FC repouso > 100 bpm = comunicar cardiologista antes de exercício aeróbico. **Espasticidade grave:** Ashworth = 4 = contraindicação relativa → avaliação de toxina botulínica antes da reabilitação intensiva. **Dupla tarefa:** NUNCA iniciar fora dos critérios BBS-BR ≥ 40 + TUG < 20 — risco de queda documentado. **Cadeia de modificadores:** P-04 Seção 5.2 (prioridade 1) → P-08 Seção 6.3 (prioridade 2) → P-07 Seções 5.2 + 7.2 (prioridade 3) → P-03 base. |
| **P-04** | Osteoporose | P-08 (Sarcopenia — osteosarcopenia), P-01 (OA — corticosteroides aceleram perda óssea), P-05 (Fratura de Fêmur — osteoporose é substrato), P-07 (Quedas — queda em osteoporótico = alto risco de fratura), P-09 (Artrose de Coluna — diferenciação de dor vertebral), P-10 (ATJ — T-score antes de carga pós-op), P-11 (ATQ — ONJ com bifosfonatos pré-cirurgia), P-16 (IC — corticosteroides crônicos), P-19 (Fraturas Vertebrais — P-04 é o protocolo de manutenção crônica após P-19) | **Restrições de carga óssea:** Tabela MODIFICADOR TRANSVERSAL em P-04 Seção 5.2 — todos os protocolos que abordam paciente com osteoporose ou risco de fratura devem citar esta tabela. 4 categorias de risco (Baixo/Médio/Alto/Muito Alto) × 3 eixos de restrição (flexão espinal / impacto / resistência). Regra geral espinal: extensão preferida sobre flexão em toda osteoporose (Sinaki 1984, PubMed 6487063). Hip hinge obrigatório em todos os movimentos. Para resistência em Muito Alto Risco ou osteosarcopenia: citar P-08 Seção 6.3 e aplicar teto de carga P-04 Seção 5.2. | Categoria de risco governa teto de carga em TODAS as fases — progressão de fase não elimina restrições. FRAX + T-score (não T-score isolado) para estratificação. Nova dor vertebral aguda durante tratamento = suspender imediatamente → ortopedia. Bifosfonatos + exercício resistido são sinérgicos (BHOF 2022) — comunicar sinergia ao paciente como motivação de aderência. Em osteosarcopenia: ativar co-tratamento P-04 + P-08 simultaneamente. |
| **P-05** | Fratura de Fêmur Proximal / Quadril | P-04 (Osteoporose — osteoporose é substrato frequente da fratura por fragilidade; restrições de carga óssea via P-04 Seção 5.2 obrigatórias em TODAS as fases), P-08 (Sarcopenia — fraqueza muscular pré-fratura comum; dosagem de resistência via P-08 Seção 6.3 a partir da Fase 2), P-07 (Quedas — prevenção de queda recorrente pós-fratura; P-07 Seção 5.2 protocolo de sessão + P-07 Seção 7.2 hierarquia de equilíbrio como comodificador obrigatório), P-01 (OA — OA de quadril/joelho frequentemente coexiste), P-10 (ATJ — problemas contralaterais ou concorrentes de joelho), P-11 (ATQ — quando fratura tratada com artroplastia total; consultar P-11 para precauções de luxação), P-06 (Parkinson — quedas e fraturas altamente comórbidos), P-18 (Demência — delirium pós-fratura e desafios de adesão) | **CFS na admissão:** Clinical Frailty Scale (Rockwood 2005) mandatório na admissão de P-05 como preditor de mortalidade (PubMed 33215137). Mapeamento: CFS 1–3 = Robusto; CFS 4–5 = Pré-frágil; CFS 6–7 = Frágil; CFS 8 = paliativo conjunto; CFS 9 = fora do escopo. Complementar com Fenótipo de Fried quando possível. **Três modificadores cruzados consumidos:** P-04 Seção 5.2 (restrições de carga óssea — sempre), P-08 Seção 6.3 (dosagem de resistência — Fase 2+), P-07 Seções 5.2 e 7.2 (protocolo de sessão e hierarquia de equilíbrio — todas as fases). | CFS ≥ 7: equipe interdisciplinar obrigatória; CFS 8: abordagem paliativa conjunta. FES-I-BR ≥ 23: ativação mandatória de P-07 como comodificador. TEV awareness: seção declara escopo de prática — fisioterapia NÃO prescreve regime anticoagulante; tabela de implicações de exercício por agente (LMWH, DOACs, aspirina, warfarina). Mobilização precoce < 48h como profilaxia mecânica de TEV (AAOS 2021). Delirium pós-operatório: MoCA-BR obrigatório; incidência 35–65% em idosos com fratura de quadril. |
| **P-06** | Doença de Parkinson | P-01 (OA — artropatia coexistente frequente; dor articular governa carga nos exercícios resistidos), P-03 (AVC — cluster neuromotor compartilhado; TEMPLATE CLUSTER NEUROMOTOR — P-03 Seção 7.2 referenciado por P-06 Fase 3 com adaptações de on/off), P-04 (Osteoporose — quedas em DP = fratura frequente; ativar P-04 Seção 5.2 quando T-score presente), P-05 (Fratura de Fêmur — altamente comórbido com DP; instabilidade postural + freezing aumenta risco de queda recorrente), P-07 (Quedas — P-07 Seção 5.2 protocolo de sessão OBRIGATÓRIO; P-07 Seção 7.2 hierarquia de equilíbrio governa Fases 1–3; freezing de marcha como fator de risco específico), P-08 (Sarcopenia — HIRT é recomendação APTA CPG 2022 grau A; dosagem de resistência via P-08 Seção 6.3), P-10 (ATJ — queda + rigidez pós-op em Parkinson), P-11 (ATQ — alta comorbidade ATQ/Parkinson; instabilidade postural aumenta risco de luxação recorrente), P-18 (Demência — DLB / demência de Parkinson; comprometimento cognitivo requer adaptações de instrução de P-18 quando MoCA < 18) | **Regra de timing de levodopa:** Sessões 45–60 min pós-dose dopaminérgica (estado ON) — regra estrutural em TODAS as fases. **Tabela ON/OFF:** Diferenciação de prescrição por estado clínico (P-06 Seção 5.2) — exercício de alta intensidade e progressão de equilíbrio APENAS no estado ON; protocolo de sessão em estado OFF (carga reduzida 30%, sem progressão, exercícios sentados). **Treinamento de cuidadores:** Componente FORMAL — 3 sessões obrigatórias integradas nas fases (não apêndice optativo); conteúdo: reconhecer estados ON/OFF, cueing para freezing, suporte de marcha, segurança domiciliar (APTA CPG 2022). **TEMPLATE CLUSTER NEUROMOTOR** (Fase 3): referência a P-03 Seção 7.2 com adaptações P-06 — ON obrigatório para DT; reduzir complexidade se approaching-off. **Cueing externo:** Visual + auditivo + tátil para freezing de marcha (Nieuwboer 2007, Lancet Neurol). **HIRT:** Alta intensidade resistida por APTA CPG 2022 — seguro e eficaz no estado ON. Diretriz primária: APTA CPG 2022 (PubMed 34963139; PMC9046970). NÃO COBRE: parkinsonismos atípicos (PSP, MSA), Hoehn e Yahr 5, tremor essencial. Instrumentos: TUG, SPPB-BR, Dinamometria, BBS-BR, FES-I-BR, MoCA-BR, MDS-UPDRS III (estado ON), Hoehn e Yahr Modificada, Registro de horários de medicação dopaminérgica. | **Crise acinética:** Rigidez extrema + hipertermia + instabilidade autonômica = SAMU 192 — emergência neurológica. **Haloperidol CONTRAINDICADO** em DP (piora dramática de sintomas motores) — alertar equipe se prescrito. **Dupla tarefa (TEMPLATE P-03 Seção 7.2):** NUNCA iniciar fora dos critérios BBS-BR ≥ 40 + TUG < 20 + estado ON. **Discinesias:** Se interferem no equilíbrio durante DT, pausar e retomar em DT-1 após resolução. **Hipotensão ortostática:** PA ortostática obrigatória antes de cada sessão (agonistas dopaminérgicos + disautonomia autonômica). **Cadeia de modificadores:** P-04 Seção 5.2 (carga óssea, se osteoporose) → P-08 Seção 6.3 (HIRT) → P-07 Seções 5.2 + 7.2 (sessão + equilíbrio) → P-03 Seção 7.2 (dupla tarefa adaptada). |
| **P-07** | Quedas e Síndrome Pós-Queda | P-08 (Sarcopenia — fraqueza muscular é fator de risco muscular primário para queda; dosagem de resistência via P-08 Seção 6.3), P-04 (Osteoporose — fratura risk amplifica consequências de queda; restrições de carga via P-04 Seção 5.2), P-01 (OA — dor e rigidez articular comprometem equilíbrio), P-05 (Fratura de Fêmur — prevenção de queda recorrente mandatória pós-fratura), P-06 (Parkinson — instabilidade postural e freezing de marcha), P-03 (AVC — hemiparesia afeta equilíbrio bilateral e marcha), P-10 (ATJ — déficit de equilíbrio pós-operatório e propriocepção reduzida), P-11 (ATQ — risco de queda combinado com precauções de luxação), P-18 (Demência — comprometimento cognitivo afeta dupla tarefa e segurança de sessão), P-17 (Neuropatia Periférica Diabética — perda sensorial compromete propriocepção e reflexo protetivo de queda) | **DOIS modificadores cruzados de P-07:** (1) **Hierarquia de equilíbrio:** Tabela INFRAESTRUTURA DE SEGURANÇA — HIERARQUIA DE INTERVENÇÃO DE EQUILÍBRIO em P-07 Seção 7.2 — referência normativa para todos os protocolos neuromotores e de fragilidade (P-03, P-05, P-06, P-08, P-10, P-11, P-18). 4 níveis (Estático/Dinâmico/Dupla Tarefa/Perturbação) com critérios objetivos TUG/SPPB/BBS de entrada e saída. Citar: "Progressão de equilíbrio conforme P-07, Seção 7.2." (2) **Protocolo de sessão:** Template INFRAESTRUTURA DE SEGURANÇA — PROTOCOLO DE RISCO DE QUEDA POR SESSÃO em P-07 Seção 5.2 — template reutilizável para todos os protocolos com pacientes de risco de queda (TUG > 13,5 seg OU FES-I-BR ≥ 23 OU ≥ 1 queda no último ano). 4 elementos: VAS fadiga pré-sessão + PA ortostática + cinto por TUG + saída supervisionada. Citar: "Aplicar Protocolo de Risco de Queda por Sessão conforme P-07, Seção 5.2." | Avaliação da síndrome pós-queda (tríade completa: medo de cair + restrição de atividade + perda funcional progressiva) mandatória — não reduzir a apenas "medo de cair". FES-I-BR ≥ 31 = escalamento obrigatório a psicólogo/geriatra antes de progressão hierárquica. STOPPFall: rastreamento de medicamentos de risco para queda em todo paciente com ≥ 4 medicamentos psicoativos ou combinação benzodiazepínico + opioide + anti-hipertensivo (O'Mahony D et al. Age Ageing 2021; PubMed 34651149). Cadeia de modificadores: P-04 define teto de carga óssea (prioridade 1) → P-08 define parâmetros de resistência (prioridade 2) → P-07 define progressão de equilíbrio e segurança de sessão (normativo para Fases 4-8). |
| **P-08** | Sarcopenia / Fraqueza Muscular Generalizada | P-04 (Osteoporose — osteosarcopenia), P-01 (OA — fraqueza potencializa carga articular), P-05 (Fratura de Fêmur — sarcopenia retarda reabilitação), P-07 (Quedas — sarcopenia é fator de risco muscular primário), P-10 (ATJ), P-11 (ATQ) | **Dosagem de resistência:** Tabela Modificador Transversal em P-08 Seção 6.3 — todos os protocolos que abordam exercício resistido em sarcopenia devem citar esta tabela. Estratificação por Fragilidade (Fried): Robusto 65% 1RM / 3 séries / 8–12 reps / 3×sem; Pré-frágil 50% 1RM / 2–3 séries / 8–12 reps / 2–3×sem; Frágil 35% 1RM / 2 séries / 6–10 reps / 2×sem. Duração mínima: 12 semanas. | EWGSOP2 FACS — gravidade (Grave = gait < 0,8 m/s ou SPPB ≤ 8 ou TUG > 20 seg) reduz carga inicial adicional em 20% na faixa Frágil; encaminhamento ao nutricionista obrigatório quando ingestão proteica < 1,0 g/kg/dia, IMC < 22 ou sarcopenia grave; coordenar com P-04 em osteosarcopenia |
| **P-09** | Artrose de Coluna / Espondilose | P-04 (Osteoporose — MODIFICADOR TRANSVERSAL obrigatório via P-04 Seção 5.2 quando T-score ≤ -2,5; bone-loading constraint governa extensão com carga; extensão é recomendada mas teto de carga governa); P-07 (Quedas — P-07 Seção 5.2 protocolo de sessão quando TUG > 13,5 seg; P-07 Seção 7.2 hierarquia de equilíbrio); P-08 (Sarcopenia — dosagem de resistência P-08 Seção 6.3 quando dinamometria < EWGSOP2); P-02 (diagnóstico diferencial — estenose com claudicação neurogênica predominante); P-12 (diagnóstico diferencial — DLC inespecífica quando substrato não explica carga de dor) | Fragilidade (Fried); AINEs crônicos; bifosfonatos (sinergia com exercício resistido — comunicar ao paciente); betabloqueadores (usar RPE exclusivo); corticosteroides crônicos (ativar P-04 Seção 5.2) | **Extensão vertebral RECOMENDADA** em P-09 (inversão terapêutica em relação a P-02 onde é contraindicada) — suspensa apenas quando P-04 Muito Alto Risco com teto de carga ultrapassado. **Hip hinge:** padrão universal em todos os movimentos. **Claudicação instalada durante tratamento:** suspender P-09 → reavaliação de imagem → redirecionar para P-02. **CSI-BR ≥ 40:** progressão tempo-contingente ativa; PNE adjunto (conteúdo: "artrose não é ruína — imagem não determina dor"). **Cauda equina:** menos frequente que P-02 mas possível — SAMU 192 + NÃO MOBILIZAR. **Cadeia de modificadores:** P-04 Seção 5.2 (prioridade 1 — governa carga de extensão) → P-08 Seção 6.3 (prioridade 2) → P-07 Seções 5.2+7.2 (prioridade 3). |
| **P-10** | Pós-op Artroplastia Total de Joelho (ATJ) | P-01 (OA — condição subjacente; desfecho compartilhado WOMAC-BR), P-04 (Osteoporose — restrições de carga óssea se T-score ≤ -2,5; citar P-04 Seção 5.2), P-08 (Sarcopenia — dosagem de resistência; citar P-08 Seção 6.3), P-07 (Quedas — déficit de equilíbrio e propriocepção pós-op; citar P-07 Seções 5.2 e 7.2), P-05 (Fratura de Fêmur — fratura contralateral ou prévia; CFS pode ser necessário), P-11 (ATQ — diferenciação de escopo; artroplastia bilateral simultânea exige atenção especial), P-06 (Parkinson — queda + rigidez pós-op), P-18 (Demência — desafios de adesão e compliance pós-op) | **Vigilância de síndrome compartimental (5 Ps):** Sinal de alarme específico pós-ATJ — dor desproporcional ao movimento passivo (especialmente dorsiflexão de tornozelo), pressão compartmental, palidez, parestesia, paralisia. Bloqueio epidural pode mascarar dor (PubMed 16498006). 2 ou mais sinais = emergência cirúrgica. **Metas de ROM:** Flexão ≥ 90° por 6 semanas; ≥ 120° por 12 semanas. Extensão = 0° (déficit completo é falha terapêutica). **Lag de quadríceps:** monitorar incapacidade de extensão ativa dos últimos 15° contra gravidade. **Escopo:** ATJ primária apenas — diferenciada de P-11 (ATQ); revisão de ATJ necessita adaptação. |
| **P-11** | Pós-op Artroplastia Total de Quadril (ATQ) | P-01 (OA — condição subjacente; desfecho compartilhado WOMAC-BR), P-04 (Osteoporose — restrições de carga óssea; citar P-04 Seção 5.2; bifosfonatos + exercício resistido sinérgicos — comunicar ortopedista), P-08 (Sarcopenia — dosagem de resistência; citar P-08 Seção 6.3), P-07 (Quedas — risco de queda pós-artroplastia + precauções de luxação restringem movimentos protetivos; citar P-07 Seções 5.2 e 7.2), P-05 (Fratura de Fêmur — hemiartroplastia por fratura redirecionada para P-05; coxartrose frequentemente coexistente em pacientes de P-05), P-10 (ATJ — diferenciação de escopo; ATQ e ATJ em contexto bilateral exigem protocolos paralelos), P-06 (Parkinson — alta comorbidade ATQ/Parkinson; instabilidade postural aumenta risco de luxação recorrente), P-18 (Demência — adesão às precauções de luxação crítica; envolver cuidador obrigatoriamente) | **Precauções de luxação abordagem-dependente:** Verificar abordagem cirúrgica ANTES de iniciar qualquer exercício de ROM de quadril. Posterior: evitar flexão > 90°, adução, rotação interna (evidência 2024 questiona necessidade — PMC11651519; conduta: seguir orientação cirúrgica). Anterior Direto: evitar extensão além de neutro, rotação externa excessiva. Anterolateral: mínimas precauções; monitorar déficit de glúteo médio (nervo glúteo superior em risco). Precauções NÃO se relaxam automaticamente — clearance cirúrgico documentado obrigatório. **Déficit de abdutores:** Força de glúteo médio e sinal de Trendelenburg monitorados em todas as fases. **Discrepância de comprimento:** Medida funcional na admissão; > 1 cm = comunicar ortopedista. **Escopo:** ATQ primária por qualquer abordagem — diferenciada de P-10 (ATJ) e P-05 (hemiartroplastia por fratura). |
| **P-12** | Dor Lombar Crônica Inespecífica | P-02 (diagnóstico diferencial — estenose canal; substrato estrutural suficiente redireciona para P-02); P-09 (diagnóstico diferencial — espondilose mecânica com correlação anatômica redireciona para P-09); P-04 (Osteoporose coexistente — P-04 Seção 5.2 quando T-score ≤ -2,5); P-07 (Quedas — P-07 Seção 5.2 quando TUG > 13,5 seg; P-07 Seção 7.2 hierarquia de equilíbrio); P-08 (Sarcopenia — P-08 Seção 6.3 quando dinamometria < EWGSOP2); P-19 (diagnóstico diferencial — fratura vertebral quando dor aguda em osteoporótico) | Fragilidade (Fried); opioides (maior risco de uso crônico inadequado nesta população — documentar + comunicar médico); gabapentinoides (sedação + queda); antidepressivos (hipotensão ortostática); benzodiazepínicos (queda + AGS Beers); betabloqueadores (RPE exclusivo) | **PNE é o componente CENTRAL** (não adjunto) — protocolo de 4 módulos de 30–40 min cada; exercício sem PNE não é P-12. **CSI-BR ≥ 40:** progressão tempo-contingente obrigatória; graded exposure integrado. **HADS ≥ 11:** referência psicológica antes de progressão de fase. **PCS-BR ≥ 30:** reforçar PNE intensivo + referência psicológica. **Opioides:** grupo de maior risco de inadequação de tratamento — rastrear e comunicar. **Diferença de P-02/P-09:** substrato estrutural ausente ou desproporcional à carga de dor — classificação IASP de Dor Crônica Primária como ponto de partida. |
| **P-13** | Síndrome do Ombro Doloroso | P-04 (Osteoporose — modificador de carga óssea P-04 Seção 5.2 quando T-score ≤ -2,5; cautela em extensão de coluna torácica durante exercício overhead); P-08 (Sarcopenia — dosagem de resistência P-08 Seção 6.3 quando dinamometria < EWGSOP2); P-07 (Quedas — P-07 Seção 5.2 quando TUG > 13,5 seg; exercícios em pé requerem avaliação de equilíbrio); P-11 (ATQ — durante reabilitação de quadril, exercícios de ombro em cadeia cinética fechada upper limb podem ser utilizados como complemento quando limitação de MMII impede exercício convencional — comunicar fisioterapeuta principal); P-09 (Artrose de coluna — radiculopatia cervical pode simular ombro doloroso; realizar screening cervical obrigatório — Spurling, distração cervical); P-01 (OA glenoumeral coexistente — se confirmada, P-01 como comodificador); P-15 (DPOC — SpO₂ monitorar durante exercícios de ombro acima de 90°); P-16 (IC — RPE exclusivo; evitar isométricos de alta intensidade sem controle de PA) | Fragilidade (Fried); corticosteroides injetáveis CSI (janela de exercício 2–3 dias; max 3×/ano; NICE NG228 — não standalone); AINEs tópicos (primeira linha preferida em idosos); betabloqueadores (RPE exclusivo); anticoagulantes (mobilização agressiva — monitorar hematoma periarticular); gabapentinoides (sedação + queda — timing de sessão) | **Origem cardíaca em ombro esquerdo:** EXCLUIR SEMPRE antes de iniciar P-13 — dor de SCA pode manifestar-se como dor em ombro esquerdo; verificar caráter + fatores de piora + FR cardiovasculares. **CSI-BR ≥ 40:** progressão tempo-contingente; PNE adjunto obrigatório. **Ruptura completa com pseudoparalisia** (incapacidade de elevar > 45°): suspender P-13 → ortopedia — candidatura cirúrgica a avaliar. **Capsulite Estágio I:** NUNCA mobilização forçada além do limiar de dor — deslizamento grau I–II apenas. **Radiculopatia cervical:** screening obrigatório (Spurling + distração) para diferenciação de fonte de dor antes de iniciar. **Lesões assintomáticas de manguito:** prevalência crescente com idade (10% em 60–70 anos → 30% em > 80 anos) — educação do paciente obrigatória; ruptura assintomática com função preservada NÃO é indicação cirúrgica. |
| **P-14** | Disfunção do Assoalho Pélvico | **P-07** (Quedas — incontinência de urgência aumenta risco de queda por pressa ao banheiro; FES-I-BR ≥ 23 = ativar P-07 Seção 5.2; TUG > 13,5 s = cinto pélvico em exercícios de pé); **P-08** (Sarcopenia pélvica — Oxford ≤ 2 + dinamometria < 16 kg = reduzir carga PFMT em 20% + eletroestimulação passiva complementar; consultar P-08 Seção 6.3 para resistência periférica coexistente); **P-04** (Osteoporose — precauções de carga óssea em exercícios de solo e resistidos; P-04 Seção 5.2 quando T-score ≤ -2,5; hip hinge universal em exercícios posturais); **P-18** (Demência — MMSE < 24 = instrução proprioceptiva manual substitui instrução verbal; MMSE < 18 = eletroestimulação passiva como intervenção principal; cuidador obrigatório) | **Passo 0 Estrutural OBRIGATÓRIO** (classificação hipertônico vs. hipotônico vs. misto ANTES de qualquer exercício — ABRAFISM 2025, PMC11847513): Modified Oxford Grading Scale + PERFECT Scheme + palpação digital vaginal. **PFMT (Kegel) CONTRAINDICADO em hipertônico** — piora hipertonia, aumenta dor, agrava retenção. **Down-training** (hipertônico): respiração diafragmática + relaxamento progressivo + biofeedback de inibição. **ICIQ-SF-BR** (PMID 15243675) como desfecho primário — MCID ≥ 3 pontos (MEDIUM confidence). **Fase 3 PERMANENTE:** DAP em idosas é crônica; alta clínica = HEP autônomo com revisão trimestral. **Rastreio cognitivo:** MMSE < 24 = instrução adaptada obrigatória. Diretrizes primárias: Cochrane PFMT (Dumoulin 2018, PMC5756818, Nível A); ICS/IUGA 2010; ABRAFISM 2025. NÃO COBRE: prolapso com indicação cirúrgica (grau III–IV POP-Q), fístula urogenital, homens pós-prostatectomia, ITU ativa. | **Kegel para hipertônico = erro clínico grave (iatrogenic worsening):** Passo 0 Estrutural é a proteção — classificar SEMPRE antes de prescever. **Incontinência de urgência + pressa ao banheiro:** risco de queda elevado — checar FES-I-BR; FES-I-BR ≥ 23 = ativar P-07 Seção 5.2 obrigatoriamente. **Piora progressiva de dor pélvica em 12 semanas** de protocolo correto = revisão diagnóstica completa (cistometria, urodinâmica, avaliação especializada). **Hematúria macroscópica:** suspender protocolo → urologia urgente — exclusão de neoplasia urotelial. **MMSE < 24 = instrução adaptada obrigatória;** PFMT ativa contraindicada quando MMSE < 18 por incapacidade de isolamento muscular — eletroestimulação passiva como alternativa primária. **Cadeia de modificadores:** P-04 Seção 5.2 (carga óssea) → P-08 Seção 6.3 (sarcopenia pélvica) → P-07 Seções 5.2 + 7.2 (queda por urgência + segurança de sessão). |
| **P-15** | DPOC | P-01 (OA — limitação de mobilidade coexistente; dor articular governa carga), P-04 (Osteoporose — ICS crônico aumenta risco de perda óssea; ativar P-04 Seção 5.2 quando T-score ≤ -2,5), P-07 (Quedas — descondicionamento + fraqueza + dispneia = risco elevado; citar P-07 Seção 5.2 quando TUG > 13,5 s), P-08 (Sarcopenia — prevalência > 25% em DPOC grave; citar P-08 Seção 6.3 quando dinamometria < EWGSOP2), P-10 (ATJ — coexistência frequente em idosos; limitação funcional aeróbica + reabilitação pós-op), P-11 (ATQ — idem P-10), P-16 (IC — comodificador quando IC coexistente: RPE, peso diário, temperatura; P-15 é base quando DPOC é diagnóstico primário), P-18 (Demência — comprometimento cognitivo afeta aderência ao HEP e monitoramento de SpO₂ domiciliar), P-03 (AVC — cluster cardiorrespiratório pode coexistir com sequela neuromotora; monitoramento SpO₂ durante treino funcional), P-06 (Parkinson — disfunção autonômica + descondicionamento cardiorrespiratório; SpO₂ durante exercício relevante) | **SpO₂ mandatória:** Monitoramento de SpO₂ a cada 5 min durante exercício aeróbico; SpO₂ ≤ 90% = NÃO INICIAR; SpO₂ < 88% = parada imediata. **Borg Dispneia 0–10:** Instrumento primário de intensidade (alvo 4–6). **Template Universal Seção 11 (SHARED-FOUNDATION Seção 7.4):** P-15 estabelece o template de Precauções Cardiorrespiratórias usado em todos os 20 protocolos — subseções 11.1 (pré-sessão) e 11.2 (parada imediata) são universais; 11.3–11.5 são específicas do diagnóstico. **TC6M como desfecho primário:** MCID 25–30 m; equação Britto 2013 BR. **GOLD 2025 + ATS 2023 (PMID 37581410)** como diretrizes primárias. NÃO COBRE: asma não-DPOC, exacerbação aguda, IC como diagnóstico primário (→ P-16), HP severa (PAP > 55 mmHg). Instrumentos: TUG, SPPB-BR, Dinamometria, TC6M (ATS 2002), mMRC, CAT, Borg Dispneia 0–10, SpO₂. | **Dessaturação silenciosa:** DPOC moderada-grave pode ter SpO₂ < 88% sem dispneia proporcional — oximetria objetiva é mandatória, não negociável. **Exacerbação:** Critérios de Anthonisen (aumento de escarro + cor + dispneia) = SUSPENDER PR por 28 dias. **ICS crônico + ≥ 60 anos:** Ativar P-04 Seção 5.2 (osteoporose) + P-08 Seção 6.3 (sarcopenia) simultaneamente. **DPOC + IC coexistente:** P-15 como base (DPOC é diagnóstico primário) + modificadores P-16 (peso diário, RPE, temperatura). **Cadeia de modificadores:** P-04 Seção 5.2 (se osteoporose) → P-08 Seção 6.3 (se sarcopenia) → P-07 Seções 5.2+7.2 (se TUG > 13,5 s) → P-16 (se IC coexistente). |
| **P-16** | Insuficiência Cardíaca / Cardiopatias | P-01 (OA — artropatia coexistente frequente; cicloergômetro preferencial quando dor articular limita caminhada), P-04 (Osteoporose — corticosteroides crônicos em IC aumentam risco de perda óssea; citar P-04 Seção 5.2), P-07 (Quedas — anticoagulantes + hipotensão ortostática = risco elevado; citar P-07 Seção 5.2 quando TUG > 13,5 s), P-08 (Sarcopenia — prevalência > 20% em IC moderada-grave; citar P-08 Seção 6.3 quando dinamometria < EWGSOP2), P-10 (ATJ — coexistência frequente; cicloergômetro e precauções de ROM compatíveis com reabilitação cardíaca), P-11 (ATQ — precauções de luxação + hipotensão ortostática; anticoagulantes comuns em IC), P-15 (DPOC — comodificador quando DPOC coexistente: Borg Dispneia, SpO₂ contínua; P-16 é base quando IC é diagnóstico primário), P-18 (Demência — comprometimento cognitivo afeta protocolo de peso diário; cuidador como responsável pelo monitoramento), P-06 (Parkinson — disautonomia autonômica em DP + IC; hipotensão ortostática amplificada), P-05 (Fratura de Fêmur — anticoagulação em IC e reabilitação pós-fratura; risco de sangramento em queda) | **RPE Borg 6–20 EXCLUSIVO:** FC CONTRAINDICADA como parâmetro de intensidade em IC com betabloqueador. Betabloqueadores causam cronotropia negativa — FC embotada. Usar RPE 6–20 exclusivamente (alvo 11–13 Robusto; 10–11 Frágil/NYHA III). **Peso diário obrigatório:** Protocolo de pesagem (manhã, mesma balança) + limiares: ≥ 1,5 kg/24h e ≥ 2 kg/3 dias = SUSPENDER + contatar médico. **Termorregulação:** Temperatura ambiente ≤ 22°C ideal; máx 26°C; > 30°C sem AC = suspender. Hidratação pré-sessão 200 mL (se sem restrição hídrica). **IC-FEr vs IC-FEp:** Ambas cobertas — IC-FEp por AHA Scientific Statement 2023 (CIR.0000000000001122). **Template Universal Seção 11 (herdado de P-15):** P-16 herda subseções 11.1 e 11.2 do template P-15 + adapta 11.3–11.5 com modificadores IC-específicos. Instrumentos: TUG, SPPB-BR, Dinamometria, NYHA, MLHFQ (MCID ≥ 5 pts), RPE Borg 6–20, PA, FC repouso, Peso, Edema, TC6M (desfecho secundário). Diretrizes primárias: AHA/ACC/HFSA 2022 (CIR.0000000000001063); AHA Scientific Statement IC-FEp 2023 (CIR.0000000000001122); Diretriz BR Reab. Cardiovascular 2020 (PMC8387006). NÃO COBRE: IC aguda descompensada, NYHA IV instável, DPOC como diagnóstico primário (→ P-15). | **FC embotada por betabloqueador:** FC repouso ≤ 50 bpm = suspender sessão + contatar cardiologista. FC durante exercício é dado observacional de SEGURANÇA, nunca alvo de prescrição. **Valsalva PROIBIDO:** Expiração contínua obrigatória em todos os exercícios resistidos. **Descompensação:** Ganho ≥ 2 kg/3 dias ou ≥ 1,5 kg/24h + edema + ortopneia = SUSPENDER PR; avaliação cardiológica obrigatória antes de retorno. **AINEs CONTRAINDICADOS:** Precipitam retenção hídrica e descompensação — preferir paracetamol. **Digoxina:** FC artificialmente baixa por efeito cronotrópico negativo — RPE exclusivamente. **Cadeia de modificadores:** P-04 Seção 5.2 (se osteoporose por corticosteroide) → P-08 Seção 6.3 (se sarcopenia) → P-07 Seções 5.2+7.2 (se TUG > 13,5 s ou anticoagulante) → P-15 (se DPOC coexistente). |
| **P-17** | Neuropatia Periférica Diabética | **P-07** (Quedas — OBRIGATÓRIO em TODOS os pacientes com NPD; risco de queda 15× elevado em relação à população geriátrica sem neuropatia; hierarquia sensorial SE-1 a SE-4 fundamentada em P-07 Seção 7.2; protocolo de sessão P-07 Seção 5.2 verbatim em todas as fases); **P-08** (Sarcopenia e amiotrofia distal — dinamometria < 27 kg H / < 16 kg M = consultar P-08 Seção 6.3; NPD motora causa amiotrofia intrínseca do pé e distal de tornozelo; reduzir carga inicial em 20% adicional ao modificador Fried); **P-04** (Osteoporose — DM aumenta risco de perda óssea; P-04 Seção 5.2 quando osteoporose confirmada por densitometria; teto de carga governa progressão resistida); **P-01** (OA coexistente — dor articular governa carga); **P-16** (Neuropatia autonômica cardíaca — FC embotada; RPE Borg 6–20 como monitor exclusivo de intensidade; mesma lógica de P-16 com betabloqueador) | **Infraestrutura de segurança NÃO-NEGOCIÁVEL pré-sessão:** (1) Verificação glicêmica capilar — < 90 mg/dL = não iniciar (snack + reavaliar); 90–250 = iniciar normalmente; 250–300 sem cetonúria = baixa intensidade + glicemia a cada 20 min; > 300 ou cetonúria = não iniciar (Colberg 2016, PMC6977405; nota MEDIUM confidence); (2) Inspeção de pés bilateral ANTES de cada sessão — não delegável ao paciente; úlcera ativa = suspender exercício em ortostatismo (ADA 2025 Standards Section 12); (3) Calçado adequado OBRIGATÓRIO em TODAS as atividades — NUNCA descalço. **Hierarquia sensorial SE-1 a SE-4** (adaptação de P-07 Seção 7.2 para NPD): SE-1 = visão como canal substituto à propriocepção (superfície firme + olhos abertos); SE-2 = foam pad baixa densidade MAX (NUNCA wobble board, BOSU ou disco de equilíbrio); SE-3 = dupla tarefa sobre superfície FIRME (NUNCA instável + dupla tarefa simultâneas em NPD); SE-4 = ambiente externo com supervisão direta. **RPE Borg 6–20 exclusivo** quando neuropatia autonômica — FC blunted pelo mesmo mecanismo de P-16 com betabloqueador. Diretrizes primárias: ADA 2025 Standards Section 12; Colberg 2016 (PMC6977405); PMC12069999; PMC12167735. NÃO COBRE: neuropatia não-diabética (alcoólica, urêmica, paraneoplásica), túnel do carpo, úlcera ativa (→ pé diabético), HbA1c > 10% sem acompanhamento. | **Hipoglicemia com neuropatia autonômica = risco silencioso:** resposta adrenérgica (tremor, sudorese, taquicardia) pode estar abolida — hipoglicemia se manifesta diretamente como confusão ou perda de consciência. Verificação glicêmica pré-sessão não é negociável. **Úlcera de pé diabético (qualquer grau Wagner)** durante tratamento = suspender exercício em ortostatismo imediatamente → equipe de pé diabético. **HbA1c > 10% sem acompanhamento médico ativo** = contraindicação relativa — aguardar estabilização + início de acompanhamento. **Foam pad máxima instabilidade em SE-2:** NUNCA wobble board ou BOSU em NPD moderada-grave — perda de sensibilidade protetora plantar torna superfícies altamente instáveis iatrogênicas (risco de úlcera oculta por trauma de pressão). **Dupla tarefa (SE-3): NUNCA sobre superfície instável** — canal proprioceptivo periférico comprometido + atenção dividida supera capacidade compensatória vestibular-visual. **FES-I-BR ≥ 31:** integrar componente de síndrome pós-queda (P-07 Seção 5.3). **Cadeia de modificadores:** P-04 Seção 5.2 (osteoporose — prioridade 1) → P-08 Seção 6.3 (amiotrofia distal/sarcopenia — prioridade 2) → P-07 Seções 5.2 + 7.2 OBRIGATÓRIO (equilíbrio + sessão — prioridade 3). |
| **P-18** | Demência / Alzheimer (leve a moderado) | P-01 (OA — artropatia coexistente frequente; PAINAD-BR ajuda identificar dor não comunicada), P-03 (AVC — cluster neuromotor compartilhado; TEMPLATE CLUSTER NEUROMOTOR — P-03 Seção 7.2 referenciado por P-18 Fase 3 com adaptações de instrução cognitiva), P-04 (Osteoporose — risco de fratura aumentado em demência; ativar P-04 Seção 5.2; fratura silenciosa frequente), P-05 (Fratura de Fêmur — delirium pós-fratura em 35–65% dos idosos; desafios de adesão; PAINAD-BR mandatório pós-operatório), P-06 (Parkinson — DLB / demência de Parkinson; co-gerenciar P-06 + P-18; timing de levodopa + instrução adaptada simultâneos), P-07 (Quedas — comprometimento cognitivo é fator de risco independente para queda; P-07 Seção 5.2 adaptada para MMSE < 18 com cuidador presente; P-07 Seção 7.2 hierarquia de equilíbrio), P-08 (Sarcopenia — sarcopenia frequente em demência por inatividade e subnutrição; dosagem resistida via P-08 Seção 6.3), P-10 (ATJ — adesão às restrições de ROM comprometida; cuidador deve ser treinado), P-11 (ATQ — adesão às precauções de luxação crítica; cuidador obrigatório na instrução; envolvimento desde admissão) | **Sistema de Instrução Adaptada ao MMSE-BR (Seção 5.3):** 4 estratos (≥ 24, 20–23, < 24, < 18) — técnica de instrução diferenciada obrigatória em cada sessão; fundamentado em aprendizagem procedimental/implícita preservada em Alzheimer (Kalbe 2007). **Política de HEP Pictográfico:** MMSE < 24 = formato pictográfico MANDATÓRIO; máximo 3 exercícios (MMSE 20–23) ou 2 exercícios (MMSE < 18); imagem + símbolo de frequência + ZERO texto descritivo. **Cuidador como co-terapeuta:** Identificação obrigatória na admissão; presença em TODAS as sessões quando MMSE < 18; 3 sessões formais de treinamento de cuidador integradas ao protocolo. **PAINAD-BR:** Instrumento primário de dor para MMSE < 18 ou comunicação verbal comprometida (PubMed 25993063); aplicado em TODAS as sessões para este estrato. **TEMPLATE CLUSTER NEUROMOTOR (Fase 3):** Referência a P-03 Seção 7.2 com adaptações P-18 — tarefa cognitiva FAMILIAR e PROCEDIMENTAL; NUNCA aritmética ou fluência verbal para MMSE < 20. **Consistência de rotina:** Mesmo horário, mesmo espaço, mesmo terapeuta — componente terapêutico, não operacional. Diretrizes primárias: NICE NG97 (2018) + PMC12599043 (2025). NÃO COBRE: demência grave (MMSE < 10, CDR 3), delirium agudo, agitação não controlada. Instrumentos: TUG, SPPB-BR, Dinamometria, BBS-BR, FES-I-BR, MoCA-BR, MMSE-BR (estratificação), PAINAD-BR, CDR. | **Agitação psicomotora:** Causa orgânica obrigatória a excluir (dor oculta — PAINAD-BR, infecção, retenção urinária, constipação) antes de qualquer atribuição comportamental. **Deterioração cognitiva súbita** (MMSE ≥ 5 pontos em < 4 semanas) = emergência neurológica — delirium / AVC / infecção do SNC. **Precauções cirúrgicas (P-10/P-11):** Paciente com demência pode NÃO respeitar restrições de ROM/luxação — cuidador deve ser treinado nas precauções CIRÚRGICAS, não apenas nas de exercício. **Benzodiazepínicos:** AGS Beers potencialmente inapropriado — risco de queda elevado; advocar deprescrição com médico. **Abbey Pain Scale:** Validação cultural BR não confirmada — preferir PAINAD-BR. **Cadeia de modificadores:** P-04 Seção 5.2 (carga óssea) → P-08 Seção 6.3 (resistência) → P-07 Seções 5.2 + 7.2 (sessão + equilíbrio, adaptados ao MMSE) → P-03 Seção 7.2 (dupla tarefa com adaptação P-18). |
| **P-19** | Fraturas Vertebrais por Compressão | **P-04** (co-gerente OBRIGATÓRIO — P-04 Seção 5.2 governa TODOS os exercícios de P-19; fratura vertebral confirmada = classificação automática Muito Alto Risco; após alta de P-19 = continuar com P-04 para gestão crônica da osteoporose); P-07 (Quedas — P-07 Seção 5.2 protocolo de sessão OBRIGATÓRIO em todas as fases + P-07 Seção 7.2 hierarquia de equilíbrio quando TUG > 13,5 seg; maior risco de queda recorrente com nova fratura); P-08 (Sarcopenia — P-08 Seção 6.3 quando dinamometria < EWGSOP2; sarcopenia frequente no substrato da fratura por fragilidade); P-02 (diagnóstico diferencial — estenose canal sem fratura em DX diferencial de dor lombar aguda); P-09 (diagnóstico diferencial — artrose espinal sem fratura); P-12 (sensibilização central se dor > 3 meses além da recuperação estrutural) | Fragilidade (Fried — Fase Aguda: SEMPRE iniciar na faixa Frágil independente da pontuação de Fried); bifosfonatos/denosumab (sinérgicos com exercício resistido — comunicar ao paciente para motivação de aderência); opioides (risco de queda amplificado em idoso com fratura); corticosteroides crônicos (miopatia + perda óssea adicional — ativar P-04 Seção 5.2); AINEs (risco GI/renal na população frágil); betabloqueadores (RPE exclusivo) | **Flexão vertebral CONTRAINDICADA Fases 1 e 2** (Sinaki 1984, PubMed 6487063; P-04 Seção 5.2 Muito Alto Risco — regra absoluta). **Hip hinge:** padrão PERMANENTE em TODOS os movimentos de TODAS as fases. **Síndrome de cauda equina:** SAMU 192 + NÃO MOBILIZAR — mesmo protocolo de P-02. **Teto P-04:** verificar e documentar carga máxima para cada exercício. **Nova fratura durante P-19:** NRS súbito + nova perda de estatura + dor aguda em faixa = suspeita de nova fratura → suspender + ortopedia + RX/RNM. **P-04 após alta:** referência obrigatória para gestão crônica da osteoporose — P-19 não substitui P-04. **Cadeia de modificadores:** P-04 Seção 5.2 (governa todas as fases — prioridade 1) → P-08 Seção 6.3 (resistência) → P-07 Seções 5.2+7.2 (sessão + equilíbrio). |
| **P-20** | Gonalgia / Coxalgia Degenerativa (Conservador Definitivo) | P-01 (OA — diferenciação de escopo: P-20 = conservador definitivo; P-01 = pré-cirúrgico ou decisão em aberto; declínio rápido em P-20 = sinalizar médico para reconsiderar decisão cirúrgica); P-04 (Osteoporose — P-04 Seção 5.2 obrigatório verificar; evitar impacto alto em Alto/Muito Alto Risco FRAX; hip hinge em todos os movimentos); P-07 (Quedas — P-07 Seção 5.2 quando TUG > 13,5 seg; P-07 Seção 7.2 hierarquia de equilíbrio para treinamento proprioceptivo); P-08 (Sarcopenia — P-08 Seção 6.3 MANDATÓRIO verificar em TODOS os pacientes; sarcopenia frequente em OA avançada + inatividade crônica); P-10 (ATJ — se paciente aceitar cirurgia futuramente: redirecionar P-20 → P-01 → cirurgia → P-10); P-11 (ATQ — idem P-10 para coxalgia); P-05 (Fratura de Fêmur — risco aumentado em OA + osteoporose + queda; fratura muda rota para P-05); P-15 (DPOC — SpO₂ durante exercício aeróbico de MMII); P-16 (IC — RPE exclusivo se betabloqueador; peso diário + temperatura) | Fragilidade (Fried — obrigatório classificar); sarcopenia (P-08 obrigatório em TODOS); osteoporose (P-04 verificar em TODOS); betabloqueadores (RPE exclusivo — alta prevalência HAS + OA); AINEs tópicos (primeira linha em ≥ 75 anos — AGS Beers 2023); opioides (mascaramento completo de dor — NRS não confiável quando ativo); anticoagulantes (risco hematoma em queda — aplicar P-07 Seção 5.2) | **Diferenciação P-01:** declínio funcional rápido (WOMAC piora > 20% em 3 meses) OU falha conservadora > 12 meses = sinalizar médico para reconsiderar opção cirúrgica (retornar a P-01). **Fase 3 PERMANENTE:** não há "alta" convencional — HEP indefinido + revisão trimestral obrigatória + gerenciamento de expectativas formal. **WOMAC-BR como primário** (Oliveira 2022, PMC9673866); KOOS-BR/HOOS-BR secundários com cautela de validação. **Efusão articular aguda com calor:** SUSPENDER + excluir artrite séptica. **Trava mecânica súbita:** SUSPENDER + ortopedia. **P-08 obrigatório:** verificar sarcopenia em TODOS os pacientes P-20 — comorbidade frequente determinante da dosagem. **Bengala no lado CONTRALATERAL à dor de quadril** (reduz força de reação do solo no quadril ipsilateral). |

### 8.2 Cabeçalho da Matriz de Interações (Guia de Preenchimento)

Ao completar cada protocolo, preencher as células da linha correspondente conforme:

- **Interações Conhecidas:** Outros protocolos cujas condições frequentemente coexistem (ex: P-01 e P-04 coexistem frequentemente em mulheres pós-menopausa)
- **Modificadores Compartilhados:** Variáveis que afetam múltiplos protocolos (ex: fragilidade, sarcopenia, uso de corticosteroides)
- **Precauções Específicas:** Alertas cruzados — ex: "Se P-01 + P-16 coexistem, iniciar na faixa Frágil independente do SPPB"

---

## Questões Abertas e Verificações Pendentes

As seguintes questões foram identificadas durante a fase de pesquisa e devem ser verificadas antes da publicação definitiva de qualquer protocolo:

| # | Questão | Status | Recomendação Atual |
|---|---------|--------|-------------------|
| 1 | **Status OARSI 2024** — Houve publicação de nova diretriz pós-2019? | Não confirmado | Usar OARSI 2019 como diretriz vigente; tratar revisão de 2024 como contexto suplementar |
| 2 | **Status EWGSOP3** — Foi publicado EWGSOP3 (atualização de 2018)? | Não confirmado | Usar EWGSOP2 (2018); verificar imediatamente se EWGSOP3 anunciado |
| 3 | **AGS Beers 2025/2026** — Existe edição mais recente que 2023? | Não confirmado | Usar AGS Beers 2023; verificar antes de publicação definitiva |
| 4 | **Limiares NRS — documento IASP específico** | Não encontrado | Usar limiares baseados em prática estabelecida em RCTs; não citar como "diretriz IASP" |
| 5 | **ATS/ERS 2023 Pulmonary Rehabilitation Statement** — Status final | Resolvido | ATS CPG 2023 (PMID 37581410) adotado como diretriz primária para P-15 — substitui ATS/ERS 2013 Position Statement. Verificar adendos/corrigendum 2024–2026 antes de publicação definitiva. |

---

*Documento gerado em: 2026-03-12*
*Responsável pela atualização: Especialista em Validação de Protocolos de Reabilitação Geriátrica*
*Próxima revisão recomendada: 2026-09-12 (6 meses); exceções: OARSI e EWGSOP3 (verificar trimestralmente)*
