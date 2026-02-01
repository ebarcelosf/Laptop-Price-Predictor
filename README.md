# Predição de Preços de Laptops com Machine Learning 💻📊

Este projeto desenvolve um modelo de regressão capaz de prever o preço de laptops com base em suas especificações técnicas. Desenvolvido para a disciplina **INF1032 - Introdução à Ciência de Dados na PUC-Rio**.

## 🎯 Objetivo
O objetivo principal foi criar um modelo preditivo com um erro médio (MAE) inferior a 7.500,00 INR, permitindo uma avaliação justa de mercado tanto para consumidores quanto para vendedores.

## 🛠️ Tecnologias e Ferramentas
* **Linguagem:** Python
* **Bibliotecas:** Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn
* **Interpretabilidade:** SHAP (SHapley Additive exPlanations)

## 📁 Dataset
Utilizamos o *Uncleaned Laptop Price Dataset* do Kaggle, contendo 1.303 amostras e 12 variáveis iniciais, como Marca, Resolução de Tela, CPU, RAM, Memória, GPU e Sistema Operacional.

## 🚀 Metodologia
O projeto seguiu as seguintes etapas cruciais:
1.  **Limpeza e Pré-processamento:** Tratamento de valores nulos, conversão de unidades (ex: remoção de 'kg' e 'GB') e correção de tipos de dados.
2.  **Análise Exploratória (EDA):** Identificação de distribuições assimétricas e correlações entre hardware e preço.
3.  **Feature Engineering:** Criação de 32 novas features a partir das variáveis originais para capturar nuances técnicas (ex: tipo de armazenamento, marca do processador).
4.  **Modelagem e Tuning:** Comparação entre modelos Baseline (Regressão Linear), Random Forest e XGBoost com otimização de hiperparâmetros.
5.  **Interpretabilidade:** Uso de análise SHAP para quantificar o impacto de cada característica no preço final.

## 📈 Resultados
O modelo final utilizando **XGBoost com Log Transformation** alcançou:
* **MAE:** 8.168,71 INR (uma redução de 78,1% em relação ao baseline).
* **R²:** 0.8432 (o modelo explica 84,32% da variância dos preços).

A análise demonstrou que a técnica de *Feature Engineering* teve um impacto superior ao ajuste fino de hiperparâmetros.

## 👥 Equipe
* Luis Felipe Gadelha
* Victor Coutinho
* Enzo Ferreira
