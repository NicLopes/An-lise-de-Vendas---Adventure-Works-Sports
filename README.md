# 🏪 Análise de Vendas - Adventure Works Sports
Análise exploratória de dados de uma empresa de artigos esportivos, cobrindo o período de 2014 a 2016. O projeto integra quatro datasets (vendas, produtos, clientes e territórios) e explora dimensões de produto, geografia e sazonalidade, com foco em insights orientados a negócio.

#🛠️ Ferramentas e Tecnologias

Python — Pandas, Plotly Express, Plotly Graph Objects, Matplotlib
Jupyter Notebook
Excel — fonte dos dados brutos


# 📂 Estrutura do Projeto
analise_sport/
│
├── analise_sport.ipynb       # Notebook principal com análises e visualizações
├── Customer.xlsx             # Dados demográficos dos clientes
├── Product.xlsx              # Catálogo de produtos
├── Sales.xlsx                # Transações de vendas
├── Territories.xlsx          # Regiões e países
└── README.md

# 🔧 Etapas de Limpeza e Preparação

Tratamento de valores nulos por categoria: preenchimento com "Unknown", "Not Specified" e "No description" conforme contexto
Imputação de valores numéricos ausentes (StandardCost, ListPrice) pela mediana
Merge dos quatro datasets em um único DataFrame consolidado (df_sport)
Remoção de colunas irrelevantes para a análise
Criação de colunas derivadas: Profit, Margem_%, Month, Year


# 📊 Análises Desenvolvidas
Produto

Top 10 produtos por faturamento com escala de margem de lucro
Faturamento e margem por categoria (gráfico combinado barra + linha)
Scatter de Volume x Rentabilidade com linhas de referência de média

## Geografia

Faturamento e lucro por país
Participação percentual de faturamento por país (donut chart)
Evolução anual do faturamento por país (2014–2016)

## Temporal

Evolução mensal do faturamento agregado
Mês de maior faturamento por ano
Top 10 dias com maior volume de vendas


## 📌 Principais Insights

Estados Unidos e Austrália concentram 62,9% do faturamento total, evidenciando distribuição geográfica desigual da receita
2016 registrou recuperação expressiva após retração em 2015, com forte sazonalidade no último trimestre do ano
Bikes lidera em faturamento absoluto, mas Accessories apresenta a maior margem proporcional entre as categorias — volume elevado não garante maior rentabilidade
Esse padrão se inverte no nível de produto individual: os itens de maior faturamento tendem a apresentar também as maiores margens
Os maiores volumes de vendas se concentram nos últimos dias do mês e no último trimestre do ano, refletindo ciclos de pagamento e sazonalidade de fim de ano
