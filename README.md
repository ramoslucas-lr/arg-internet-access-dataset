# 📊 Tratamento de Dados do Banco Mundial para Análise da Evolução da Internet na Argentina 🇦🇷

Este repositório contém um notebook Jupyter 📓 e um dataset tratado para a análise da evolução da internet na Argentina, utilizando dados do Banco Mundial 🌐. O objetivo é fornecer uma visão clara e organizada dos dados, facilitando a criação de visualizações 📈 e a geração de insights relevantes 💡.

## Conteúdo do Repositório 📂

* `datasets/worldbank_data.csv`: Dataset bruto do Banco Mundial 🌍.
* `treated_dataset.csv`: Dataset tratado, pronto para análise e visualização ✅.
* `data_treatment.ipynb`: Notebook Jupyter com o código de tratamento dos dados 👨‍💻.
* `README.md`: Este arquivo, com informações sobre o repositório 📝.

## Tratamento dos Dados 🛠️

O notebook `data_treatment.ipynb` realiza as seguintes etapas de tratamento dos dados:

1.  **Leitura do Dataset Bruto 📖:**
    O dataset bruto é lido do arquivo `worldbank_data.csv` usando `pandas.read_csv()`.
2.  **Limpeza Inicial 🧹:**
    * Remoção da coluna 'Series Code' 🗑️.
    * Extração dos anos dos nomes das colunas 📅.
    * Renomeação das colunas para facilitar a manipulação 🏷️.
3.  **Transformação para o Formato Longo (Melt) 🔄:**
    O DataFrame é transformado para o formato longo usando `pandas.melt()`.
4.  **Remoção de Duplicatas 👯‍♂️➡️ 1️⃣:**
    As linhas duplicadas são removidas.
5.  **Pivotagem para o Formato Largo ↔️:**
    O DataFrame é pivotado para o formato largo, com os indicadores como colunas.
6.  **Substituição de NaN por None 🚫➡️ ⚪:**
    Os valores NaN são substituídos por None para evitar problemas com bancos de dados.
7.  **Salvamento do Dataset Tratado 💾:**
    O DataFrame tratado é salvo em `treated_dataset.csv`.

## Requisitos 📦

Para executar o notebook, você precisará das seguintes bibliotecas Python 🐍:

* `numpy` 🔢
* `pandas` 🐼
* `re` 🔍

Você pode instalar essas bibliotecas usando o `pip`:

```bash
pip install numpy pandas
