---
layout: default
title: SQL
nav_order: 2
has_children: true
permalink: /sql
---

# Roadmap de Estudos: SQL - Do Zero à Referência Técnica

Bem-vindo ao guia completo de SQL. Este roadmap foi desenhado para levar qualquer pessoa do zero absoluto a um nível de proficiência capaz de resolver problemas complexos de dados, otimizar performance e entender a arquitetura por trás de grandes sistemas.

Cada título principal é um link para uma página dedicada com teoria, exemplos de código e exercícios.

---

## 🚀 Nível Júnior: A Base Obrigatória
*O objetivo aqui é ganhar fluência na extração e manipulação de dados. Se não dominar isso, não sai do lugar.*

### 1. Fundamentos do Banco de Dados Relacional
- O que é um banco de dados relacional vs. NoSQL?
- Conceitos: Tabelas, Linhas (Registros), Colunas (Campos).
- Chaves: Chave Primária (PK), Chave Estrangeira (FK), Chave Única (Unique Key).
- Tipos de Dados Essenciais: `INT`, `VARCHAR`, `TEXT`, `DATE`, `TIMESTAMP`, `DECIMAL`, `FLOAT`, `BOOLEAN`.

### 2. Consultas e Filtros (A Linguagem Essencial)
- Comandos Essenciais: `SELECT`, `FROM`, `WHERE`.
- Ordenação e Limitação: `ORDER BY (ASC/DESC)`, `LIMIT` (ou `TOP` / `FETCH FIRST`).
- Valores Únicos: `DISTINCT`.
- Apelidos (Aliases): `AS` para colunas e tabelas.

### 3. Operadores para Filtros Precisos
- Comparação: `=`, `<`, `>`, `<=`, `>=`, `<>` (ou `!=`).
- Lógicos: `AND`, `OR`, `NOT`.
- Padrões de Texto: `LIKE` (com os wildcards `%` e `_`).
- Intervalos e Listas: `BETWEEN`, `IN`.
- Tratamento de Nulos: `IS NULL`, `IS NOT NULL`.

### 4. Funções de Agregação (Resumindo Dados)
- Funções Essenciais: `COUNT()`, `SUM()`, `AVG()`, `MIN()`, `MAX()`.
- Agrupamento de Dados: `GROUP BY`.
- Filtro Pós-Agrupamento: `HAVING` (e a diferença crucial para o `WHERE`).

### 5. Manipulação de Dados (CRUD)
- **C**reate: `INSERT INTO ... VALUES`.
- **R**ead: `SELECT` (já vimos!).
- **U**pdate: `UPDATE ... SET ... WHERE`.
- **D**elete: `DELETE FROM ... WHERE`.

### 6. Junção de Tabelas
- `INNER JOIN`: O cruzamento fundamental.
- Entendendo a cláusula `ON`.

### 🎓 Projeto Prático Nível Júnior:
- **Análise de Vendas de uma Livraria:** Dado um conjunto de tabelas (Livros, Autores, Vendas), responder perguntas como: "Quais os 5 livros mais vendidos?", "Qual o total de receita por autor?", "Quantos clientes únicos fizeram compras no último mês?".

---

## ✈️ Nível Pleno: Entregando Resultados de Negócio
*Aqui você se torna realmente útil, respondendo perguntas complexas, organizando queries e garantindo a qualidade dos dados.*

### 1. Joins Avançados e Combinação de Dados
- `LEFT JOIN` e `RIGHT JOIN`: Encontrando dados que não se correspondem.
- `FULL OUTER JOIN`: Vendo o universo completo de duas tabelas.
- `CROSS JOIN`: O produto cartesiano (e quando ter cuidado com ele).
- `UNION` vs. `UNION ALL`: Combinando resultados de múltiplas queries.

### 2. Organizando Queries Complexas
- **Subqueries (Subconsultas):** No `SELECT`, `WHERE`, `FROM` e a diferença entre subqueries escalares, multi-linha e correlacionadas.
- **CTE (Common Table Expressions):** A cláusula `WITH` para legibilidade e modularidade. Por que são (quase) sempre melhores que subqueries complexas.
- `EXISTS` e `NOT EXISTS`: Alternativas performáticas ao `IN` e `NOT IN`.

### 3. Funções de Transformação e Limpeza
- **Lógica Condicional:** `CASE WHEN ... THEN ... END`.
- **Tratamento de Nulos Avançado:** `COALESCE`, `NULLIF`.
- **Funções de Texto:** `CONCAT`, `SUBSTRING`, `REPLACE`, `TRIM`, `UPPER`, `LOWER`, `LENGTH`.
- **Funções de Data:** `DATE_TRUNC`, `DATE_PART` (ou `EXTRACT`), `DATEADD`, `DATEDIFF`, `NOW()`.
- **Conversão de Tipos:** `CAST` e `CONVERT`.

