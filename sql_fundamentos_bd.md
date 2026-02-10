# Fundamentos do Banco de Dados Relacional

[Voltar para o Roadmap de SQL](sql.md)

---

Bem-vindo ao ponto de partida! Antes de escrever nossa primeira linha de SQL, precisamos entender onde estamos pisando. Um banco de dados relacional é como um armário de arquivamento digital, perfeitamente organizado.

## O que é um Banco de Dados Relacional?

Imagine uma biblioteca. Os livros não ficam jogados em uma pilha gigante. Eles são organizados por gênero (Ficção, História, Ciência), depois por autor e título. Essa organização permite que você encontre qualquer livro de forma rápida e eficiente.

Um **banco de dados relacional** faz a mesma coisa com informações. Ele organiza os dados em tabelas que se "relacionam" (se conectam) umas com as outras. A "linguagem" que usamos para conversar com esse banco, pedir informações ou guardar coisas novas, é o **SQL**.

## Os Blocos de Construção

Todo banco de dados relacional é feito de três componentes básicos:

### 1. Tabelas (Tables)
A tabela é o principal componente. Pense nela como uma planilha do Excel. Cada tabela armazena dados sobre um assunto específico. Por exemplo, em um sistema de uma loja, teríamos uma tabela de `CLIENTES`, uma de `PRODUTOS` e outra de `PEDIDOS`.

### 2. Colunas (Columns / Campos)
As colunas são as "categorias" de informação dentro de uma tabela. Na nossa tabela de `CLIENTES`, as colunas seriam `ID_Cliente`, `Nome`, `Email`, `Data_de_Nascimento`, etc. Cada coluna tem um nome e um tipo de dado específico.

### 3. Linhas (Rows / Registros)
As linhas são os registros individuais de dados. Cada linha na tabela `CLIENTES` representa um cliente único, com as informações preenchidas em cada uma das colunas.

**Exemplo Visual (Tabela `CLIENTES`):**

| ID_Cliente (INT) | Nome (VARCHAR) | Email (VARCHAR) |
| :--- | :--- | :--- |
| 1 | João Silva | joao.s@email.com |
| 2 | Maria Santos | maria.s@email.com |

## As Chaves: A Cola que Une as Tabelas

As chaves são colunas especiais que criam as "relações" entre as tabelas.

- **Chave Primária (Primary Key - PK):** É o identificador **único e obrigatório** de cada linha em uma tabela. Na tabela `CLIENTES`, a coluna `ID_Cliente` é a Chave Primária. Não podem existir dois clientes com o mesmo ID.

- **Chave Estrangeira (Foreign Key - FK):** É uma coluna em uma tabela que se refere à Chave Primária de outra tabela. É assim que criamos a conexão. Por exemplo, na tabela `PEDIDOS`, teríamos uma coluna `ID_do_Cliente` que seria uma Chave Estrangeira apontando para a coluna `ID_Cliente` da tabela `CLIENTES`. Isso nos permite saber qual cliente fez qual pedido.

## Tipos de Dados Essenciais

Cada coluna precisa ter um tipo de dado definido. Isso garante a integridade e a eficiência do banco. Os mais comuns são:

- **`INT` ou `INTEGER`:** Para números inteiros (ex: 1, 45, 1000).
- **`VARCHAR(n)`:** Para textos de tamanho variável, onde `n` é o número máximo de caracteres (ex: `VARCHAR(100)` para um nome).
- **`TEXT`:** Para textos longos, sem um limite fixo.
- **`DATE`:** Para armazenar datas (ex: '2026-02-10').
- **`TIMESTAMP` ou `DATETIME`:** Para armazenar data e hora juntas.
- **`DECIMAL(p, s)`:** Para números com casas decimais, ideais para valores monetários (ex: `DECIMAL(10, 2)` para R$ 99.99). `p` é o total de dígitos e `s` é o número de dígitos após a vírgula.
- **`BOOLEAN`:** Para valores de verdadeiro/falso (`true`/`false` ou `1`/`0`).

---

Com esses conceitos em mente, você está pronto para começar a fazer consultas!

[Próximo Tópico: Consultas e Filtros](link_para_proxima_pagina.md) *(Este link ainda não funciona)*
