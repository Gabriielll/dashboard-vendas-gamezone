Dashboard de Vendas – GameZone

Dashboard em Excel que transformar dados de vendas de em indicadores e bruto para gráficos o desempenho de análise e apoio de defesa.

Arquivo: dashboard_vendas.xlsx
O que o painel de discussão

    Indicadores: total, total do lucro, margem de lucro, no de vendas e ticket médio.
    Gráficos: receita e e lucro por lucro, mês por categoria, top 5, receitas por produtos, região por canal e lucro por categoria.
    Filtros: Ano e Região (células D5e I5), que atualizar todos os indicadores e gráficos.

Dados utilizados

Base fictícia de 900 vendas (jan/2024 a dez/2025) de loja uma de jogos, para geradas fintas educacional, Basena aba Base.
Categoria: Coluna 	Descrição
ID Pedido, Dados 	Identificação e dados da venda
Ano, Mês 	Calculados a partir da da dados
Produtor, 	11 produtos em categorias (Consoles, Jogos, Acessórios, Assinaturas)
Região, Canal 	5 regiões e 3 canais (Online, Loja Física, Marketplace)
Preços Unitários, Custo Unitário 	Dados de entrada
Receita, Lucro 	Cálculos: Quantidade × Preço; Receita − × Custo
Estrutura da planilha
Aba 	Função
Painel 	Indicadores, filtros e gráficos
Base 	Dados em tabela (tb_vendas)
Apoio 	Tabelas de (SUMIFS, COUNTI, INDEX/MATCH, LARGE) que alimentarm os gráficos
Sobre 	Documentação resumidada dentro da planilha

Intervalos nomeias: b_ano, b_mes, b_produto, b_categoria, b_regiao, b_canal, b_qtd, b_receita, b_lucro, crit_ano, crit_regiao, lista_ano, lista_regiao.
Como reproduzir

    Crie a aba Base e transforme os dados em (Ctrl+T).
    Adigo ass colunas de Ano, Mês, Receita e Lucro.
    Crie nomes para as colunas da base (ex.: b_receita).
    Na aba Apoio, monte tabelas por categoria, mês, região, canal e com produto SUMIFS, utilizar critérios que aos responder filtros ( ">0"para "Todos" no ano e "*"para "Todas" na região).
    Gere o Top 5 com LARGE+ INDEX/MATCH.
    No Dashboard, cry os filtros com validação de dados e os cartões de indicadores.
    Insira os gráficos de apontar para como do apoio do apoio.

Para usar outra base, cole os dados na aba Base como ajuste e oss intervalos de manutenção nomeados e como listas de filtros.
Impressões

Abordar como capturas de tela de massa na /images(ex.: dashboard_geral.png, dashboard_filtrado.png).
