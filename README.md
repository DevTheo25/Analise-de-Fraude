# Análise de Fraude em Empréstimos Financeiros
![img](https://github.com/DevTheo25/Analise-de-Fraude/assets/122491960/99f46c3f-0f04-4f5d-81d9-9d34e36f5b77)

## Introdução

Este projeto tem como objetivo principal desenvolver um modelo de machine learning capaz de identificar fraudes em empréstimos financeiros. Utilizando técnicas de análise de dados e modelagem preditiva, buscamos detectar padrões que possam indicar atividades fraudulentas em empréstimos financeiros.

---
# Análise Exploratória - Visão Geral
- O objetivo desta analise é ter uma visão geral do conjunto de dados, compreendendo seu tamanho, variaveis, tipo de dados e período dos dados coletados.

### Problemas Identificados:
- Colunas com valores nulos.
- Colunas com outliers.
- Colunas categóricas com alta variabilidade nos dados.
- Colunas com redundância nos dados.
- Colunas irrelevantes para o treinamento.

Após a visão geral dos dados, fizemos uma análise profunda dos dados, utilizando gráficos para visualizar a variabilidade de cada coluna e suas medidas estatísticas.


# Pré-processamento de Dados
Após a análise exploratória, iniciamos o pré-processamento dos dados para corrigir os problemas identificados:

- Tratamento de valores nulos: Substituímos os valores nulos pela mediana da coluna.
- Criação de colunas de faixas para remover os outliers, por exemplo: **Faixa_Etária**, **Faixa_Salarial**, **Faixa_Dias_Atraso**.
- Codificação de colunas categóricas para reduzir a alta variabilidade.
- Tratamento das colunas com dados redundantes.
- Exclusão de colunas irrelevantes para o treinamento.

# Engenharia de Recursos
Avançamos para a etapa de transformação dos dados, onde aplicamos algumas técnicas para preparar os dados para a modelagem:

- **Train_test_split:** Separando os dados entre dados de treino e dados de teste.
- **Label Encoding:** Convertendo variáveis categóricas em numéricas através de codificação.
- **SMOTE:** Balanceamento da coluna Target.
- **MinMaxScaler:** Escalando os dados para um intervalo entre 0 e 1.

  
Essas transformações são essenciais para garantir que os dados estejam em um formato adequado para os algoritmos de aprendizado de máquina.
---

# Modelagem

## Modelo
