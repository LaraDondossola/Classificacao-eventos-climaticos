# 🌊 Classificação e Estimativa de Eventos Climáticos Extremos

Projeto de **Machine Learning** desenvolvido para analisar eventos climáticos extremos, estimando a população afetada e classificando o nível de risco em **Baixo, Médio ou Alto**.

## 🎯 Objetivo

O projeto utiliza algoritmos de **Aprendizado Supervisionado** para:

- Estimar quantitativamente a população afetada por um evento;
- Classificar o nível de risco do desastre;
- Comparar diferentes modelos de regressão;
- Disponibilizar os resultados por meio de uma interface web.

## 🔄 Etapas do projeto

```text
Dados originais
      ↓
Inserção de ruídos
      ↓
Limpeza e tratamento dos dados
      ↓
Feature Engineering
      ↓
Pré-processamento
      ↓
Treinamento dos modelos
      ↓
Avaliação
      ↓
Interface Web
```

## 📊 Dataset

O projeto utiliza dados históricos de danos informados em eventos climáticos, incluindo informações sobre população, danos humanos, materiais e prejuízos econômicos.

## 🛠️ Tecnologias

- Python
- Pandas e NumPy
- Scikit-learn
- Matplotlib e Seaborn
- Streamlit
- Joblib

## 📂 Estrutura do projeto

```text
Classificacao-eventos-climaticos/
│
├── Datasets/
│   ├── Danos_Informados.xlsx
│   ├── Danos_Informados_Original.xlsx
├── Models/
│   ├── modelo_knn_regressor.pkl
│   ├── modelo_random_forest.pkl
│   └── preprocessor.pkl
│
├── Notebooks/
│   ├── Introdução_de_ruídos.ipynb
│   ├── Limpeza_e_Pré_processamento.ipynb
│   └── Interface_eventos_climáticos.ipynb
│
└── README.md
```

##📊 Avaliação

Os modelos são avaliados utilizando:

MAE – Erro Absoluto Médio;
RMSE – Raiz do Erro Quadrático Médio;
R² – Coeficiente de Determinação.

Também são realizadas análises dos erros e dos resíduos das previsões.

##👩‍💻 Projeto

Classificação e Estimativa de Eventos Climáticos Extremos

Desenvolvido como projeto acadêmico de Machine Learning.
