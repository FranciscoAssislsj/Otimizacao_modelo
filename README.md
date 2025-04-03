# Otimização de Modelos com GridSearchCV

## Objetivo:
Utilizar GridSearchCV para otimizar os hiperparâmetros do modelo GradientBoostingRegressor e avaliar seu impacto no desempenho.

## Tecnologias Utilizadas
Python, Pandas, NumPy, Scikit-learn

## Dados:
Variáveis categóricas e numéricas que influenciam no preço.
SalePrice: O preço final do imóvel (variável alvo).

##Normalização e Tratamento de Dados:

Preenchimento de valores nulos com a média da coluna.
Normalização dos dados numéricos antes do treinamento do modelo.

## Otimização de Hiperparâmetros
O GridSearchCV é utilizado para testar diferentes combinações de hiperparâmetros do modelo GradientBoostingRegressor, incluindo:
learning_rate: [0.03]
subsample: [0.2]
n_estimators: [100, 1000, 5000]
max_depth: [5, 8]
A avaliação é feita com cross-validation (cv=2) e a métrica utilizada para seleção do melhor modelo é o R² (scoring='r2').
