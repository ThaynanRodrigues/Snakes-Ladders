# Snakes and Ladders — Simulação Estatística e Análise de Probabilidades em R

Projeto de modelagem e simulação do jogo *Snakes and Ladders*, desenvolvido em R, com foco em validação lógica, análise estatística e geração de insights a partir de dados simulados.

---

## Visão Geral

Este projeto tem como objetivo analisar o comportamento do jogo Snakes and Ladders sob diferentes cenários, utilizando simulação computacional para estimar probabilidades, médias e padrões estruturais.

A abordagem combina modelagem matemática, validação de regras e análise exploratória para responder perguntas relevantes sobre dinâmica, aleatoriedade e equilíbrio do jogo.

---

## Objetivos

* Modelar o jogo de forma programática em R
* Validar a consistência das regras implementadas
* Simular milhares de partidas para análise estatística
* Avaliar o impacto de mudanças nas regras do jogo
* Identificar padrões e gerar insights interpretáveis

---

## Estrutura do Projeto

```
snakes-ladders/
│
├── slides.qmd              # Apresentação final (Quarto / RevealJS)
├── R/
│   ├── board.R             # Estrutura do tabuleiro (cobras e escadas)
│   └── simulate.R          # Funções de simulação
│
├── figs/                   # Gráficos e imagens
├── output/                 # Arquivos renderizados
└── README.md
```

---

## Modelagem do Problema

O tabuleiro foi representado como um sistema de transições entre casas:

* Escadas: avançam o jogador
* Cobras: fazem o jogador retroceder
* Regra de vitória: atingir ou ultrapassar a última casa

Toda a lógica foi encapsulada em funções reutilizáveis, permitindo simulação eficiente de múltiplos cenários.

---

## Metodologia

O projeto foi estruturado em quatro etapas principais:

1. Modelagem do tabuleiro
2. Validação das regras do jogo
3. Simulação de partidas (Monte Carlo)
4. Análise estatística dos resultados

Foram realizadas milhares de simulações por cenário para garantir estabilidade estatística das estimativas.

---

## Validações Implementadas

Antes da análise final, foram realizadas verificações para garantir a confiabilidade do modelo:

* Distribuição uniforme do dado
* Aplicação correta de cobras e escadas após o movimento
* Alternância correta de turnos entre jogadores
* Tratamento de casos de borda

  * vitória ao atingir ou ultrapassar a última casa
  * prevenção de estados inválidos
  * controle de loops

---

## Perguntas Investigadas

### Q1. Quem começa tem vantagem?

A simulação indicou que o jogador que inicia a partida possui uma leve vantagem estatística, com probabilidade de vitória acima de 50%.

---

### Q2. Qual a frequência de cobras e escadas?

As ocorrências de cobras e escadas são frequentes ao longo das partidas, mostrando que esses elementos são estruturais no comportamento do jogo.

---

### Q3. Qual o impacto de escadas com uso probabilístico (50%)?

Ao reduzir a efetividade das escadas, observou-se:

* aumento no número médio de jogadas
* maior variabilidade na duração das partidas

Isso evidencia o papel das escadas como mecanismo de aceleração do jogo.

---

### Q4. Como tornar o jogo mais equilibrado?

Foi realizada uma busca em duas fases para identificar a posição inicial do Jogador 2 que aproxima as probabilidades de vitória de 50%.

Pequenas alterações nas condições iniciais foram suficientes para neutralizar a vantagem do primeiro jogador.

---

### Q5. Qual o impacto de imunidade à primeira cobra?

Ao permitir que o Jogador 2 ignore a primeira cobra, observou-se alteração nas probabilidades de vitória, demonstrando sensibilidade do jogo a mudanças nas regras.

---

## Principais Insights

* Existe vantagem estrutural para quem começa
* A duração das partidas é relativamente estável, apesar da aleatoriedade
* Cobras e escadas impactam diretamente a dinâmica e variabilidade do jogo
* Reduzir a efetividade das escadas prolonga significativamente as partidas
* Pequenas mudanças nas regras podem alterar o equilíbrio do sistema

---

## Tecnologias Utilizadas

* R
* RStudio
* Quarto (RevealJS)
* tidyverse
* ggplot2
* knitr
* kableExtra

---

## Como Executar

1. Clone o repositório:

```bash
git clone <URL_DO_REPOSITORIO>
cd snakes-ladders
```

2. Abra o projeto no RStudio

3. Renderize a apresentação:

```bash
quarto render slides.qmd
```

---

## Apresentação

O projeto inclui uma apresentação desenvolvida em Quarto, com foco em:

* clareza metodológica
* validação do raciocínio
* visualização dos resultados
* comunicação de insights

---

## Autor

Thaynan Rodrigues

---

## Contato

* [LinkedIn](https://www.linkedin.com/in/thaynanrodrigues/)
* [GitHub](https://github.com/ThaynanRodrigues)
