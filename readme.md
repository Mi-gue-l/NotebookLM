# Detecção de Fraude em Cartão de Crédito

Projeto de machine learning para identificar transações fraudulentas em cartões de crédito,
com foco no desbalanceamento extremo da base: apenas 0,17% das transações são fraude. Por isso,
a métrica principal não é acurácia, e sim **recall**, **precisão** e **F1** da classe de fraude.

## O que foi feito
- Criação da variável `log_amount` e padronização com `StandardScaler`.
- Divisão treino/teste com `stratify` para manter a proporção de fraudes.
- Treino e comparação de Regressão Logística, Random Forest e XGBoost, com balanceamento
  de classes.
- Ajuste do limiar de decisão pelo melhor F1 na curva de precisão-recall.
- Explicação das previsões com **SHAP**.

## Resultados (classe fraude)

| Modelo               | Precisão | Recall | F1 |
|-----------------------|----------|--------|----|
| Regressão Logística   | [x]      | [x]    | [x]|
| Random Forest         | [x]      | [x]    | [x]|
| XGBoost               | [x]      | [x]    | [x]|

Limiar escolhido: **[x]**

## Diferenças em relação à Expert
[preencher]

## Ferramentas
pandas, numpy, scikit-learn, xgboost, shap, matplotlib, seaborn
