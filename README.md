# Classificação de flores Iris com ML

Este repositório apresenta um pequeno projeto de machine learning, para aplicar e exercitar conceitos básicos do tema.

## Dataset

O conjunto de dados utilizado é o **Iris Dataset**, disponível diretamente na biblioteca `scikit-learn`.

Cada observação contém quatro características da flor:

* Comprimento da sépala
* Largura da sépala
* Comprimento da pétala
* Largura da pétala

O objetivo do modelo é prever a **espécie da flor**, que pode ser:

* *Iris setosa*
* *Iris versicolor*
* *Iris virginica*

## Modelos utilizados

Serão treinados e comparados três modelos de classificação:

* `Regressão Logística`
* `Árvore de Decisão`
* `Random Forest`

## Pipeline

1. Carregamento do dataset
2. Exploração inicial dos dados
3. Separação entre features (X) e target (y)
4. Divisão em conjunto de treino e teste
5. Treinamento dos modelos
6. Geração de previsões
7. Avaliação de desempenho

## Conclusões e aprendizados

A análise exploratória mostrou que as **características das pétalas são muito mais discriminativas** do que as da sépala. 

Nos gráficos de dispersão, as pétalas formam grupos bem definidos entre as espécies, enquanto as sépalas apresentam maior sobreposição.


Em relação aos modelos, observou-se que:
- `Regressão Logística`:
Os coeficientes do modelo evidenciam que as features relacionadas às pétalas possuem maior peso na classificação, especialmente na distinção da espécie *virginica*.

  A matriz de confusão da Regressão Logística indicou apenas um erro de classificação, onde uma amostra da classe *versicolor* foi classificada como *virginica*, resultando em alta acurácia: **~96.67%**.

- `Árvore de Decisão`:
Apresentou desempenho semelhante, também com acurácia de **~96.67%** e apenas um erro de classificação. A árvore gerada possui baixa profundidade (5) e poucas folhas (8), indicando que o problema pode ser resolvido com regras relativamente simples.

- `Random Forest`:
Apresentou desempenho ligeiramente inferior de **~93.33%**, com dois erros de classificação. Ainda assim, o modelo confirmou a importância das features de pétalas, especialmente *petal width*, que apresentou maior relevância na decisão.


De forma geral, todos os modelos tiveram alto desempenho, o que é esperado para o dataset Iris, que possui boa separabilidade entre classes.

Com isso, este projeto permitiu consolidar conceitos fundamentais de machine learning supervisionado, além de reforçar a importância da análise exploratória para entender quais variáveis realmente contribuem para a solução do problema.
