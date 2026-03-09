# Teste-AB-em-Marketing-Campanha-Simples-com-Grupo-de-Controle

📌 Visão Geral

Este projeto tem como objetivo analisar os resultados de um experimento de A/B Testing realizado em uma campanha de marketing digital. A análise busca verificar se a exibição de anúncios aumenta a taxa de conversão dos usuários em comparação com um grupo de controle.

Utilizando técnicas de Análise Exploratória de Dados (EDA) e testes estatísticos, avaliamos se a diferença observada entre os grupos é estatisticamente significativa e qual o impacto potencial da campanha em termos de conversões.

🎯 Problema de Negócio

Empresas frequentemente utilizam testes A/B para avaliar a eficácia de campanhas de marketing antes de implementá-las em larga escala.

Neste experimento, os usuários foram divididos em dois grupos:

Grupo Ad – usuários expostos ao anúncio

Grupo PSA – usuários que não visualizaram o anúncio (grupo de controle)

A análise busca responder:

O anúncio aumenta a taxa de conversão?

A diferença entre os grupos é estatisticamente significativa?

Qual o impacto potencial da campanha caso seja aplicada para todos os usuários?

📂 Fonte dos Dados

O conjunto de dados utilizado está disponível na plataforma:

Dataset: Marketing A/B Testing

Plataforma: Kaggle

O dataset contém informações sobre usuários participantes do experimento, incluindo:

Grupo do teste

Conversão

Dia e hora da exposição

Informações relacionadas ao experimento

🔎 Metodologia
1️⃣ Carregamento e compreensão dos dados

Importação das bibliotecas

Leitura do dataset

Análise da estrutura e tipos de dados

2️⃣ Limpeza e pré-processamento

Verificação de valores nulos

Identificação de inconsistências

Ajuste de tipos de variáveis

3️⃣ Análise Exploratória de Dados (EDA)

Distribuição dos usuários entre os grupos

Taxa de conversão por grupo

Visualização de padrões e comportamento dos dados

4️⃣ Análise estatística

Definição das hipóteses

Aplicação de testes estatísticos para comparação de proporções

Avaliação da significância estatística

5️⃣ Interpretação dos resultados

Comparação do desempenho dos grupos

Avaliação do impacto da campanha

Geração de insights e recomendações

📊 Principais Análises

Durante o projeto foram realizadas análises como:

Comparação da taxa de conversão entre os grupos

Avaliação da distribuição dos usuários no experimento

Aplicação de testes estatísticos para validação do resultado

Estimativa do impacto potencial da campanha

📈 Resultados e Insights

A análise permitiu identificar se o grupo exposto aos anúncios apresentou desempenho superior ao grupo de controle e se essa diferença é estatisticamente significativa.

Com base nos resultados obtidos, foi possível avaliar:

A eficácia da campanha publicitária

O impacto potencial na conversão de usuários

A viabilidade de implementação da estratégia em larga escala

🛠️ Ferramentas e Tecnologias

Python

Pandas

NumPy

Matplotlib / Seaborn

SciPy

Statsmodels

🚀 Possíveis Expansões do Projeto

Construção de modelos preditivos de conversão

Análise de segmentação de usuários

Simulação de impacto financeiro da campanha

Criação de dashboard interativo

# Teste A/B para Campanha de Marketing

## Objetivo
Avaliar se a campanha "ad" apresenta performance superior à campanha "psa" em termos de taxa de conversão.

---

### Pergunta de Negócio
A campanha tradicional ("ad") gera mais conversões do que a campanha alternativa ("psa")?

---

### Métrica Primária
Taxa de Conversão (Conversion Rate)

---

### Técnicas Aplicadas
- EDA
- Teste Z para proporções
- Qui-quadrado
- Intervalo de Confiança
- Tamanho de efeito (Cohen’s d)
- Regressão Logística
- ANOVA
