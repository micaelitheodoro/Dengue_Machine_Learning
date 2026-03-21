#  Previsão de Casos de Dengue com Machine Learning

Este projeto apresenta um estudo de modelagem preditiva aplicado a séries temporais, com o objetivo de prever a evolução dos casos ativos de dengue a partir de dados históricos e variáveis climáticas.

---

## Objetivo

Desenvolver um modelo capaz de antecipar a dinâmica de casos de dengue ao longo do tempo, considerando:

- Dependência temporal da série
- Sazonalidade
- Influência de fatores externos (clima)

---

##  Abordagem

O projeto foi estruturado em etapas clássicas de um pipeline de Data Science:

###  1. Integração de Dados
- Dados epidemiológicos (casos de dengue)
- Dados meteorológicos (precipitação e temperatura)

###  2. Engenharia de Features
Foram criadas variáveis para capturar a dinâmica temporal:

- **Lags temporais** (histórico da série)
- **Médias móveis** (tendência)
- **Componentes sazonais** (sen/cos)
- **Variáveis climáticas defasadas**

Essa etapa foi fundamental para melhorar a capacidade preditiva do modelo.

---

## 🤖 Modelo

Foi utilizado o modelo:

- **Gradient Boosting Regressor**

Principais motivos da escolha:
- Captura relações não lineares
- Modela interações entre variáveis
- Robusto para datasets de tamanho moderado
- Não requer normalização

O modelo foi treinado de forma temporal, respeitando a ordem dos dados, evitando vazamento de informação.

---

## Avaliação

O desempenho foi avaliado em um período futuro em relação ao treinamento, simulando um cenário real de previsão.

Métrica utilizada:
- **MAE (Mean Absolute Error)**

Também foram gerados gráficos comparando valores reais vs previstos.

---

## Interpretabilidade

Além da previsão, o projeto inclui análise de interpretabilidade:

### Feature Importance
- Identifica quais variáveis foram mais relevantes para o modelo

### PRCC (Partial Rank Correlation Coefficient)
- Avalia a influência individual de cada variável
- Permite análise mais robusta da dinâmica do sistema

---

## Principais Insights

- Forte dependência do histórico recente da série
- Tendência (médias móveis) como fator dominante
- Influência relevante de variáveis climáticas
- Indícios de comportamento sazonal e cíclico

---

## Aplicação Industrial

A abordagem desenvolvida é diretamente aplicável a contextos industriais.

Possíveis aplicações:
- Manutenção preditiva
- Previsão de falhas em equipamentos
- Análise de séries temporais de sensores (vibração, temperatura, carga)

A lógica permanece a mesma:
- Uso de dados históricos
- Engenharia de features temporais
- Modelos de Machine Learning para previsão de eventos futuros

---

## Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

---


## Autor: Micaeli M. Theodoro





**Micaeli M. Theodoro**  
Projeto desenvolvido como case técnico para Data Science / AI
