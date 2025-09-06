# 🎬 Desafio Ciência de Dados - IMDb

Projeto desenvolvido como parte do **Desafio Lighthouse 2025** em Ciência de Dados.

---

## 📌 Objetivo
Explorar e analisar um conjunto de dados de filmes do IMDb, extraindo insights relevantes e construindo um modelo de Machine Learning capaz de prever a nota dos filmes (IMDB Rating).

---

## 📊 Etapas do Projeto
1. **Análise Exploratória (EDA)**  
   - Visualização de distribuições de notas, faturamento e duração.  
   - Relações entre variáveis (correlação, scatterplots, evolução temporal).  
   - Investigação dos gêneros mais frequentes e dos atores mais recorrentes.  
   - Identificação de padrões, como atores e gêneros que tendem a estar associados a melhores notas.

2. **Modelagem**  
   - Construção de um pipeline em `scikit-learn` com pré-processamento (OneHotEncoder, TF-IDF, imputação de valores).  
   - Treinamento de um modelo de Regressão Linear para prever a nota IMDb.  
   - Avaliação usando **MAE (Mean Absolute Error)** e **R²**.

3. **Resultados**  
   - Modelo atingiu um **MAE ≈ 0.17**, mostrando boa precisão em prever as notas.  
   - O **R² ≈ 0.28** indica que parte da variação das notas pode ser explicada pelas variáveis disponíveis.  
   - Insights relevantes:  
     - Filmes com certos atores apresentam médias mais altas.  
     - Duração entre 100 e 150 minutos concentra a maioria dos sucessos de bilheteria.  
     - O gênero Drama é o mais frequente e bem avaliado.  
     - As notas médias se mantêm estáveis ao longo de décadas, entre 7.8 e 8.2.

4. **Exportação**  
   - Modelo salvo em `.pkl` dentro da pasta `models/`.  
   - Exemplo de uso para carregar o modelo e fazer previsões em novos filmes.  
---
## 📂 Estrutura do Repositório
   - data/ # Dataset original
   - notebooks/ # Notebook Jupyter com análise e modelagem
   - models/ # Modelo treinado salvo (.pkl)
   - requirements.txt # Dependências do projeto
   - README.md # Documentação do projeto
---

## ▶️ Como Rodar o Projeto

1. Clone este repositório:
   ```bash
   git clone https://github.com/ArturCesarGit/desafio-ciencia-dados-imdb.git
   cd desafio-ciencia-dados-imdb
   python -m venv .venv
   .venv\Scripts\activate
   (mac/linux) source .venv/bin/activate
   pip install -r requirements.txt
   jupyter notebook notebooks/imdb_pipeline.ipynb
🚀 Resultados

O modelo pode ser usado para prever a nota IMDb de novos filmes, a partir de atributos como ano, gênero, certificação, duração, descrição e elenco.

A análise exploratória trouxe insights interessantes sobre padrões do cinema e fatores que podem influenciar avaliações.
   
