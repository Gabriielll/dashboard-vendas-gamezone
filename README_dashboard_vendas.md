# Dashboard de Vendas – GameZone

Dashboard em Excel que transforma dados brutos de vendas em indicadores e gráficos para analisar o desempenho e apoiar decisões.

**Arquivo:** `dashboard_vendas.xlsx`

## O que o dashboard mostra

- **Indicadores:** receita total, lucro total, margem de lucro, nº de vendas e ticket médio.
- **Gráficos:** receita e lucro por mês, receita por categoria, top 5 produtos, receita por região, receita por canal e lucro por categoria.
- **Filtros:** Ano e Região (células `D5` e `I5`), que atualizam todos os indicadores e gráficos.

## Dados utilizados

Base **fictícia** de 900 vendas (jan/2024 a dez/2025) de uma loja de games, gerada para fins educacionais, na aba **Base**.

| Coluna | Descrição |
|---|---|
| ID Pedido, Data | Identificação e data da venda |
| Ano, Mês | Calculados a partir da data |
| Produto, Categoria | 11 produtos em 4 categorias (Consoles, Jogos, Acessórios, Assinaturas) |
| Região, Canal | 5 regiões e 3 canais (Online, Loja Física, Marketplace) |
| Quantidade, Preço Unitário, Custo Unitário | Dados de entrada |
| Receita, Lucro | Calculados: Quantidade × Preço; Receita − Quantidade × Custo |

## Estrutura da planilha

| Aba | Função |
|---|---|
| Dashboard | Indicadores, filtros e gráficos |
| Base | Dados em tabela (`tb_vendas`) |
| Apoio | Tabelas de cálculo (SUMIFS, COUNTIFS, INDEX/MATCH, LARGE) que alimentam os gráficos |
| Sobre | Documentação resumida dentro da planilha |

Intervalos nomeados: `b_ano`, `b_mes`, `b_produto`, `b_categoria`, `b_regiao`, `b_canal`, `b_qtd`, `b_receita`, `b_lucro`, `crit_ano`, `crit_regiao`, `lista_ano`, `lista_regiao`.

## Como reproduzir

1. Crie a aba **Base** e transforme os dados em tabela (Ctrl+T).
2. Adicione as colunas calculadas de Ano, Mês, Receita e Lucro.
3. Crie nomes para as colunas da base (ex.: `b_receita`).
4. Na aba **Apoio**, monte tabelas por mês, categoria, região, canal e produto com `SUMIFS`, usando critérios que respondem aos filtros (`">0"` para "Todos" no ano e `"*"` para "Todas" na região).
5. Gere o Top 5 com `LARGE` + `INDEX/MATCH`.
6. No **Dashboard**, crie os filtros com validação de dados e os cartões de indicadores.
7. Insira os gráficos apontando para as tabelas da aba Apoio.

Para usar outra base, cole os dados na aba Base mantendo as colunas e ajuste os intervalos nomeados e as listas de filtros.

## Prints

Coloque as capturas de tela na pasta `/images` (ex.: `dashboard_geral.png`, `dashboard_filtrado.png`).
