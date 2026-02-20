---
layout: default
title: Power BI
nav_order: 3
has_children: false
permalink: /powerbi
---

# Roadmap de Estudos para a Certificação Microsoft Power BI (PL-300)

Este é um guia de estudos completo e detalhado, focado nos tópicos essenciais para a aprovação na prova de certificação de Power BI da Microsoft. O conteúdo abrange desde a preparação de dados até a governança, com ênfase nos conceitos que mais reprovam candidatos.

---

## 1️⃣ Preparar os Dados (Power Query – ETL)

### 🔹 Conexão de Dados
- [ ] Excel, CSV, TXT
- [ ] Banco relacional (SQL Server, MySQL etc.)
- [ ] SharePoint
- [ ] Web
- [ ] Pastas
- [ ] Dataflows
- [ ] Entender a diferença: DirectQuery vs. Import vs. Live Connection
- [ ] Criar e usar Parâmetros

### 🔹 Transformações (Power Query M)
- [ ] Remover / renomear colunas
- [ ] Alterar tipo de dados
- [ ] Mesclar consultas (Merge)
- [ ] Acrescentar consultas (Append)
- [ ] Criar Colunas personalizadas
- [ ] Criar Colunas condicionais
- [ ] Criar Colunas por exemplo
- [ ] Agrupar dados (Group By)
- [ ] Pivot (Dinamizar Colunas) / Unpivot (Transformar Colunas em Linhas)
- [ ] Transpor
- [ ] Dividir colunas
- [ ] Extrair texto (Primeiros/Últimos/Intervalo de Caracteres)
- [ ] Tratamento de erros
- [ ] Detectar e remover duplicados
- [ ] Criar coluna de índice
- [ ] Criar tabela calendário via Linguagem M
- [ ] Entender o conceito de Query Folding e seu impacto na performance
- [ ] Boas práticas de performance no Power Query

---

## 2️⃣ Modelar os Dados (Coração da Prova)

### 🔹 Conceitos Obrigatórios
- [ ] Modelo estrela (Star Schema)
- [ ] Tabela fato vs. Tabela dimensão
- [ ] Cardinalidade (1:1, 1:N, N:N)
- [ ] Direção do filtro (Single vs. Both)
- [ ] Relacionamento ativo vs. inativo
- [ ] Usar a função `USERELATIONSHIP` em cálculos DAX
- [ ] Entender o conceito de Snowflake schema
- [ ] Criar e marcar uma Tabela de Datas corretamente
- [ ] Conceitos de Normalização vs. Desnormalização

### 🔹 Boas Práticas e Otimização
- [ ] Evitar relacionamentos bidirecionais desnecessários
- [ ] Criar dimensões auxiliares (e.g., para medidas)
- [ ] Otimizar o desempenho do modelo
- [ ] Estratégias para redução de cardinalidade
- [ ] Entender quando usar Colunas Calculadas vs. Medidas
- [ ] Otimização geral do modelo para performance

---

## 3️⃣ DAX (A Parte que Mais Reprova)

### 🔹 Conceitos Base (Obrigatório Dominar)
- [ ] Contexto de linha
- [ ] Contexto de filtro
- [ ] Transição de contexto (Context transition)
- [ ] **CALCULATE:** Entender profundamente seu funcionamento
- [ ] Funções de modificação de contexto: `ALL`, `ALLEXCEPT`, `REMOVEFILTERS`
- [ ] Funções de tabela: `VALUES`, `DISTINCT`
- [ ] Funções de relacionamento: `RELATED`, `RELATEDTABLE`

### 🔹 Funções Essenciais por Categoria
- [ ] **Funções de Agregação e Iteradoras:** `SUM`, `AVERAGE`, `COUNT`, `COUNTROWS`, `DISTINCTCOUNT`, e suas versões com `X` (`SUMX`, `AVERAGEX`).
- [ ] **Funções Lógicas:** `IF`, `SWITCH`, `AND` / `OR`, `ISBLANK`, `COALESCE`.
- [ ] **Função de Divisão Segura:** `DIVIDE`.
- [ ] **Inteligência de Tempo (Muito Cobrado):** `TOTALYTD`, `TOTALMTD`, `TOTALQTD`, `SAMEPERIODLASTYEAR`, `DATEADD`, `DATESYTD`, `DATESMTD`, `DATESBETWEEN`, `PARALLELPERIOD`.
- [ ] **Funções de Ranking e Análise:** `RANKX`, `TOPN`.
- [ ] **Funções de Tabela para Cálculos:** `FILTER`, `ADDCOLUMNS`, `SUMMARIZE`, `SUMMARIZECOLUMNS`, `GENERATE`, `CROSSJOIN`.
- [ ] **Função `EARLIER`:** Entender o conceito, mesmo sendo menos usada hoje.

---

## 4️⃣ Criar Relatórios (Visualização)

### 🔹 Visuais e Interações
- [ ] Gráfico de colunas, barras, linha, área e combinado
- [ ] Tabela e matriz
- [ ] Cartão e KPI
- [ ] Segmentação de Dados (Slicer)
- [ ] Configurar Drill-through e Drill-down
- [ ] Criar Tooltip (Dica de Ferramenta) personalizado
- [ ] Editar interações entre visuais
- [ ] Sincronizar slicers entre páginas
- [ ] Usar Botões, Bookmarks e Navegação para criar uma experiência de App

### 🔹 UX e Layout
- [ ] Criar Layout responsivo para web e mobile
- [ ] Aplicar um Tema personalizado
- [ ] Manter cores e fontes consistentes
- [ ] Considerar boas práticas de Acessibilidade

---

## 5️⃣ Performance e Otimização
- [ ] Usar o Performance Analyzer para identificar gargalos
- [ ] Otimizar fórmulas DAX
- [ ] Reduzir a cardinalidade do modelo
- [ ] Evitar colunas desnecessárias
- [ ] Entender o impacto de Medidas vs. Colunas Calculadas
- [ ] Conhecer as limitações de performance do DirectQuery

---

## 6️⃣ Segurança
- [ ] **RLS (Row-Level Security):**
    - [ ] Criar funções (roles) estáticas e dinâmicas
    - [ ] Usar a função `USERPRINCIPALNAME()` para segurança dinâmica
    - [ ] Testar as regras de segurança como um usuário

---

## 7️⃣ Power BI Service (Online)
- [ ] Publicar um relatório
- [ ] Criar e publicar um App
- [ ] Gerenciar Workspaces
- [ ] Configurar a atualização agendada
- [ ] Entender e configurar o Gateway (On-premises)
- [ ] Criar e consumir Dataflows
- [ ] Gerenciar compartilhamento e permissões
- [ ] Usar Certificação e Promoção (Endorsement) de datasets

---

## 8️⃣ Governança e Administração
- [ ] Usar a visão de linhagem de dados (Lineage view)
- [ ] Fazer análise de impacto de alterações
- [ ] Configurar Pipelines de Implantação (Deployment Pipelines)
- [ ] Estratégias de versionamento de arquivos PBIX
- [ ] Aplicar rótulos de sensibilidade (Sensitivity labels)
- [ ] Classificação de dados (Data classification)

---

## 🔥 Nível de Exigência Real
- [ ] **Modelagem:** Ser capaz de criar um modelo estrela do zero.
- [ ] **DAX:** Escrever medidas de YTD, crescimento % e ranking sem copiar.
- [ ] **Segurança:** Implementar RLS dinâmico.
- [ ] **Publicação:** Publicar e configurar um gateway de dados.
- [ ] **Conceitual:** Ser capaz de explicar contexto de filtro sem travar.
