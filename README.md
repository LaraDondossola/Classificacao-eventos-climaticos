# 🌪️ Classificação de Riscos e Estimativa de Eventos Climáticos Extremos

> **Aprendizado Baseado em Problema (ABP) — Machine Learning**  
> *Engenharia de Computação — Centro Universitário SATC (UniSATC)*  
> 🗓️ **Ano:** 2026

---

## 📌 Visão Geral do Projeto

Este projeto utiliza **Algoritmos de Aprendizado Supervisionado (Machine Learning Clássico)** para apoiar o planejamento e a tomada de decisão na gestão de desastres climáticos, atuando como ferramenta de suporte a órgãos como a **Defesa Civil**. 

A partir de dados históricos de desastres naturais no Brasil ocorridos em **2024** (extraídos do **S2iD**), a solução aborda o problema sob duas perspectivas complementares:

1. **🎯 Classificação Multiclasse:** Categorização rápida do **nível de risco/gravidade** do evento (*Baixo*, *Médio* ou *Alto*).
2. **📈 Regressão Quantitativa:** Estimativa contínua do **volume total de população afetada** pelo desastre.

---

## 🎯 Objetivos do Projeto

### 🟢 Objetivo Geral
Desenvolver e comparar modelos de Machine Learning para prever a população afetada e classificar o nível de risco de eventos climáticos extremos no Brasil.

### 🔹 Objetivos Específicos
- 📂 **Coleta e Inspecção:** Estruturar o dataset oficial do S2iD relativo ao ano de 2024.
- 📊 **Análise Exploratória (EDA):** Identificar padrões, qualidade dos dados e distribuições de danos materiais/humanos.
- 🧹 **Pré-Processamento & Feature Engineering:** Limpeza de ruídos, imputação de nulos e criação das variáveis alvo (`Total Afetados` e `Nível de Risco`).
- 🤖 **Treinamento e Otimização:** Testar e comparar múltiplos algoritmos de aprendizado supervisionado.
- 📈 **Avaliação e Importância:** Analisar métricas de desempenho e a relevância das variáveis (*Feature Importance*).

---

## 🗃️ Base de Dados (Dataset)

Os dados utilizados são provenientes do **S2iD (Sistema Integrado de Informações sobre Desastres)**, mantido pelo Ministério da Integração e do Desenvolvimento Regional. 

### 💡 Principais Variáveis do Dominio:
- **Localização:** UF, Município, COBRADE (Classificação de Desastre).
- **Danos Humanos:** Número de mortos, feridos, enfermos, desabrigados, desalojados e desaparecidos.
- **Danos Materiais e Prejuízos (R$):** Impactos na saúde, ensino, habitação, infraestrutura e prejuízos nos setores de agricultura, pecuária, indústria, comércio e serviços.

---

## 🏗️ Estrutura do Repositório

```text
Classificacao-eventos-climaticos/
│
├── Datasets/
│   ├── Danos_Informados_Original.xlsx   # Dados brutos extraídos do S2iD
│   └── Danos_Informados.xlsx       # Base com ruídos controlados para testes de pipeline
│
├── notebooks/
│   ├── Introdução_de_ruídos.ipynb       # Script para simulação de imperfeições no dataset
│   └── eda_e_modelagem.ipynb            # Notebook principal de EDA, Limpeza e Machine Learning
│
└── README.md                            # Documentação principal
