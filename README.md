# Alura_Data-Science
Desafio Alura
Análise de Desempenho de Lojas - AluraStore Brasil

Visão Geral do Projeto

Este projeto consiste em uma análise exploratória de dados (EDA) de quatro lojas da rede fictícia "AluraStore Brasil". O objetivo principal é fornecer uma recomendação de negócios baseada em dados para a gestão (Sr. João) sobre qual das quatro unidades deve ser vendida, visando a otimização das operações e a consolidação dos ativos mais rentáveis.

O notebook AluraStoreBrasil (1).ipynb contém todo o processo de análise, desde a importação e limpeza dos dados até a geração de visualizações e o relatório final.

Fonte dos Dados

Os dados foram fornecidos pela Alura e estão divididos em quatro arquivos CSV, cada um representando uma loja:

loja_1.csv

loja_2.csv

loja_3.csv

loja_4.csv

O conjunto de dados consolidado inclui as seguintes colunas:
Produto, Categoria do Produto, Preço, Frete, Data da Compra, Vendedor, Local da compra, Avaliação da compra, Tipo de pagamento, Quantidade de parcelas, lat, lon e Loja.

Metodologia e Análises Realizadas

A análise foi estruturada em várias etapas para garantir uma visão completa do desempenho de cada loja:

Consolidação dos Dados: Os quatro arquivos CSV foram importados e unificados em um único DataFrame (df_completo), com a adição de uma coluna Loja para identificar a origem de cada registro.

Análise de Faturamento: Cálculo do faturamento total da rede e o faturamento individual de cada loja.

Vendas por Categoria: Contagem de vendas e análise de faturamento por categoria de produto para identificar as mais populares.

Média de Avaliação: Cálculo da média de satisfação dos clientes (de 1 a 5) para cada loja.

Produtos Mais/Menos Vendidos: Identificação dos 5 produtos mais e menos vendidos em toda a rede.

Custo de Logística: Análise do frete médio cobrado por cada loja.

Análise Temporal: Verificação da tendência de faturamento ao longo do tempo (mensal).

Análise Geográfica (Extra): Mapeamento das vendas usando latitude e longitude para identificar concentrações geográficas.

Ferramentas Utilizadas

Python 3

Pandas: Para importação, manipulação e análise dos dados.

Matplotlib: Para a geração de visualizações (Gráficos de Pizza e Linha).

Seaborn: Para a geração de visualizações estatísticas (Gráficos de Barras e Dispersão).

Jupyter Notebook (Google Colab): Como ambiente para a análise.

Principais Descobertas e Visualizações

A análise gerou diversos insights, consolidados nos seguintes gráficos:

faturamento_por_loja.png (Gráfico de Barras): Mostra que as lojas 1, 2 e 3 têm desempenho de faturamento similar e robusto, enquanto a Loja 4 fatura significativamente menos.

vendas_por_categoria_pizza.png (Gráfico de Pizza): Revela as categorias mais populares (Top 5 + Outros), com "eletronicos", "moveis" e "brinquedos" liderando as vendas.

faturamento_ao_longo_do_tempo.png (Gráfico de Linha): Demonstra a tendência de faturamento mensal de toda a rede, mostrando picos e vales sazonais.

analise_geografica_dispersao.png (Gráfico de Dispersão): Mapeia a localização de todas as vendas, diferenciando por loja (cor) e valor (tamanho), ajudando a visualizar o alcance geográfico de cada unidade.

Descoberta Chave: A avaliação média das lojas é quase idêntica (entre 3.98 e 4.05), indicando que a qualidade do serviço é consistente e não é um fator decisivo para a escolha da loja a ser vendida.

Conclusão e Recomendação

Com base na análise de desempenho, a recomendação é a venda da Loja 4.

Justificativa: O fator decisivo para esta recomendação é o desempenho financeiro. A Loja 4 apresenta o menor faturamento entre as quatro unidades, tornando-a a candidata lógica para desinvestimento. A venda desta unidade permitirá à gestão focar esforços e capital nas lojas mais lucrativas (1, 2 e 3), otimizando a rentabilidade geral da operação.

Como Replicar a Análise

Clone este repositório.

Certifique-se de ter as bibliotecas Python (pandas, matplotlib, seaborn) instaladas.

Abra o arquivo AluraStoreBrasil (1).ipynb em um ambiente como Jupyter Notebook ou Google Colab.

Execute as células na ordem apresentada para carregar os dados, realizar as análises e gerar os gráficos.
