# METRO IMOB: Dashboard Comercial em Power BI

Painel de indicadores comerciais construído em Power BI para uma
imobiliária com equipe de vendas distribuída por região e canal.

🔗 [Ver relatório publicado](https://app.powerbi.com/view?r=eyJrIjoiNzI0MDkwMjAtMmZkYy00NzY4LTllNDAtNWVkNWRkMjg1NjljIiwidCI6IjY1OWNlMmI4LTA3MTQtNDE5OC04YzM4LWRjOWI2MGFhYmI1NyJ9)

---

## O Problema

A equipe comercial trabalhava com dados espalhados em planilhas soltas
e no sistema de vendas, sem nenhum painel único. Isso criava dois
problemas na prática: ninguém enxergava rápido quais regiões ou
vendedores estavam abaixo da meta, e as reuniões de resultado viravam
uma corrida atrás de números, cada gestor levava sua própria planilha,
muitas vezes com totais diferentes.

## Dados

- **Sistema de vendas**: receita, metas e ranking por vendedor
- **Excel**: metas históricas por período
- **CRM/ERP**: cadastro de clientes, região e canal

## Tratamento e Modelagem

Consolidação das fontes (Excel, CRM e ERP) num único modelo, com
tabelas fato e dimensão relacionadas por canal, região, vendedor e
período. Medidas em DAX para:

- % de meta atingida e variação mês a mês
- Ranking de vendedores e canais por receita
- Comparativos por região com filtros cruzados (período, cliente, tipo de produto)

## Tecnologias

| Camada | Tecnologia |
|---|---|
| Modelagem | Power BI Desktop, DAX |
| Fontes de dados | Excel/CSV, CRM, ERP |

## Dashboard

Layout dividido em blocos simples: visão geral, desempenho por canal,
ranking e análise regional, pensado pra um gestor entender em 10
segundos onde estão os problemas, sem precisar ler tabela.

**Próxima melhoria planejada:** filtro de setores para refinar a
visualização por segmento (Todos, Data, etc.).

## Principais Insights

Com o painel em tempo real, deu pra parar de discutir números na
reunião e começar a discutir ação, quem estava abaixo da meta já
chegava sinalizado, com histórico de evolução ao lado. Reduziu
bastante o retrabalho de montar relatório manual toda semana.

## Imagens

*(prints do dashboard em breve)*

## Como Reproduzir

Este painel foi construído no Power BI a partir de dados internos de
vendas (Excel, CRM e ERP, não públicos). Não há pipeline de código
associado, o relatório publicado acima permite exploração interativa
completa dos filtros e visualizações.
