# 🚀 Detecção de Anomalias em Transações Financeiras

[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1i-ugfCzAT1uirz8D_Ur8R2yw0ULZERQc?usp=sharing)

## 📌 Sobre o Projeto

Este projeto foi desenvolvido como parte do **Bootcamp da DIO (Digital Innovation One)** e tem como objetivo detectar transações fraudulentas utilizando técnicas de Machine Learning. O sistema lida com dados desbalanceados e garante explicabilidade das decisões através do SHAP.

## 🎯 Objetivo

Desenvolver um sistema de detecção de fraudes em transações financeiras utilizando técnicas de Machine Learning, com foco em:

- Lidar com dados desbalanceados (apenas 3% de fraudes)
- Garantir explicabilidade das decisões do modelo
- Comparar diferentes algoritmos
- Otimizar performance através de ajuste de threshold

## 📊 Metodologia

### 1. Análise Exploratória de Dados (EDA)
- Distribuição das classes (Normal vs Fraude)
- Correlação entre features e variável alvo
- Identificação do desbalanceamento severo

### 2. Pré-processamento
- Padronização com StandardScaler
- Divisão estratificada (70% treino, 30% teste)

### 3. Balanceamento
- Aplicação de **SMOTE** (Synthetic Minority Over-sampling Technique)
- Geração de amostras sintéticas da classe minoritária

### 4. Modelos Utilizados
- **Random Forest**: Ensemble de árvores de decisão
- **XGBoost**: Gradient Boosting otimizado

### 5. Avaliação
- Matriz de Confusão
- Classification Report (Precision, Recall, F1-Score)
- AUC-ROC
- Curva Precision-Recall
- Ajuste de Threshold

### 6. Explicabilidade
- **SHAP** (SHapley Additive exPlanations)
- Interpretação das decisões do modelo
- Transparência para compliance e auditoria

## 📈 Resultados Obtidos

| Modelo | AUC-ROC | Recall (Fraude) | Precision (Fraude) | F1-Score (Fraude) |
|--------|---------|-----------------|-------------------|-------------------|
| Random Forest | 0.95 | 0.85 | 0.75 | 0.80 |
| XGBoost | 0.96 | 0.88 | 0.78 | 0.83 |
| XGBoost (Threshold 0.4) | 0.96 | 0.92 | 0.72 | 0.81 |

## 🛠️ Tecnologias Utilizadas

- **Google Colab**: Ambiente 100% online
- **Python 3.10**: Linguagem principal
- **Pandas & NumPy**: Manipulação de dados
- **Scikit-learn**: Pré-processamento e modelos
- **Imbalanced-learn**: SMOTE para balanceamento
- **XGBoost**: Modelo avançado
- **SHAP**: Explicabilidade
- **Matplotlib & Seaborn**: Visualizações

## 💡 Diferenciais do Projeto

✅ Tratamento de dados desbalanceados com SMOTE
✅ Comparação entre múltiplos algoritmos
✅ Explicabilidade com SHAP
✅ Ajuste fino de threshold
✅ 100% online (Google Colab)
✅ Código completamente documentado

## 🎯 Conclusão

O projeto demonstra que é possível detectar fraudes com alta precisão utilizando Machine Learning. O modelo XGBoost com SMOTE apresentou a melhor performance, com AUC-ROC de 0.96, identificando aproximadamente 88% das transações fraudulentas.

## 🔮 Próximos Passos

- Implementar validação cruzada
- Testar LightGBM e CatBoost
- Deploy do modelo em produção
- Monitoramento contínuo

## 📂 Estrutura do Projeto
