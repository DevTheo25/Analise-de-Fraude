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


# Modelagem
Nesta etapa, decidimos testar três modelos: **RandomForest**, **KNN** e **SVM**. Utilizamos **GridSearch** para treinar os modelos com vários parâmetros e identificamos os melhores parâmetros a serem utilizados para cada modelo.

## Modelo RandomForest
O Random Forest é um algoritmo que combina múltiplas árvores de decisão em um ensemble, onde cada árvore é treinada com uma amostra aleatória dos dados e as predições são feitas através da votação ou média das previsões de todas as árvores. Isso ajuda a reduzir overfitting e aumenta a robustez do modelo.

- Acurácia em Treinamento: 99.25%
- Tempo de Treinamento do Modelo:  353.9s
- Quantidade de treinamentos realizados:  324

## Modelo SVM
SVM, ou Support Vector Machine. Ele busca encontrar o hiperplano que melhor separa as classes no espaço de características, maximizando a margem entre as classes. O SVM é eficaz em espaços de alta dimensionalidade e pode lidar com conjuntos de dados complexos através do uso de funções de kernel para mapear os dados em espaços de características não lineares.

- Acurácia em Treinamento: 98.94%
- Tempo de Treinamento do Modelo:  100.31s
- Quantidade de treinamentos realizados:  192
  
## Modelo KNN
O KNN, ou k-Nearest Neighbors, é um algoritmo que classifica um ponto de dados com base na classe predominante entre seus vizinhos mais próximos em um espaço de características.

- Acurácia em Treinamento: 97.08%
- Tempo de Treinamento do Modelo:  24.82s
- Quantidade de treinamentos realizados:  120
  

