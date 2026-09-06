# Dataset-Netflix-Quality
# Diagnóstico de Qualidade de Dados — Netflix Movies and TV Shows

Análise exploratória com foco em diagnóstico de qualidade de dados, desenvolvida como resumo de Iniciação Científica (Ciência de Dados).

## Sobre o projeto

Este trabalho investiga o estado de qualidade do dataset público *Netflix Movies and TV Shows* (Kaggle), identificando valores ausentes, colunas com tipo de dado incorreto e inconsistências de formatação — especialmente na coluna de datas (`date_added`), que revelou problemas não visíveis em uma checagem simples de valores nulos.

## Dataset

- **Nome:** Netflix Movies and TV Shows
- **Fonte:** [Kaggle](https://www.kaggle.com/) — autor Shivam Bansal
- **Tamanho:** 8.807 registros, 12 variáveis

## Tecnologias utilizadas

- Python
- Pandas

## Funções principais aplicadas

`read_csv()`, `shape`, `dtypes`, `isnull()`, `to_datetime()`, `isna()`, `sort_values()`

## Principais achados

- A coluna `director` apresentou o maior percentual de valores ausentes (29,9%).
- A coluna `date_added`, com apenas 10 nulos originais, revelou 98 registros com datas inválidas após conversão de tipo — um problema de formatação oculto na checagem inicial.
