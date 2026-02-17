# Classificação de Risco de Produtos  
## Machine Learning aplicado a Compliance e Monitoramento de Performance

Este projeto tem como objetivo classificar produtos digitais de uma plataforma de infoprodutos em categorias de risco (A a E), com base em indicadores operacionais e de qualidade.

A solução foi desenvolvida para apoiar o time de compliance na priorização de análises e no monitoramento contínuo da qualidade dos produtos.

## ➡️ Problema de Negócio

Produtos com:

- Altas taxas de estorno
- Elevadas taxas de chargeback
- Grande volume de reclamações

representam risco financeiro e reputacional para a plataforma.

O objetivo é transformar esses indicadores em uma **classificação estruturada de risco**, permitindo:

- Monitoramento mensal padronizado
- Priorização de análise manual
- Definição de metas de melhoria
- Apoio à tomada de decisão estratégica

## ➡️ Estrutura da Classificação

Os produtos são classificados de forma hierárquica:

- **Classe A** → menor risco
- **Classe B**
- **Classe C**
- **Classe D**
- **Classe E** → maior risco

A categorização é baseada nos seguintes indicadores:

- `tx_estorno` (taxa de estorno)
- `tx_chargeback` (taxa de chargeback)
- `reclamacoes` (volume de reclamações)

## ➡️ Abordagem Metodológica

### 1. Análise Exploratória

- Estatísticas descritivas
- Identificação de outliers
- Avaliação de distribuição das variáveis
- Diagnóstico de normalidade (Shapiro-Wilk e Kolmogorov-Smirnov)

### 2. Seleção de Variáveis

- Testes estatísticos (ANOVA)
- Avaliação da relevância das variáveis preditoras
- Redução de dimensionalidade quando necessário

### 3. Preparação dos Dados

- Tratamento de valores ausentes
- Normalização das variáveis
- Balanceamento das classes (Imbalanced-learn)

### 4. Modelagem

Modelos utilizados:

- K-Nearest Neighbors (KNN)
- Árvore de Decisão

Procedimentos:

- Divisão treino/teste
- Avaliação comparativa de desempenho
- Validação do modelo selecionado
- Exportação do modelo com `joblib`

## ➡️ Avaliação

A avaliação considerou:

- Acurácia
- Precisão
- Recall
- F1-Score

A escolha do modelo final levou em conta:

- Capacidade de discriminar classes de maior risco
- Interpretação dos resultados
- Estabilidade do desempenho

## ➡️ Discussões Técnicas

- O balanceamento foi essencial para evitar viés em classes majoritárias.
- A normalização impactou diretamente o desempenho do KNN.
- Modelos mais simples podem ser preferíveis quando interpretabilidade é relevante para compliance.

Extensões possíveis incluem:

- Random Forest ou Gradient Boosting
- Análise de importância de variáveis
- Ajuste de thresholds por nível de risco
- Monitoramento temporal do score

## ➡️ Dicionário de Variáveis

- `produto_id`: Identificador único do produto
- `classificacao`: Classe alvo (A a E)
- `tx_estorno`: Taxa de estorno
- `tx_chargeback`: Taxa de chargeback
- `reclamacoes`: Número de reclamações

## ➡️ Tecnologias Utilizadas

### Linguagem
- Python

### Manipulação e Análise
- Pandas
- NumPy

### Visualização
- Matplotlib
- Seaborn

### Modelagem
- Scikit-learn
- Imbalanced-learn

### Estatística
- SciPy

### Exportação de Modelo
- Joblib



