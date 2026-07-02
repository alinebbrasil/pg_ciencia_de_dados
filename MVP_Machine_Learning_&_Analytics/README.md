# MVP — Machine Learning & Analytics | Previsão de Churn de Clientes

## Descrição

Este projeto acadêmico consiste no desenvolvimento de um **MVP de Machine Learning**, no qual foi construída uma solução completa para **previsão de churn (cancelamento de clientes)** utilizando técnicas de classificação supervisionada.

O trabalho contempla todas as principais etapas de um projeto de Ciência de Dados, incluindo **análise exploratória dos dados (EDA)**, **pré-processamento**, **construção de pipelines**, **treinamento e comparação de modelos**, **otimização de hiperparâmetros** e **avaliação final**, seguindo boas práticas para garantir a reprodutibilidade dos experimentos e evitar vazamento de dados.

---

## Objetivo

O objetivo principal deste MVP é desenvolver um modelo de **Machine Learning** capaz de prever quais clientes possuem maior probabilidade de cancelar os serviços de uma empresa de telecomunicações.

Ao longo do projeto, buscou-se responder às seguintes questões:

* Quais características estão mais associadas ao churn?
* Como preparar adequadamente os dados para treinamento dos modelos?
* Qual algoritmo apresenta melhor desempenho para este problema?
* A otimização de hiperparâmetros produz ganhos relevantes de desempenho?
* Quais são as limitações da solução proposta?

As decisões metodológicas, limitações encontradas e oportunidades de melhoria são discutidas ao longo do notebook.

---

## Plataforma e Tecnologias Utilizadas

* **Plataforma:** Jupyter Notebook
* **Linguagem:** Python
* **Bibliotecas:** Pandas, NumPy, Matplotlib, Seaborn e Scikit-learn
* **Modelos:** DummyClassifier, Regressão Logística e Random Forest
* **Otimização:** GridSearchCV com validação cruzada
* **Controle de Versão:** Git e GitHub

---

## Fonte dos Dados

Os dados utilizados neste projeto correspondem ao conjunto **Telco Customer Churn**, amplamente utilizado para estudos de classificação em Machine Learning.

O dataset contém informações sobre clientes de uma empresa de telecomunicações, incluindo características demográficas, serviços contratados, forma de pagamento, tempo de permanência e a variável-alvo **Churn**, indicando se o cliente permaneceu ou cancelou o serviço.

---

## Etapas do Projeto

### 1. Entendimento do Problema

Foi realizada a definição do problema de negócio, identificação da variável-alvo e compreensão dos objetivos da previsão de churn.

---

### 2. Preparação dos Dados

Nesta etapa foram realizadas atividades como:

* carregamento do dataset;
* inspeção inicial dos dados;
* análise da estrutura das variáveis;
* identificação de valores ausentes;
* conversão de tipos de dados;
* organização do ambiente de trabalho.

---

### 3. Análise Exploratória dos Dados (EDA)

A análise exploratória permitiu compreender o comportamento das variáveis e sua relação com o cancelamento dos clientes.

Foram realizadas análises envolvendo:

* distribuição das variáveis;
* análise de valores ausentes;
* comparação entre clientes que permaneceram e cancelaram;
* análise das variáveis categóricas e numéricas;
* identificação de possíveis padrões relacionados ao churn.

---

### 4. Pré-processamento

Foi desenvolvido um pipeline completo de preparação dos dados utilizando o **Scikit-learn Pipeline** e **ColumnTransformer**.

Entre as transformações realizadas destacam-se:

* imputação de valores ausentes;
* padronização das variáveis numéricas;
* codificação das variáveis categóricas com OneHotEncoder;
* separação entre treino e teste utilizando Holdout Estratificado.

---

### 5. Construção e Avaliação dos Modelos

Foram treinados diferentes modelos de classificação:

* DummyClassifier (baseline);
* Regressão Logística;
* Random Forest.

Os modelos foram comparados utilizando as métricas:

* Acurácia;
* Precisão;
* Recall;
* F1-score.

Também foram analisadas as respectivas matrizes de confusão.

---

### 6. Otimização de Hiperparâmetros

Foi realizada uma etapa de otimização da **Random Forest** utilizando **GridSearchCV** com validação cruzada de 5 folds.

Foram avaliadas diferentes combinações de hiperparâmetros buscando melhorar o equilíbrio entre Precisão e Recall por meio do **F1-score**, métrica principal adotada neste projeto.

---

### 7. Avaliação Final

Após a comparação entre os modelos e a etapa de otimização, foi selecionado o modelo de melhor desempenho para avaliação final utilizando exclusivamente o conjunto de teste.

Também foram discutidos:

* análise dos erros;
* possíveis sinais de overfitting e underfitting;
* limitações da solução;
* oportunidades para trabalhos futuros.

---

## Estrutura do Repositório

```text
MVP_Machine_Learning_&_Analytics/
│
├── Telco-Customer-Churn.csv
├── MVP_Machine_Learning_&_Analytics.ipynb
└── README.md
```

---

## Principais Resultados

Os experimentos demonstraram que todos os modelos candidatos superaram o **DummyClassifier**, indicando capacidade de aprender padrões relevantes presentes nos dados.

Após a comparação entre os algoritmos avaliados, a **Regressão Logística** apresentou o melhor desempenho geral, obtendo:

* **Acurácia:** 80,55%
* **Precisão:** 65,72%
* **Recall:** 55,88%
* **F1-score:** 60,40%

A **Random Forest** apresentou melhorias significativas após a otimização de hiperparâmetros utilizando **GridSearchCV**, tornando-se uma alternativa competitiva, embora tenha permanecido ligeiramente abaixo da Regressão Logística na métrica principal utilizada neste estudo.

Todas as análises, gráficos e discussões metodológicas encontram-se documentados diretamente no notebook.

---

## Autoavaliação

O desenvolvimento deste MVP permitiu aplicar, de forma prática, conceitos fundamentais de **Machine Learning**, incluindo preparação de dados, construção de pipelines, avaliação de modelos, validação cruzada e otimização de hiperparâmetros.

Além dos aspectos técnicos, o projeto reforçou a importância da documentação das decisões metodológicas, da interpretação crítica dos resultados e da utilização de boas práticas para garantir a reprodutibilidade dos experimentos.

Como trabalhos futuros, o projeto pode ser expandido com:

* avaliação de novos algoritmos de classificação;
* utilização de técnicas de balanceamento das classes;
* ampliação do espaço de busca de hiperparâmetros;
* validação utilizando novos conjuntos de dados;
* implantação do modelo em uma aplicação web para realização de previsões.

---

## Autora

**Aline Bastos Brasil**

Projeto acadêmico desenvolvido para fins educacionais como parte da disciplina **Machine Learning & Analytics** da **Pontifícia Universidade Católica do Rio de Janeiro (PUC-Rio)**.
