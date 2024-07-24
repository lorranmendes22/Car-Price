

# Previsão de Venda de Carros Usados

Este projeto tem como objetivo desenvolver um modelo de machine learning para prever se um carro será vendido com base em características como idade do modelo, quilometragem por ano e preço.

## Bibliotecas Utilizadas
- pandas
- numpy
- sklearn.neighbors (KNeighborsClassifier)
- sklearn.svm (LinearSVC, SVC)
- sklearn.model_selection (train_test_split)
- seaborn

## Dataset
Utilizamos um dataset de preços de carros, contendo informações como quilometragem por ano, ano do modelo, preço e se foi vendido.

## Pré-processamento
- Renomeação de colunas para melhor compreensão.
- Conversão da variável alvo "vendido" para valores binários (0 - não vendido, 1 - vendido).
- Criação de novas colunas como idade do modelo e quilometragem convertida para quilômetros.
- Remoção de colunas desnecessárias.

## Análise Exploratória
- Balanceamento dos dados mostrou que 58% dos carros foram vendidos.

## Modelagem e Avaliação
- Testamos diversos modelos de classificação:
  - Linear SVC
  - SVC com kernel linear
  - SVC com kernel RBF (com StandardScaler para normalização)
  - Decision Tree Classifier

- Avaliamos a acurácia dos modelos e comparamos com um Dummy Classifier.

## Conclusão
O modelo mais promissor até agora foi o SVC com kernel RBF, alcançando uma acurácia de 75.92%.

