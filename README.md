## Categorização de Produtos - Classificação ML
Uma plataforma de infoprodutos estava com dificuldades de separar os produtos bons e os ruins de sua base de dados. De acordo com a regra de negócio da empresa, produtos com altas taxas de estorno, chargeback e alto volume de reclamações são considerados produtos ruins.

A classificação de produtos será criada para ajudar no monitoramento dos produtos e facilitar o acompanhamento mensal dos produtos com base nos seus indicadores. Assim, podendo definir metas para melhorar os produtos ativos e até utilizar para diferentes análises e tomadas de decisões. 

Portanto, o objetivo do projeto é categorizar de A a E, de forma hierárquica, os produtos de uma amostra com base no sua taxa de estorno, taxa de chargeback e o número de reclamações. Produtos da classe A apresentam os menores indicadores e a classe E os maiores indicadores.

Para isso, iremos avaliar uma amostra desses produtos e classificar por meio de um modelo KNN e um modelo de Árvore de Decisão para definir o melhor algoritmo de classificação.

#### **Tópicos do Projeto**

1. **Preparação do Ambiente**\
    1.1 Importação das bibliotecas\
    1.2 Leitura dos dados\
    1.3 Identificação de valores faltantes

2. **Análise Descritiva e Diagnóstica**\
    2.1 Análise Descritiva\
    2.2 Análise Diagnóstica

3. **Seleção de Variáveis Usando Testes Estatísticos**\
    3.1 Avaliação da Normalidade dos Dados\
    3.2 Seleção de Variáveis Quantitativas (ANOVA)

4. **Preparação dos Dados**\
    4.1 Balanceamento\
    4.2 Normalização

5. **Modelagem**\
    5.1 Divisão de Treino e Teste\
    5.2 Treinamento e Avaliação

6. **Exportando o Modelo**

Disponibilizei os dados, também, na plataforma Kaggle: https://www.kaggle.com/datasets/marianacaetano/indicadores-dos-produtos

##### **Dicionário das Variáveis**

* `produto_id`: Identificador do produto.
* `classificacao`: Classificação do produto pré definida.
* `tx_estorno`: Taxa de estorno.
* `reclamacoes`: Número de reclamações.
* `tx_chargeback`: Taxa de chargeback.