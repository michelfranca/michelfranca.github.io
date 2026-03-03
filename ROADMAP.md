# 🗺️ Meu Roadmap para Especialista em Dados & Business Intelligence

Este documento detalha a trilha de estudos que estou seguindo para me tornar um especialista em BI, com foco em análise, visualização e estratégia de dados.

**Como usar:** Este é um checklist vivo. Conforme avanço nos estudos, marco os itens concluídos com `[x]`.

[< Voltar para a Home](./README.md)

---

## ✅ Fase 1: A Fundação Sólida (Meses 1-3)
*O alicerce de um bom analista está na sua capacidade de entender e manipular os dados em sua origem.*

### SQL para Análise de Dados (Nível Especialista)
- [ ] **Fundamentos:** `SELECT`, `FROM`, `WHERE`, `DISTINCT`, `AS`, `ORDER BY`, `LIMIT`.
- [ ] **Filtragem Avançada:** `BETWEEN`, `IN`, `LIKE`, `IS NULL`.
- [ ] **Junção de Dados:** `INNER JOIN`, `LEFT JOIN`, `RIGHT JOIN`, `FULL OUTER JOIN`, `UNION`, `UNION ALL`.
- [ ] **Agregação e Agrupamento:** `GROUP BY`, `HAVING`, e funções de agregação (`COUNT`, `SUM`, `AVG`, `MAX`, `MIN`).
- [ ] **Subqueries (Subconsultas):** Utilização de `SELECT` dentro de `WHERE`, `FROM` ou `SELECT`.
- [ ] **Funções de Janela (Window Functions):** `ROW_NUMBER`, `RANK`, `DENSE_RANK`, `LEAD`, `LAG`, `SUM() OVER (PARTITION BY ...)`.
- [ ] **Expressões de Tabela Comuns (CTEs - Common Table Expressions):** Uso do `WITH` para organizar consultas longas.
- [ ] **Manipulação de Tipos de Dados:** Funções de data (`DATE_TRUNC`, `EXTRACT`), texto (`CONCAT`, `SUBSTRING`) e conversão (`CAST`).

### Modelagem de Dados Dimensional (Conceitos de Data Warehouse)
- [ ] **Diferenciar OLTP vs. OLAP:** Entender sistemas transacionais vs. analíticos.
- [ ] **Tabelas Fato:** Granularidade e tipos de métricas (aditivas, semi-aditivas, não aditivas).
- [ ] **Tabelas Dimensão:** Chaves primárias e estrangeiras, atributos descritivos.
- [ ] **Esquemas:**
  - [ ] **Star Schema (Esquema Estrela):** O modelo ideal para Power BI.
  - [ ] **Snowflake Schema (Floco de Neve):** Quando e por que usar (e quando evitar).
- [ ] **Slowly Changing Dimensions (SCD):** Tipos 1, 2 e 3 para rastrear mudanças históricas.

### Certificação PL-900: Microsoft Power Platform Fundamentals
- [ ] **Módulo 1: Power Platform:** Componentes (Power BI, Power Apps, Power Automate, Power Virtual Agents), Conectores e Dataverse.
- [ ] **Módulo 2: Power BI:** Identificar os componentes e usos do serviço do Power BI e do Desktop.
- [ ] **Módulo 3: Power Apps:** Identificar os componentes e usos de Canvas Apps e Model-Driven Apps.
- [ ] **Módulo 4: Power Automate:** Identificar os componentes e usos dos fluxos de nuvem.
- [ ] **Módulo 5: Soluções Complementares:** Power Virtual Agents e AI Builder.
- [ ] **Status:** [Não iniciado]
- [ ] **Data da Prova:** [A agendar]
- [ ] **Resultado:** [Aguardando]

---

## ✅ Fase 2: Especialização em Power BI (Meses 4-7)
*Mergulho profundo na principal ferramenta de visualização e análise do mercado, cobrindo todos os domínios da certificação PL-300.*

