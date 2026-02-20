---
layout: default
title: Power BI
nav_order: 3
has_children: false
permalink: /powerbi
---

# Roadmap de Estudos: Power BI - Do Zero ao Expert em Dashboards

Este roadmap foi criado para guiar seus estudos em Power BI, desde os conceitos mais básicos de conexão com dados até as técnicas avançadas de modelagem, performance e governança exigidas em grandes corporações.

O progresso é atualizado manualmente editando este arquivo no GitHub e marcando `[ ]` como `[x]`.

---

## 🚀 Nível Júnior: Construindo os Primeiros Dashboards
*O objetivo é se tornar autônomo na criação de relatórios funcionais, desde a importação dos dados até a publicação.*

### 1. Fundamentos e Ambiente Power BI
- [ ] O que é Business Intelligence (BI) e o papel do Power BI?
- [ ] Os componentes do ecossistema: Power BI Desktop, Power BI Service (Online) e Power BI Mobile.
- [ ] Navegando pela interface do Power BI Desktop: As 3 visões (Relatório, Dados, Modelo).

### 2. Conexão e Tratamento de Dados (Power Query)
- [ ] Conectando a fontes de dados: Excel, CSV, Pastas e Bancos de Dados (SQL).
- [ ] A interface do Power Query Editor: O coração do ETL.
- [ ] Transformações essenciais: Remover/Renomear colunas, alterar tipos de dados, filtrar linhas.
- [ ] Adicionar colunas: Coluna Condicional e Coluna Personalizada (básico).
- [ ] Combinar dados: Mesclar consultas (Merge - análogo aos Joins) e Anexar consultas (Append - análogo ao Union).
- [ ] Boas práticas: Organizando as etapas aplicadas.

### 3. Modelagem de Dados (Visão Modelo)
- [ ] O que é um modelo de dados?
- [ ] Criando e gerenciando relacionamentos entre tabelas (cardinalidade e direção do filtro).
- [ ] O conceito de Tabela Fato vs. Tabela Dimensão (Modelo Star Schema).
- [ ] Criando uma Tabela Calendário básica.

### 4. Cálculos com DAX (Data Analysis Expressions)
- [ ] Diferença: Colunas Calculadas vs. Medidas.
- [ ] Criando suas primeiras Medidas: `SUM`, `AVERAGE`, `COUNT`, `DISTINCTCOUNT`.
- [ ] A função mais importante: `CALCULATE()`.
- [ ] Funções de Tabela Simples: `FILTER`, `ALL`.

### 5. Visualização de Dados (Visão Relatório)
- [ ] Adicionando e formatando visuais: Gráficos de Barra, Linha, Pizza e Cartões.
- [ ] Usando Matrizes e Tabelas.
- [ ] Filtros e Segmentação de Dados (Slicers).
- [ ] Configurando interações entre visuais.
- [ ] Boas práticas de design: Cores, alinhamento e simplicidade.

### 6. Publicação e Compartilhamento (Power BI Service)
- [ ] Publicando um relatório do Desktop para o Service.
- [ ] O que são Workspaces.
- [ ] Criando e compartilhando um Dashboard simples.
- [ ] Atualização de dados: Configurando o Gateway de dados para atualização agendada.

---

## ✈️ Nível Pleno: Dashboards Relevantes para o Negócio
*Aqui você vai além do básico, criando modelos de dados robustos, cálculos DAX complexos e relatórios que contam uma história.*

### 1. Power Query Avançado
- [ ] Parâmetros: Tornando suas queries dinâmicas.
- [ ] Funções personalizadas em Linguagem M.
- [ ] Técnicas de performance: Desabilitar carga, otimizar etapas.
- [ ] Tratamento de erros e dados "sujos".

### 2. DAX Intermediário e Avançado
- [ ] **Contexto de Avaliação:** O conceito mais crucial em DAX (Contexto de Linha vs. Contexto de Filtro).
- [ ] Funções Iteradoras (sufixo X): `SUMX`, `AVERAGEX`, `RANKX`.
- [ ] **Inteligência de Tempo:** `DATESYTD`, `SAMEPERIODLASTYEAR`, `DATEADD`.
- [ ] Funções de Tabela Avançadas: `VALUES`, `SUMMARIZE`, `CROSSJOIN`.
- [ ] Variáveis em DAX (`VAR` ... `RETURN`) para organizar e otimizar cálculos.

### 3. Modelagem de Dados Avançada
- [ ] Relacionamentos complexos: Muitos-para-muitos (com tabela ponte).
- [ ] Otimizando o modelo: Cardinalidade, direção do filtro e o impacto na performance.
- [ ] Segurança em nível de linha (Row-Level Security - RLS).
- [ ] Hierarquias e Grupos.

### 4. Visualização e Storytelling
- [ ] Bookmarks (Marcadores) para criar navegação e contar histórias.
- [ ] Tooltips (Dicas de Ferramenta) personalizados.
- [ ] Drill-through para navegar entre páginas de relatório.
- [ ] Uso de visuais personalizados da AppSource.
- [ ] Parâmetros "What-if" para simulações.

---

## 🛰️ Nível Sênior/Especialista: Performance, Governança e Arquitetura
*O foco muda para a otimização de grandes volumes de dados, governança, reusabilidade e a integração do Power BI na arquitetura de dados da empresa.*

### 1. Otimização de Performance (Performance Tuning)
- [ ] **DAX Studio e Tabular Editor:** Ferramentas externas para analisar e otimizar seu modelo.
- [ ] Analisando o desempenho de queries com o Performance Analyzer.
- [ ] Otimização do modelo de dados (VertiPaq Analyzer): Reduzindo cardinalidade e tamanho do arquivo.
- [ ] Modos de armazenamento: Import vs. DirectQuery vs. Composite. Quando usar cada um.

### 2. Arquitetura e Governança no Power BI Service
- [ ] **Fluxos de Dados (Dataflows):** Reutilizando lógicas de ETL do Power Query para múltiplos relatórios.
- [ ] **Conjuntos de Dados Compartilhados (Shared Datasets):** Criando uma "única fonte da verdade".
- [ ] Pipelines de Implantação (Dev/Test/Prod).
- [ ] Endpoints XMLA para gerenciamento avançado.
- [ ] Certificação e promoção de conteúdo.

### 3. Integração e Tópicos Avançados
- [ ] Power BI com fontes de dados na nuvem (Azure Synapse, Databricks, Snowflake).
- [ ] Incorporando relatórios do Power BI em outras aplicações (Power BI Embedded).
- [ ] Paginated Reports para relatórios com formato de impressão.
- [ ] Metas e Scorecards no Power BI.
- [ ] Noções de licenciamento: Pro vs. Premium por Usuário vs. Premium por Capacidade.
