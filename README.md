# TESTE A/B PARA CAMPANHA DE MARKETING

 <img src="https://github.com/Adriele-Cerqueira/TESTE-AB-EM-MARKETING/blob/main/Capa_AB.png" width="550">

![Python](https://img.shields.io/badge/Python-Data%20Science-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-orange)
![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-lightgrey)
![SciPy](https://img.shields.io/badge/SciPy-Statistical%20Testing-green)
![Statsmodels](https://img.shields.io/badge/Statsmodels-Statistical%20Modeling-red)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-yellow)
![Seaborn](https://img.shields.io/badge/Seaborn-Data%20Visualization-purple)


## Resumo Executivo

Este projeto teve como objetivo avaliar a eficácia de campanhas publicitárias digitais por meio de um experimento de **Teste A/B**, comparando as taxas de conversão entre dois grupos de usuários.  

---

## Problema de Negócio

Empresas frequentemente enfrentam desafios relacionados à **eficiência de campanhas de marketing digital e ao retorno sobre investimento em publicidade**.

Neste cenário, compreender **como diferentes estratégias de exposição a anúncios impactam a conversão de usuários** torna-se essencial para melhorar decisões estratégicas.

Este projeto busca responder à seguinte questão de negócio:

**A campanha tradicional ("ad") gera mais conversões do que a campanha alternativa ("psa")?**

---

## Fonte de Dados

Os dados utilizados neste projeto foram obtidos a partir de **um dataset público disponibilizado na plataforma Kaggle**.

O dataset contém informações relacionadas a:

- Identificação de usuários
- Grupo experimental (ad ou psa)
- Conversão do usuário
- Quantidade de anúncios visualizados
- Métricas de exposição à campanha

Após a coleta, os dados passaram por etapas de **limpeza, exploração e preparação** para permitir a análise estatística do experimento.

---

## Metodologia

### Preparação e exploração dos dados

- Coleta e importação dos dados para o ambiente de análise em Python  
- Análise exploratória de dados (EDA) para compreensão da distribuição das variáveis  
- Verificação da qualidade dos dados (valores nulos, inconsistências e estrutura do dataset)  
- Análise da distribuição dos grupos experimentais (ad vs psa)  
- Cálculo da taxa de conversão por grupo  

### Validação dos pressupostos estatísticos

Antes da aplicação dos testes de hipótese, foram avaliadas as suposições estatísticas necessárias para a escolha do método adequado.

- **Teste de normalidade (Shapiro-Wilk)** para verificar se os dados seguem distribuição normal  
- **Teste de homogeneidade de variâncias (Levene)** para avaliar igualdade das variâncias entre os grupos  

Os resultados indicaram que:

- Os dados **não seguem distribuição normal**
- As variâncias entre os grupos **não são homogêneas**

Dessa forma, **testes paramétricos tradicionais não são apropriados**, sendo mais adequado utilizar **testes de comparação de proporções**.

### Testes estatísticos aplicados

- Aplicação do **Teste Z para proporções** para comparar as taxas de conversão entre os grupos  
- Aplicação do **Teste Qui-quadrado de independência** para verificar associação entre grupo experimental e conversão  
- Cálculo do **intervalo de confiança (95%)** para as taxas de conversão  
- Cálculo do **tamanho do efeito (Cohen’s d)** para medir a magnitude da diferença observada  

### Modelagem estatística

- Aplicação de **regressão logística** para estimar o impacto da exposição ao anúncio na probabilidade de conversão.

### Interpretação dos resultados

- Avaliação da significância estatística dos testes  
- Interpretação dos resultados sob a perspectiva de **impacto de negócio e tomada de decisão em marketing**

---

## Skills e Ferramentas

### Linguagens

- Python  
- SQL  

### Bibliotecas

- Pandas  
- NumPy  
- Scikit-Learn  
- Matplotlib  
- Seaborn  
- SciPy  
- Statsmodels  

### Banco de Dados

- SQL / Oracle / PostgreSQL  

### Versionamento

- Git  
- GitHub  

---

## Resultados e Recomendações de Negócio

Inicialmente foi realizada uma **Análise Exploratória de Dados (EDA)** para compreender a distribuição das variáveis e comparar o desempenho entre os grupos experimentais (*ad* e *psa*). A análise revelou que **usuários expostos à campanha publicitária (grupo "ad") apresentaram taxa de conversão significativamente maior que o grupo de controle ("psa")**.

 <img src="https://github.com/Adriele-Cerqueira/TESTE-AB-EM-MARKETING/blob/main/Comparacao_Grupos.png" width="550">

Para confirmar essa hipótese, primeiramente foi avaliado os **pressupostos estatísticos** para escolha dos testes de hipótese. O **teste de normalidade de Shapiro-Wilk** indicou que os dados não seguem distribuição normal (p < 0.05), enquanto o **teste de Levene** apontou variâncias heterogêneas entre os grupos (p < 0.05).

Diante dessas características, foram aplicados testes adequados para **comparação de proporções**, incluindo o **Teste Z para proporções** e o **Teste Qui-quadrado de independência**. Os resultados indicaram **diferença estatisticamente significativa entre os grupos** (p-valor ≈ 1.7e-13), mostrando que a exposição aos anúncios está associada a uma maior taxa de conversão. 

Além disso, vamos verificar tamanho do efeito utilizando Cohen's d para medir a magnitude da diferença entre os grupos. O resultado foi d = 0.0528, indicando um efeito muito pequeno. 

Resumo dos principais resultados:

- Taxa de conversão **≈ 2,55% no grupo ad**
- Taxa de conversão **≈ 1,79% no grupo psa**
- Diferença **estatisticamente significativa (p < 0.001)** no Teste Z
- Associação confirmada pelo **teste Qui-quadrado**
- Regressão logística indica **44% mais chance de conversão** no grupo ad
- Tamanho do efeito pequeno (**Cohen's d = 0.052**)

Isso indica que **a exposição aos anúncios impacta positivamente a probabilidade de conversão**, porém o **impacto prático da diferença é relativamente pequeno**, sugerindo espaço para otimização da estratégia.

Com base nesses achados, recomenda-se:

- Direcionar estratégias para **otimizar campanhas publicitárias com maior potencial de conversão**
- Monitorar continuamente **taxas de conversão e ROI de campanhas**
- Utilizar **experimentos A/B testing de forma recorrente** para validar novas estratégias de marketing digital

Essas ações podem contribuir para **melhor alocação de investimento em mídia e aumento gradual da eficiência das campanhas**.

---

## Próximos Passos

- Desenvolver um **modelo preditivo de conversão de usuários**, identificando perfis com maior probabilidade de compra.  

- Realizar **novos experimentos A/B testando diferentes criativos, segmentações ou frequência de anúncios**.  

- Estimar o **impacto financeiro da diferença de conversão**, calculando a receita potencial gerada pelo aumento de conversões.
  
