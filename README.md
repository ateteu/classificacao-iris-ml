# Classificação de flores Iris com ML

Este repositório apresenta um pequeno projeto de machine learning, para aplicar e exercitar conceitos básicos do tema.

## Dataset

O conjunto de dados utilizado é o **Iris Dataset**, disponível diretamente na biblioteca `scikit-learn`.

Cada observação contém quatro características da flor:

* comprimento da sépala
* largura da sépala
* comprimento da pétala
* largura da pétala

O objetivo do modelo é prever a **espécie da flor**, que pode ser:

* Iris setosa
* Iris versicolor
* Iris virginica

## Modelos utilizados

Serão treinados e comparados três modelos de classificação:

* Regressão Logística
* Árvore de Decisão
* Random Forest

## Pipeline

1. Carregamento do dataset
2. Exploração inicial dos dados
3. Separação entre features (X) e target (y)
4. Divisão em conjunto de treino e teste
5. Treinamento dos modelos
6. Geração de previsões
7. Avaliação de desempenho

## Como executar

- Clone o repositório: git clone URL_DO_REPOSITORIO
- Instale as dependências: pip install -r requirements.txt
- Depois abra o notebook: jupyter notebook

## Licença

Este projeto está disponível sob a licença MIT.
