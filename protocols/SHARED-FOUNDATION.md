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

### 7.4 Precauções Cardiorrespiratórias

**Avaliação Pré-Participação:**
Todo paciente idoso deve ter avaliação cardiovascular documentada antes de iniciar exercício de intensidade moderada a intensa. Verificar e registrar:
- PA basal (em repouso, sentado, após 5 minutos)
- FC de repouso
- História de ICC, DPOC, arritmias, angina, infarto prévio
- Saturação O₂ basal (se disponível)
- Medicamentos cardiovasculares em uso (ver Seção 7.3)

**Indicadores de Parada Imediata:**

| Indicador | Limiar |
|-----------|--------|
| Dor torácica, pressão precordial ou irradiação | Qualquer ocorrência |
| Dispneia súbita e desproporcional ao esforço | Qualquer ocorrência |
| Palpitações com tontura ou síncope | Qualquer ocorrência |
| PA sistólica durante exercício | > 200 mmHg |
| Queda de PA sistólica durante esforço progressivo | > 10 mmHg |
| Saturação O₂ (se oximetria disponível) | SpO₂ < 90% |

**Adaptações para Pacientes com ICC ou DPOC Conhecida:**
- Iniciar na faixa **Frágil** independentemente do escore de fragilidade obtido
- Sessões mais curtas: 15–20 minutos, com maior frequência semanal (3–5×/semana se tolerado)
- RPE ≤ 13 (Borg 6-20) como limite superior de esforço
- Sessões supervisionadas obrigatórias nas primeiras 4 semanas
- Oximetria de pulso durante exercício se disponível

---

## 8. Esqueleto do Índice de Referência Cruzada

> **Status:** A ser preenchido progressivamente à medida que cada protocolo é desenvolvido. Apenas a linha P-01 será parcialmente preenchida após a conclusão do Plano 01-02. As demais linhas representam um shell para preenchimento futuro.

### 8.1 Matriz de Interação entre Protocolos (Shell 20×20)

| Protocolo | Condição | Interações Conhecidas | Modificadores Compartilhados | Precauções Específicas |
|-----------|----------|----------------------|------------------------------|------------------------|
| **P-01** | Osteoartrite / Artrose | P-04 (Osteoporose), P-07 (Quedas), P-08 (Sarcopenia), P-10 (ATJ), P-11 (ATQ), P-20 (Gonalgia/Coxalgia) | Fragilidade, corticosteroides, AINEs, anticoagulantes | ICC/DPOC: iniciar na faixa Frágil; Corticosteroides crônicos: consultar P-04 antes de exercício de impacto; Sarcopenia confirmada: ajustar dosagem conforme P-08 |
| **P-02** | Lombalgia Crônica e Estenose de Canal | — | — | — |
| **P-03** | AVC/AVE (fase crônica) | — | — | — |
| **P-04** | Osteoporose | P-08 (Sarcopenia — osteosarcopenia), P-01 (OA — corticosteroides aceleram perda óssea), P-05 (Fratura de Fêmur — osteoporose é substrato), P-07 (Quedas — queda em osteoporótico = alto risco de fratura), P-09 (Artrose de Coluna — diferenciação de dor vertebral), P-10 (ATJ — T-score antes de carga pós-op), P-11 (ATQ — ONJ com bifosfonatos pré-cirurgia), P-16 (IC — corticosteroides crônicos), P-19 (Fraturas Vertebrais — P-04 é o protocolo de manutenção crônica após P-19) | **Restrições de carga óssea:** Tabela MODIFICADOR TRANSVERSAL em P-04 Seção 5.2 — todos os protocolos que abordam paciente com osteoporose ou risco de fratura devem citar esta tabela. 4 categorias de risco (Baixo/Médio/Alto/Muito Alto) × 3 eixos de restrição (flexão espinal / impacto / resistência). Regra geral espinal: extensão preferida sobre flexão em toda osteoporose (Sinaki 1984, PubMed 6487063). Hip hinge obrigatório em todos os movimentos. Para resistência em Muito Alto Risco ou osteosarcopenia: citar P-08 Seção 6.3 e aplicar teto de carga P-04 Seção 5.2. | Categoria de risco governa teto de carga em TODAS as fases — progressão de fase não elimina restrições. FRAX + T-score (não T-score isolado) para estratificação. Nova dor vertebral aguda durante tratamento = suspender imediatamente → ortopedia. Bifosfonatos + exercício resistido são sinérgicos (BHOF 2022) — comunicar sinergia ao paciente como motivação de aderência. Em osteosarcopenia: ativar co-tratamento P-04 + P-08 simultaneamente. |
| **P-05** | Fratura de Fêmur Proximal / Quadril | — | — | — |
| **P-06** | Doença de Parkinson | — | — | — |
| **P-07** | Quedas e Síndrome Pós-Queda | — | — | — |
| **P-08** | Sarcopenia / Fraqueza Muscular Generalizada | P-04 (Osteoporose — osteosarcopenia), P-01 (OA — fraqueza potencializa carga articular), P-05 (Fratura de Fêmur — sarcopenia retarda reabilitação), P-07 (Quedas — sarcopenia é fator de risco muscular primário), P-10 (ATJ), P-11 (ATQ) | **Dosagem de resistência:** Tabela Modificador Transversal em P-08 Seção 6.3 — todos os protocolos que abordam exercício resistido em sarcopenia devem citar esta tabela. Estratificação por Fragilidade (Fried): Robusto 65% 1RM / 3 séries / 8–12 reps / 3×sem; Pré-frágil 50% 1RM / 2–3 séries / 8–12 reps / 2–3×sem; Frágil 35% 1RM / 2 séries / 6–10 reps / 2×sem. Duração mínima: 12 semanas. | EWGSOP2 FACS — gravidade (Grave = gait < 0,8 m/s ou SPPB ≤ 8 ou TUG > 20 seg) reduz carga inicial adicional em 20% na faixa Frágil; encaminhamento ao nutricionista obrigatório quando ingestão proteica < 1,0 g/kg/dia, IMC < 22 ou sarcopenia grave; coordenar com P-04 em osteosarcopenia |
| **P-09** | Artrose de Coluna / Espondilose | — | — | — |
| **P-10** | Pós-op Artroplastia Total de Joelho (ATJ) | — | — | — |
| **P-11** | Pós-op Artroplastia Total de Quadril (ATQ) | — | — | — |
| **P-12** | Dor Lombar Crônica Inespecífica | — | — | — |
| **P-13** | Síndrome do Ombro Doloroso | — | — | — |
| **P-14** | Disfunção do Assoalho Pélvico | — | — | — |
| **P-15** | DPOC | — | — | — |
| **P-16** | Insuficiência Cardíaca / Cardiopatias | — | — | — |
| **P-17** | Neuropatia Periférica (diabética) | — | — | — |
| **P-18** | Demência / Alzheimer (leve a moderado) | — | — | — |
| **P-19** | Fraturas Vertebrais por Compressão | — | — | — |
| **P-20** | Gonalgia / Coxalgia Degenerativa | — | — | — |

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
| 5 | **ATS/ERS 2023 Pulmonary Rehabilitation Statement** — Status final | Não confirmado | Verificar antes de finalizar P-15 (Fase 6) |

---

*Documento gerado em: 2026-03-12*
*Responsável pela atualização: Especialista em Validação de Protocolos de Reabilitação Geriátrica*
*Próxima revisão recomendada: 2026-09-12 (6 meses); exceções: OARSI e EWGSOP3 (verificar trimestralmente)*
