
# Arquitetura do Projeto: Análise Exploratória de Dados (EDA) de Pools e Yields

## 1. Estrutura de Pastas

```
.
├── data/
│   ├── raw/ (dados brutos baixados do DefiLlama)
│   └── processed/ (dados limpos e transformados)
├── notebooks/
│   ├── 01_data_ingestion.ipynb (coleta inicial de dados)
│   ├── 02_data_cleaning.ipynb (limpeza e pré-processamento)
│   ├── 03_eda.ipynb (análise exploratória de dados)
│   └── 04_reporting.ipynb (geração de relatórios/visualizações)
├── src/
│   ├── __init__.py
│   ├── data_ingestion.py (funções para coleta de dados)
│   ├── data_processing.py (funções para limpeza e transformação)
│   └── visualization.py (funções para visualização)
├── reports/
│   └── figures/ (gráficos e imagens gerados)
├── .gitignore
├── README.md
├── requirements.txt
└── setup.py (opcional, para projetos maiores)
```

## 2. Bibliotecas e Ferramentas Principais

*   **Coleta de Dados:** `requests` (para baixar CSVs do DefiLlama)
*   **Manipulação de Dados:** `pandas` (para DataFrames e Series)
*   **Análise de Dados:** `numpy` (para operações numéricas)
*   **Visualização:** `matplotlib.pyplot`, `seaborn` (para gráficos)
*   **Relatórios:** Markdown (para documentação)

## 3. Fluxo de Trabalho

1.  **Coleta:** Baixar os dados de pools e yields do DefiLlama (CSV). Salvar em `data/raw/`.
2.  **Limpeza:** Carregar os dados brutos, tratar valores ausentes, converter tipos de dados, remover duplicatas. Salvar os dados limpos em `data/processed/`.
3.  **Análise Exploratória:** Realizar análises descritivas, identificar tendências, outliers e relacionamentos usando `pandas`, `numpy` e visualizações com `matplotlib` e `seaborn`.
4.  **Visualização:** Criar gráficos e tabelas para comunicar os insights. Salvar em `reports/figures/`.
5.  **Relatório:** Documentar o processo, as descobertas e as conclusões em um arquivo Markdown ou Jupyter Notebook.

## 4. Documentação

*   **README.md:** Visão geral do projeto, como configurar e executar.
*   **Jupyter Notebooks:** Para exploração interativa e documentação do processo.
*   **Docstrings:** Documentação interna para funções e classes em `src/`.

Este é um ponto de partida. À medida que o projeto avança, podemos refinar e adicionar mais detalhes à arquitetura.

