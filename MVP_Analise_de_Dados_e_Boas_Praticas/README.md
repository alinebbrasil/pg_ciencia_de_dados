# MVP - Análise de Dados e Pré-Processamento do dataset Amazon Sales

## Descrição

Este projeto tem como objetivo a realização de uma análise exploratória e pré-processamento de dados utilizando um dataset de produtos da Amazon.

O trabalho foi desenvolvido como parte da disciplina de Análise Exploratória e Pré-Processamento de Dados, com foco na **compreensão da estrutura dos dados, identificação de padrões e preparação para possíveis etapas futuras de modelagem**.

---

## Objetivo

O principal objetivo deste MVP é analisar o comportamento de variáveis relacionadas a:

* Preços de produtos
* Descontos aplicados
* Avaliações dos usuários

Além disso, busca-se preparar os dados por meio de técnicas de pré-processamento, garantindo maior qualidade e consistência para análises futuras.

---

## Tecnologias Utilizadas

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Google Colab

---

## Fonte dos Dados

* Fonte: Kaggle (Amazon Sales Dataset)
* Dados incluem informações sobre produtos, preços, descontos e avaliações

---

## Hipóteses

Para orientar a análise, foram levantadas as seguintes hipóteses:

1. Produtos com menor preço tendem a possuir avaliações mais altas
2. Produtos com maior número de avaliações tendem a apresentar ratings mais elevados
3. Existem diferenças significativas de preço entre as categorias
4. Produtos com maiores descontos tendem a possuir melhores avaliações
5. Algumas categorias concentram a maior parte dos produtos

---

## Etapas do Projeto

* Análise Exploratória de Dados (EDA)
* Estatísticas descritivas
* Análise de distribuição (histogramas)
* Identificação de outliers (boxplots)
* Análise de correlação (matriz e mapa de calor)

---

## Pré-Processamento de Dados

* Tratamento de valores nulos
* Conversão de tipos de dados
* Remoção de colunas irrelevantes
* Normalização (MinMaxScaler)
* Padronização (StandardScaler)

---

## Principais Insights

* Forte correlação entre preço original e preço com desconto
* Baixa relação entre preço e avaliação dos produtos
* Distribuição de preços altamente assimétrica, com presença de outliers
* Diferenças significativas de preço entre categorias
* Concentração de produtos em determinadas categorias

---

## Conclusão

A análise demonstrou que fatores como preço e desconto não possuem relação direta com as avaliações dos produtos, indicando que a percepção de qualidade não depende exclusivamente do valor.

Por outro lado, a categoria dos produtos mostrou-se um fator relevante na definição de preços, evidenciando diferenças significativas entre os grupos analisados.

As etapas de pré-processamento foram fundamentais para garantir a qualidade dos dados, permitindo análises mais consistentes e preparando o dataset para possíveis aplicações futuras, como modelagem preditiva.

---

## Autora

**Aline Bastos Brasil**

Projeto acadêmico desenvolvido para fins educacionais.

