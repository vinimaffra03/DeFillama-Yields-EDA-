# Projeto de Análise Exploratória de Dados (EDA) de Pools e Yields DeFi

## Visão Geral

Este projeto tem como objetivo realizar uma Análise Exploratória de Dados (EDA) aprofundada sobre pools de liquidez e rendimentos (yields) do ecossistema de Finanças Descentralizadas (DeFi), utilizando dados fornecidos pela plataforma DefiLlama. O foco é entender as características, tendências e padrões desses dados para extrair insights valiosos.

## Objetivos

- Coletar dados históricos de pools e yields do DefiLlama.
- Realizar a limpeza e pré-processamento dos dados para garantir sua qualidade.
- Aplicar técnicas de análise descritiva e visualização de dados para identificar padrões, distribuições e correlações.
- Gerar insights sobre o comportamento das pools de liquidez e a performance dos rendimentos ao longo do tempo.

## Estrutura do Projeto

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

## Tecnologias Utilizadas

- **Python 3.x**
- **Bibliotecas:**
  - `pandas`: Manipulação e análise de dados.
  - `numpy`: Operações numéricas.
  - `matplotlib`: Visualização de dados.
  - `seaborn`: Visualização estatística de dados.
  - `requests`: Para requisições HTTP (coleta de dados).

## Como Configurar e Executar o Projeto

### 1. Clonar o Repositório

```bash
git clone <URL_DO_REPOSITORIO>
cd <NOME_DO_REPOSITORIO>
```

### 2. Criar e Ativar o Ambiente Virtual

É altamente recomendável usar um ambiente virtual para gerenciar as dependências do projeto.

```bash
python -m venv venv
source venv/bin/activate  # No Linux/macOS
# venv\Scripts\activate  # No Windows
```

### 3. Instalar as Dependências

```bash
pip install -r requirements.txt
```

### 4. Coletar os Dados

Os dados brutos podem ser baixados manualmente do DefiLlama (https://defillama.com/yields) ou utilizando o script de ingestão de dados:

```bash
# Exemplo de execução do script de ingestão (se implementado em src/data_ingestion.py)
python src/data_ingestion.py
```

Alternativamente, você pode executar o notebook `01_data_ingestion.ipynb` para realizar a coleta.

### 5. Executar a Análise

Os notebooks na pasta `notebooks/` guiam você através do processo de EDA:

1.  `01_data_ingestion.ipynb`: Coleta e salvamento dos dados brutos.
2.  `02_data_cleaning.ipynb`: Limpeza e pré-processamento dos dados.
3.  `03_eda.ipynb`: Análise exploratória e visualizações.
4.  `04_reporting.ipynb`: Geração de relatórios e insights finais.

Recomenda-se executar os notebooks em ordem para seguir o fluxo de trabalho do projeto.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests para melhorias, correções de bugs ou novas funcionalidades.

## Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes. (Se aplicável)

## Contato

Para dúvidas ou sugestões, entre em contato com [Seu Nome/Email/GitHub].
