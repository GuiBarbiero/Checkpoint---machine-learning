# Checkpoint de Machine Learning

## Integrantes
- Guilherme Barbiero — RM555185
- Marco Antonio Gonçalves — RM556818
- Vinicius Castro — RM556137
- Camila Mie Takara — RM555418
- Matheus Cantiere — RM558479

## Descrição do projeto
Este projeto foi desenvolvido como parte do checkpoint de Machine Learning, com o objetivo de aplicar na prática as principais etapas do pipeline de desenvolvimento de modelos de aprendizado de máquina.

A atividade propõe a construção de dois modelos:
- um modelo de **classificação**
- um modelo de **regressão**

O dataset escolhido foi o **Wine Quality Dataset**, utilizando a base de vinhos tintos. Esse conjunto de dados contém variáveis físico-químicas dos vinhos, como acidez, teor alcoólico, pH, densidade, entre outras, além da variável `quality`, que representa a nota de qualidade do vinho.

## Objetivo
O objetivo deste projeto é demonstrar, de forma prática, as etapas fundamentais de um pipeline de Machine Learning:
1. coleta e seleção dos dados
2. preparação dos dados
3. divisão em treino e teste
4. treinamento dos modelos
5. avaliação dos resultados

## Dataset utilizado
Foi utilizado o dataset **Wine Quality (Red Wine)**, disponível publicamente na base UCI Machine Learning Repository.

Esse dataset foi escolhido porque permite trabalhar com dois tipos de problema:
- **Regressão:** prever a nota de qualidade do vinho (`quality`)
- **Classificação:** prever se o vinho é considerado bom ou não

> **Observação:** O projeto respeita as restrições do enunciado, pois não utiliza os datasets **Iris** nem **California Housing Prices**.

## Modelos utilizados

### Classificação
Para o problema de classificação, foi criada uma variável chamada `bom_vinho`, definida da seguinte forma:
- `1` para vinhos com qualidade maior ou igual a 7
- `0` para os demais casos

Foram utilizados os seguintes algoritmos:
- **K-Nearest Neighbors (KNN)**
- **Regressão Logística**

### Regressão
Para o problema de regressão, foi utilizado o algoritmo:
- **Regressão Linear**


## Link para o video de apresentação: https://youtu.be/jNw1tMqv8KY 

## Tecnologias e bibliotecas utilizadas
O projeto foi desenvolvido em **Python**, utilizando principalmente as seguintes bibliotecas:
- Pandas
- NumPy
- Scikit-learn

O código pode ser executado em:
- Google Colab
- Jupyter Notebook
- ambiente local com Python

## Etapas do pipeline

### 1. Coleta e leitura dos dados
O dataset é carregado diretamente por URL.

### 2. Preparação dos dados
Foi realizada a separação entre variáveis de entrada e variáveis alvo.
Também foi criada a variável `bom_vinho` para o problema de classificação.

### 3. Divisão entre treino e teste
Os dados foram divididos em conjunto de treino e conjunto de teste para garantir uma avaliação mais confiável dos modelos.

### 4. Pré-processamento
Foi aplicado um pipeline com:
- preenchimento de valores ausentes com a mediana
- padronização dos dados com `StandardScaler`

### 5. Treinamento dos modelos
Foram treinados:
- KNN
- Regressão Logística
- Regressão Linear

### 6. Avaliação dos modelos

#### Métricas de classificação
- Accuracy
- Precision
- Recall
- F1-score
- Matriz de confusão
- Classification report

#### Métricas de regressão
- MAE
- MSE
- RMSE
- R²

## Estrutura do repositório
```bash
.
├── checkpoint_ml_wine_quality.ipynb
├── checkpoint_ml_wine_quality.py
└── README.md
