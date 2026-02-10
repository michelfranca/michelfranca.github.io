# Roadmap de Estudos: SQL - Do Zero à Referência Técnica

[Voltar para a Página Inicial](index.md)

---

Este é um guia de estudos completo para SQL, inspirado nas necessidades do mercado e dividido por níveis de senioridade. O objetivo é construir uma base sólida e evoluir para tópicos que resolvem problemas complexos de negócio, performance e arquitetura.

---

## 🚀 Nível Júnior: A Base Obrigatória
*Se não dominar isso, não sai do lugar. O foco é extrair informações do banco de dados com segurança e precisão.*

### 1. Fundamentos do Banco de Dados Relacional
- O que é um banco de dados relacional?
- Conceitos de Tabelas, Linhas (Registros) e Colunas (Campos)
- Chaves: Chave Primária (PK) e Chave Estrangeira (FK)
- Tipos de Dados Essenciais: `INT`, `VARCHAR`, `TEXT`, `DATE`, `TIMESTAMP`, `DECIMAL`, `BOOLEAN`

### 2. Consultas e Filtros (O pão com manteiga do SQL)
- **Comandos Essenciais:** `SELECT`, `FROM`, `WHERE`
- **Ordenação e Limitação:** `ORDER BY (ASC/DESC)`, `LIMIT` (ou `TOP` em SQL Server)
- **Valores Únicos:** `DISTINCT`
- **Apelidos (Aliases):** `AS` para colunas e tabelas

### 3. Operadores para Filtros Precisos
- **Comparação:** `=`, `<`, `>`, `<=`, `>=`, `<>` (ou `!=`)
- **Lógicos:** `AND`, `OR`, `NOT`
- **Padrões de Texto:** `LIKE` (com `%` e `_`)
- **Intervalos e Listas:** `BETWEEN`, `IN`
- **Valores Nulos:** `IS NULL`, `IS NOT NULL`

### 4. Funções de Agregação (Resumindo dados)
- `COUNT()` - Contar linhas
- `SUM()` - Somar valores
- `AVG()` - Calcular a média
- `MIN()` / `MAX()` - Encontrar o menor/maior valor
- **Agrupamento:** `GROUP BY`
- **Filtro Pós-Agrupamento:** `HAVING`

### 5. Manipulação de Dados (CRUD)
- **Criar:** `INSERT INTO`
- **Ler:** `SELECT` (já vimos!)
- **Atualizar:** `UPDATE`
- **Deletar:** `DELETE`

### 6. Junção de Tabelas
- `INNER JOIN` - O "cruzamento" mais comum

---

## ✈️ Nível Pleno: Entregando Resultados de Negócio
*Aqui você começa a ser realmente útil, respondendo perguntas de negócio complexas e organizando suas queries.*

### 1. Joins Avançados
- `LEFT JOIN` (Muito comum para encontrar o que "não cruzou")
- `RIGHT JOIN`
- `FULL OUTER JOIN`

### 2. Organizando Queries Complexas
- **Subqueries (Subconsultas):** Usando um `SELECT` dentro de `SELECT`, `WHERE` ou `FROM`
- **CTE (Common Table Expressions):** A cláusula `WITH` para deixar suas queries legíveis e modulares. (Preferível a subqueries complexas!)
- **Combinando Resultados:** `UNION` e `UNION ALL`

### 3. Funções de Transformação de Dados
- **Lógica Condicional:** `CASE WHEN ... THEN ... END`
- **Funções de Texto:** `CONCAT`, `SUBSTRING`, `REPLACE`, `TRIM`, `UPPER`, `LOWER`
- **Funções de Data:** `DATEADD`, `DATEDIFF`, `EXTRACT`, `YEAR`, `MONTH`, `DAY`, `NOW()`
- **Conversão de Tipos:** `CAST`, `CONVERT`

### 4. Tópicos Intermediários
- **Views:** Criando "tabelas virtuais" para simplificar o acesso.
- **Índices:** O que são e por que aceleram (e às vezes atrasam) as coisas.
- **Conceitos de Normalização:** Entender a ideia por trás da 1ª, 2ª e 3ª Forma Normal (1FN, 2FN, 3FN).
- **Controle de Transações:** `BEGIN TRANSACTION`, `COMMIT`, `ROLLBACK`

---

## 🛰️ Nível Sênior: Resolvendo Problemas em Escala
*Aqui você passa a pensar em performance, governança e em resolver problemas que afetam o sistema como um todo.*

### 1. Window Functions (Funções de Janela)
- **Ranking:** `ROW_NUMBER()`, `RANK()`, `DENSE_RANK()`
- **Navegação:** `LAG()` (olhar para a linha anterior), `LEAD()` (olhar para a próxima)
- **Sintaxe:** `OVER (PARTITION BY ..., ORDER BY ...)`

### 2. Otimização de Performance (Query Tuning)
- **Planos de Execução:** Entendendo o `EXPLAIN` (ou `QUERY PLAN`) para ver como o banco "pensa".
- **Índices Avançados:** Índices compostos, clustered vs. non-clustered.
- **Boas Práticas:** Evitar `SELECT *`, usar filtros eficientes (SARGable queries).

### 3. Modelagem e Arquitetura
- **Modelagem Dimensional (BI):** Tabelas Fato e Dimensão, Star Schema.
- **Procedures e Funções:** `Stored Procedures` e `User-Defined Functions (UDFs)`.
- **Triggers:** O que são, quando usar e (principalmente) quando não usar.
- **Segurança:** Gerenciamento de `Usuários`, `Roles` e `Permissões` (`GRANT`, `REVOKE`).

---

## 🌌 Nível Especialista: A Visão do Ecossistema
*O foco sai do SQL puro e entra na sua aplicação no mundo real de Cloud, Big Data e Analytics.*

### 1. Arquitetura e Grandes Volumes
- **Estratégias de Escala:** Particionamento de tabelas, Sharding (conceito).
- **Disponibilidade:** Replicação, Alta Disponibilidade (HA).
- **Carga de Dados em Lote:** `BULK INSERT`, `MERGE` (Upsert).

### 2. SQL no Ecossistema Cloud & Analytics
- **Diferenças entre Engines:** As particularidades do `PostgreSQL`, `MySQL`, `SQL Server`, `Oracle`.
- **SQL em Data Warehouses na Nuvem:** Uma visão sobre `Google BigQuery`, `Amazon Redshift`, `Snowflake`.
- **SQL para Ferramentas de BI:** Como o SQL se conecta e otimiza o `Power BI`, `Tableau`, `Looker`.
- **Governança e Qualidade:** Usando SQL para garantir a qualidade dos dados (Data Quality).

