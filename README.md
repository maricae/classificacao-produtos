## Categorização de Produtos - Classificação (Machine Learning)

<img src="https://cdn-images-1.medium.com/max/1600/1*leQNkzi9oo3nu1PPMvtHyQ.jpeg" alt="drawing" width="800"/>

Uma plataforma de infoprodutos estava com dificuldades de separar os produtos bons e os ruins de sua base de dados. De acordo com a regra de negócio da empresa, produtos com altas taxas de estorno, chargeback e alto volume de reclamações são considerados produtos ruins.

A classificação dos produtos será criada para ajudar no monitoramento dos produtos e facilitar o acompanhamento mensal com base nos seus indicadores. Assim, podendo definir metas para melhorar os produtos ativos e até utilizá-las para diferentes análises e tomadas de decisões. 

Portanto, o objetivo do projeto é categorizar de A a E, de forma hierárquica, os produtos de uma amostra com base na sua taxa de estorno, taxa de chargeback e o número de reclamações. Produtos da classe A apresentam os menores indicadores e a classe E os maiores indicadores.

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

##

### Dicionário das Variáveis:

* `produto_id`: Identificador do produto.
* `classificacao`: Classificação do produto pré definida.
* `tx_estorno`: Taxa de estorno.
* `reclamacoes`: Número de reclamações.
* `tx_chargeback`: Taxa de chargeback.

##

### Requisitos:
1. [Pandas](https://pandas.pydata.org/docs/): para leitura e manipulação de dados

2. [Numpy](https://numpy.org/): para realizar calculos e operações de manipulação de estrutura de dados

3. [Matplotlib](https://matplotlib.org/): para visualização de dados

4. [Seaborn](https://seaborn.pydata.org/): para visualização de dados

5. [Imblearn](https://imbalanced-learn.org/stable/): para realizar o método de balanceamento de classes

6. [Scikit-learn](https://scikit-learn.org/stable/install.html): para criação de modelos de machine learning

7. [Scipy](https://scipy.org/install/): para realizar testes estatísticos

8. [Joblib](https://joblib.readthedocs.io/en/stable/): para exportar o modelo
