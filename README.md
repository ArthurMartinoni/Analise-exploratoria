# Análise Exploratória de Dados — Credit Card Fraud Detection

## Descrição

Análise exploratória de dados (EDA) sobre transações de cartão de crédito, com o objetivo de identificar distribuições, padrões e possíveis indicadores de fraude. Projeto individual desenvolvido em Python.

## Fonte dos dados

[Credit Card Fraud Detection (Kaggle/ULB)](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) — 284.807 transações de cartão de crédito de titulares europeus, registradas ao longo de 2 dias em setembro de 2013.

## Ferramentas utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

## Etapas do projeto

1. **Coleta de dados** — carregamento do dataset público via Pandas.
2. **Inspeção** — verificação de estrutura, tipos de dados, valores nulos e duplicados.
3. **Tratamento de dados** — investigação e remoção de 1.081 linhas duplicadas, com verificação prévia da taxa de fraude nesse subconjunto para garantir que nenhum padrão relevante fosse descartado sem análise.
4. **Análise exploratória** — distribuições de valor (Amount) e tempo (Time), comparação entre transações fraudulentas e não fraudulentas, e matriz de correlação.
5. **Conclusão** — síntese dos principais achados.

## Principais achados

- O dataset é extremamente desbalanceado: apenas 0,172% das transações são fraude.
- A distribuição do valor das transações (Amount) é fortemente assimétrica à direita, concentrada em valores baixos.
- O volume de transações ao longo do tempo segue um padrão cíclico, compatível com os 2 dias cobertos pelo dataset.
- Transações fraudulentas apresentam maior variabilidade de valor dentro da faixa comum, quando comparadas a transações normais.
- A matriz de correlação identificou V17, V14, V12 e V10 como as variáveis com maior correlação negativa com fraude, e V11, V4, V2 e V19 com maior correlação positiva — mesmo com os dados anonimizados por PCA.

## Como executar

1. Clone este repositório.
2. Baixe o arquivo `creditcard.csv` no [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) (não incluído aqui por tamanho) e coloque na mesma pasta do notebook.
3. Instale as dependências: `pip install pandas numpy matplotlib`
4. Abra o notebook `fraudes.ipynb` no Jupyter ou VS Code.

## Autor

Arthur Martinoni
[LinkedIn](https://linkedin.com/in/ArthurMartinoni) | [GitHub](https://github.com/ArthurMartinoni)