### Certificação PL-300: Microsoft Power BI Data Analyst
- [ ] **Preparar os Dados (ETL com Power Query / Linguagem M)**
  - [ ] **Conectar a Fontes de Dados:** Bancos de dados, arquivos (Excel, CSV), pastas, fontes web.
  - [ ] **Limpeza e Transformação:** Remover erros, substituir valores, `Unpivot/Pivot`, dividir colunas, alterar tipos de dados.
  - [ ] **Estruturação de Dados:** `Append` (anexar) vs. `Merge` (mesclar) consultas.
  - [ ] **Parâmetros:** Criar parâmetros para dinamizar fontes de dados.
  - [ ] **Otimização:** Entender e aplicar o conceito de `Query Folding`.

- [ ] **Modelar os Dados (Relacionamentos e DAX)**
  - [ ] **Design do Modelo:** Configurar relacionamentos (cardinalidade e direção do filtro). Implementar Star Schema.
  - [ ] **DAX - Data Analysis Expressions:**
    - [ ] **Fundamentos:** Colunas Calculadas vs. Medidas. Contexto de Linha vs. Contexto de Filtro.
    - [ ] **Funções Iteradoras (X-Functions):** `SUMX`, `AVERAGEX`, `MAXX`.
    - [ ] **A Função Mestra - `CALCULATE`:** Dominar a manipulação do contexto de filtro.
    - [ ] **Funções de Filtro:** `FILTER`, `ALL`, `ALLEXCEPT`, `KEEPFILTERS`.
    - [ ] **Inteligência de Tempo:** `DATESYTD`, `PREVIOUSMONTH`, `SAMEPERIODLASTYEAR` (requer Tabela Calendário).
    - [ ] **Funções de Relacionamento:** `RELATED` e `USERELATIONSHIP`.
    - [ ] **Variáveis (VAR):** Organizar e otimizar fórmulas DAX.

- [ ] **Visualizar e Analisar os Dados (Criação de Relatórios)**
  - [ ] **Design e Interatividade:** Escolha de visuais, `Bookmarks` (indicadores) e `Drillthrough`.
  - [ ] **Recursos de Análise:** Linhas de tendência, previsão (forecasting), análise de anomalias.
  - [ ] **Visuais com IA:** Q&A (Perguntas e Respostas), Principais Influenciadores, Árvore de Decomposição.

- [ ] **Gerenciar Ativos no Serviço do Power BI**
  - [ ] **Workspaces, Apps e Compartilhamento.**
  - [ ] **Atualização de Dados:** Configurar `Gateway` e agendar atualizações.
  - [ ] **Segurança:** Implementar `Row-Level Security` (RLS) estática e dinâmica.
- [ ] **Status:** [Não iniciado]
- [ ] **Data da Prova:** [A agendar]
- [ ] **Resultado:** [Aguardando]

---

## ✅ Fase 3: Automação e Diferenciais (Meses 8-10)
*Indo além do BI tradicional para criar soluções mais eficientes e robustas.*

### Power Automate para Analistas de Dados
- [ ] **Gatilhos e Ações:** Entender os conceitos fundamentais.
- [ ] **Fluxos Automatizados:** Ex: Quando um arquivo chegar em uma pasta, iniciar a atualização do dataset do Power BI.
- [ ] **Integração com Power BI:** Criar alertas de dados que disparam fluxos.

### Python para Análise de Dados
- [ ] **Ambiente:** Configurar VS Code com Jupyter Notebooks.
- [ ] **Pandas:** Manipulação de DataFrames, limpeza, `groupby`, `merge`.
- [ ] **Integração com Power BI:**
  - [ ] Usar scripts Python como fonte de dados.
  - [ ] Usar scripts Python para transformações no Power Query.
  - [ ] Criar visuais com Matplotlib/Seaborn no Power BI.

---

## ✅ Fase 4: Portfólio e Projetos Práticos (Contínuo)
*Conhecimento aplicado é o que gera valor. Esta seção será um link para a página de projetos.*

- [ ] **Projeto 1: Análise de Vendas**
- [ ] **Projeto 2: Análise de RH**
- [ ] **Projeto 3: Análise Financeira**

[< Voltar para a Home](./README.md)