### 4. Estrutura e Performance Inicial
- **Views:** Criando "tabelas virtuais" para simplificar o acesso e a segurança.
- **Índices:** O que são, como funcionam (conceito de B-Tree) e o impacto de um `SELECT` vs. `INSERT/UPDATE`.
- **Controle de Transações:** `BEGIN TRANSACTION`, `COMMIT`, `ROLLBACK`. A importância da atomicidade (ACID).

### 🎓 Projeto Prático Nível Pleno:
- **Análise de Churn de uma Plataforma de Streaming:** Usando Joins, CTEs e funções de data, identificar padrões em clientes que cancelaram a assinatura. "Clientes que cancelam assistem menos horas?", "Qual o tempo médio de vida de um assinante?".

---

## 🛰️ Nível Sênior: Resolvendo Problemas em Escala
*O foco muda para performance, governança e queries que resolvem problemas sistêmicos, não apenas perguntas pontuais.*

### 1. Window Functions (Funções de Janela)
- **Ranking e Numeração:** `ROW_NUMBER()`, `RANK()`, `DENSE_RANK()`, `NTILE()`.
- **Navegação entre Linhas:** `LAG()` (olhar para trás), `LEAD()` (olhar para frente).
- **Agregações em Janela:** `SUM() OVER (...)`, `AVG() OVER (...)` para criar médias móveis e totais acumulados.
- **Sintaxe Completa:** `OVER (PARTITION BY ... ORDER BY ... ROWS BETWEEN ...)`

### 2. Otimização de Performance (Query Tuning)
- **Planos de Execução:** Lendo e interpretando o `EXPLAIN PLAN` (ou similar) para identificar gargalos.
- **Índices Avançados:** Índices compostos, cobertos (covering indexes), e o que é "index seek" vs. "index scan".
- **SARGable Queries:** Escrevendo cláusulas `WHERE` que podem usar índices de forma eficiente.
- **Materialized Views:** Quando e por que pré-calcular resultados.

### 3. Modelagem e Arquitetura de Dados
- **Normalização:** 1ª, 2ª e 3ª Formas Normais (1FN, 2FN, 3FN).
- **Desnormalização:** Quando quebrar as regras de normalização em prol da performance.
- **Modelagem Dimensional (BI):** Tabelas Fato e Dimensão, Star Schema vs. Snowflake Schema.
- **Slowly Changing Dimensions (SCD):** Tipos 1, 2 e 3 para rastrear histórico.

### 4. SQL Programático e Governança
- **Stored Procedures:** Criando lógicas reutilizáveis no banco.
- **User-Defined Functions (UDFs):** Funções personalizadas.
- **Triggers:** O que são, seus perigos e casos de uso legítimos.
- **Segurança:** Gerenciamento de `Usuários`, `Roles` e `Permissões` (`GRANT`, `REVOKE`).

### 🎓 Projeto Prático Nível Sênior:
- **Otimização de Dashboard de BI:** Pegar um conjunto de queries lentas de um dashboard, analisar os planos de execução, propor e aplicar otimizações (índices, refatoração com Window Functions) e medir o ganho de performance.

---

## 🌌 Nível Especialista: A Visão do Ecossistema
*O foco transcende o SQL puro e abrange sua aplicação no mundo real de Cloud, Big Data e Engenharia de Dados.*

### 1. Arquitetura e Grandes Volumes (Big Data)
- **Estratégias de Escala:** Particionamento de tabelas, Sharding (conceito).
- **Carga de Dados em Lote (ETL/ELT):** `BULK INSERT`, `COPY INTO`, `MERGE` (Upsert).
- **SQL em Data Lakes:** Conceitos de `Hive`, `Presto`, `Trino`.

### 2. SQL no Ecossistema Cloud & Analytics
- **Diferenças e Dialetos:** As particularidades do `PostgreSQL`, `MySQL`, `SQL Server`, `Oracle`.
- **SQL em Data Warehouses na Nuvem:** Uma visão sobre `Google BigQuery`, `Amazon Redshift`, `Snowflake`, `Azure Synapse`.
- **SQL para Ferramentas de BI:** Como o SQL se conecta e otimiza o `Power BI` (DirectQuery), `Tableau`, `Looker` (LookML).

### 3. Tópicos Avançados e Governança
- **SQL para Análise Estatística:** Funções de correlação, regressão e distribuição.
- **SQL para Dados Geoespaciais:** Tipos de dados como `GEOGRAPHY` e funções como `ST_Distance`.
- **Governança e Qualidade:** Usando SQL para criar testes de qualidade de dados (ex: dbt tests).
- **Controle de Concorrência:** Locks, Deadlocks e Níveis de Isolamento de Transação.
