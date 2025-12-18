# MVP — Pipeline de Dados e Análise com Olist

## 📌 Descrição

Este projeto acadêmico consiste no desenvolvimento de um **MVP de Engenharia de Dados**, no qual foi construído um **pipeline de dados em nuvem** contemplando as etapas de **busca, coleta, modelagem, carga e análise de dados**.

O trabalho utiliza dados públicos da empresa **Olist**, amplamente conhecidos no contexto de e-commerce brasileiro, com o objetivo de explorar, organizar e analisar informações relacionadas a pedidos, clientes, produtos e pagamentos.

---

## 🎯 Objetivo

O objetivo principal deste MVP é demonstrar, na prática, a construção de um pipeline de dados funcional, aplicando conceitos de **Engenharia de Dados** e **Análise de Dados**.

A partir do conjunto de dados da Olist, o projeto busca responder, entre outras, às seguintes perguntas:

* Como se distribuem os pedidos ao longo do tempo?
* Quais são os estados e cidades com maior volume de pedidos?
* Quais categorias de produtos apresentam maior volume de vendas?
* Qual o comportamento dos pagamentos (formas de pagamento e valores)?

Nem todas as perguntas necessariamente precisam ser respondidas integralmente. As limitações encontradas e os objetivos não atingidos são discutidos na seção de **Autoavaliação**.

---

## ☁️ Plataforma e Tecnologias Utilizadas

* **Plataforma:** Databricks (Community Edition)
* **Linguagem:** Python
* **Bibliotecas:** Pandas, NumPy, Matplotlib, Seaborn
* **Ambiente de Desenvolvimento:** Jupyter Notebook
* **Controle de Versão:** Git e GitHub

---

## 📂 Fonte dos Dados

Os dados utilizados neste projeto são públicos e foram obtidos a partir do **Kaggle**, no dataset:

**Brazilian E-Commerce Public Dataset by Olist**

Este conjunto de dados contém informações anonimizadas sobre pedidos realizados na plataforma Olist, incluindo dados de clientes, vendedores, produtos, pagamentos e avaliações.

---

## 🔍 Etapas do Projeto

### 1️⃣ Busca e Coleta dos Dados

Os arquivos foram obtidos diretamente do Kaggle e armazenados no ambiente em nuvem para posterior processamento. Por se tratar de um dataset público e estruturado, não foi necessário realizar web scraping.

### 2️⃣ Modelagem dos Dados

Os dados foram organizados seguindo uma abordagem semelhante a um **Data Lake**, mantendo os arquivos separados por conceito (clientes, pedidos, produtos, pagamentos, etc.).

Foi realizada a análise da estrutura de cada conjunto de dados, incluindo:

* Tipos de dados;
* Chaves de relacionamento;
* Valores esperados para atributos numéricos e categóricos.

### 3️⃣ Carga e Transformações

Durante esta etapa, foram realizadas transformações como:

* Limpeza de dados;
* Conversão de tipos;
* Junção de tabelas relacionadas;
* Criação de novas variáveis auxiliares para análise.

As transformações foram documentadas diretamente no notebook por meio de células de código e comentários explicativos.

### 4️⃣ Análise de Dados

A análise foi dividida em duas partes:

#### a) Qualidade dos Dados

Foi realizada uma verificação de:

* Valores nulos;
* Inconsistências;
* Distribuição dos dados por atributo.

Mesmo tratando-se de um dataset relativamente bem estruturado, a análise exploratória foi essencial para validar a confiabilidade das informações.

#### b) Solução do Problema

Foram aplicadas análises exploratórias e visualizações para responder às perguntas definidas no objetivo do projeto. Os resultados obtidos foram discutidos ao longo do notebook, conectando os dados analisados ao problema proposto.

---

## 📦 Estrutura do Repositório

```
pg_ciencia_de_dados/
│
├── MVP_Engenharia_de_Dados/
│   └── MVP_Engenharia_de_Dados.ipynb
│
└── README.md
```

---

## 📊 Resultados

Os resultados incluem análises estatísticas e visualizações que permitem compreender melhor o comportamento dos pedidos, clientes e pagamentos na plataforma Olist.

As evidências das análises estão disponíveis diretamente no notebook, por meio de gráficos e tabelas.

---

## 📝 Autoavaliação

O desenvolvimento deste MVP permitiu aplicar, de forma prática, os conceitos de Engenharia de Dados vistos ao longo da disciplina.

Os principais desafios estiveram relacionados à compreensão do volume de dados, à modelagem adequada das tabelas e à definição das análises mais relevantes.

Como trabalhos futuros, o projeto pode ser expandido com:

* Implementação de pipelines automatizados de ETL;
* Integração com ferramentas de visualização como Power BI ou Tableau.

---

## 👩‍🎓 Autora

**Aline Bastos Brasil**

Projeto acadêmico desenvolvido para fins educacionais.
