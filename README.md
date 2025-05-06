📊 Análise e Plotagem de Gráficos Interativos com Python

Este projeto demonstra como realizar uma análise de dados e criar gráficos interativos utilizando Python, com foco em bibliotecas como Pandas, Matplotlib e Plotly.
A abordagem é baseada no artigo de Erik Marta Garcia, que explora técnicas de visualização de dados para facilitar a interpretação e a tomada de decisões.
📁 Estrutura do Projeto

📁 analise-graficos-interativos/
├── data/
│   └── dados.csv
├── notebooks/
│   └── analise_visualizacao.ipynb
├── images/
│   └── grafico_interativo.png
├── app.py
└── README.md

🔍 Objetivo
    Realizar a análise exploratória de dados (EDA) para identificar padrões e insights.
    Criar gráficos interativos que permitam uma melhor compreensão dos dados.
    Demonstrar o uso de bibliotecas populares de Python para visualização de dados.


🧰 Tecnologias Utilizadas
    Python 3.x
    Pandas
    Matplotlib
    Plotly
    Jupyter Notebook


📊 Análise de Dados

Utilizamos o Pandas para carregar e explorar o conjunto de dados:

import pandas as pd

# Carregar os dados
df = pd.read_csv('data/dados.csv')

# Visualizar as primeiras linhas
print(df.head())

📈 Visualização com Matplotlib

Criamos gráficos básicos utilizando o Matplotlib:

import matplotlib.pyplot as plt

# Gráfico de barras
plt.figure(figsize=(10,6))
plt.bar(df['Categoria'], df['Valor'])
plt.title('Distribuição por Categoria')
plt.xlabel('Categoria')
plt.ylabel('Valor')
plt.show()

🌐 Gráficos Interativos com Plotly

Aprimoramos a visualização utilizando o Plotly para criar gráficos interativos:

import plotly.express as px

# Gráfico de dispersão interativo
fig = px.scatter(df, x='Variavel_X', y='Variavel_Y', color='Categoria', size='Valor')
fig.show()

🚀 Como Executar o Projeto

    Clone o repositório:
git clone https://github.com/seu_usuario/analise-graficos-interativos.git

    Navegue até o diretório do projeto:
cd analise-graficos-interativos

    Instale as dependências:
pip install -r requirements.txt

    Execute o notebook Jupyter:
jupyter notebook notebooks/analise_visualizacao.ipynb

📚 Referência
    Artigo original: Análise & Plotagem de Gráfico Interativo com Python
