# 🩺 Predição de Diabetes com Machine Learning

Este projeto tem como objetivo desenvolver um modelo preditivo para diagnosticar diabetes a partir de dados clínicos. O processo envolve desde a análise exploratória dos dados até a construção e avaliação de um modelo de aprendizado de máquina com técnicas de engenharia de atributos.

## 📊 Sobre o Projeto

A partir de um conjunto de dados contendo variáveis clínicas como glicose, insulina, IMC, idade e outros fatores, foi realizada uma série de etapas para aprimorar a performance do modelo, incluindo:

- Análise Exploratória de Dados (EDA)
- Tratamento de valores ausentes e outliers
- Balanceamento das classes com SMOTE
- Criação de variáveis derivadas com base em raciocínio clínico
- Testes de correlação e importância das features
- Otimização de hiperparâmetros com `RandomizedSearchCV`
- Avaliação de performance com métricas como acurácia, precisão, recall, F1-score e matriz de confusão

## 📁 Arquivos

- `diabetes_model.ipynb`: Notebook principal com todo o pipeline de análise, engenharia de atributos e modelagem.
- `dados_diabetes.csv`: Conjunto de dados utilizado para treinar e avaliar o modelo.

## 🧪 Resultados

O modelo final, um `RandomForestClassifier` com parâmetros otimizados, atingiu os seguintes resultados:

- **Acurácia no conjunto de teste:** 0.84
- **Precisão para diagnóstico positivo (diabético):** 0.81
- **Recall para diagnóstico positivo (diabético):** 0.89

As variáveis derivadas como `Glucose_BMI_Index`, `Glucose_BMI_Age`, `Insulin_per_Age` e `Glucose_Insulin_BMI` contribuíram significativamente para a melhora da performance preditiva.

## 💡 Conclusão

Através de uma abordagem centrada na compreensão clínica das variáveis e na engenharia de atributos, foi possível criar um modelo robusto, com bom desempenho e interpretabilidade. Este projeto mostra como dados clínicos bem trabalhados podem oferecer bons insights para suporte ao diagnóstico de diabetes.
