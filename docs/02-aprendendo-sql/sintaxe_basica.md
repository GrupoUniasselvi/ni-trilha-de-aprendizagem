# Aprenda sobre as sintaxes

Nesta seção, você vai aprender algumas das principais sintaxes em SQL, desde consultas simples até técnicas mais avançadas.

## Editar instruções SQL para ajustar os resultados da consulta

Editar consultas SQL é fundamental para personalizar os resultados. Você pode aprender mais sobre isso com o guia oficial da Microsoft:

[Editar Instruções SQL](https://support.microsoft.com/pt-br/topic/editar-instru%C3%A7%C3%B5es-sql-para-ajustar-os-resultados-da-consulta-5e10932d-20fc-4a66-bf40-b3f8b207e4a8)

---

## T-SQL - SELECT FROM - Consultas simples a uma Tabela - SQL Server

O comando `SELECT` é usado para buscar dados de uma tabela. Você pode selecionar colunas específicas ou todas as colunas usando `*`.

**Exemplo de código:**

```sql
-- Seleciona todas as colunas da tabela 'clientes'
SELECT * FROM clientes;

-- Seleciona apenas as colunas 'nome' e 'cidade' da tabela 'clientes'
SELECT nome, cidade FROM clientes;
```

Assista ao vídeo para entender melhor como funciona:

<iframe width="560" height="315" src="https://www.youtube.com/embed/0xO1rVj6oHA?si=iYKtQoN7__ADbsBl" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---

## T-SQL - Alias com AS - Nomes alternativos para colunas - SQL

O alias permite que você atribua nomes alternativos a colunas ou tabelas para facilitar a leitura e o entendimento da consulta.

**Exemplo de código:**

```sql
-- Renomeia a coluna 'nome' para 'Cliente' e 'cidade' para 'Cidade'
SELECT nome AS Cliente, cidade AS Cidade
FROM clientes;
```

Veja o vídeo para mais detalhes sobre alias:

<iframe width="560" height="315" src="https://www.youtube.com/embed/RbVvrcK5yJo?si=gVQdZrKkVSnZ0quL" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---

## T-SQL - DISTINCT - Consultas com valores distintos, sem repetição

O comando `DISTINCT` remove valores duplicados dos resultados da consulta.

**Exemplo de código:**

```sql
-- Seleciona todas as cidades únicas da tabela 'clientes'
SELECT DISTINCT cidade FROM clientes;
```

Assista ao vídeo para aprender mais sobre o uso de `DISTINCT`:

<iframe width="560" height="315" src="https://www.youtube.com/embed/scCo_1F6_Pg?si=-ak8GXPpcZc5OhUF" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---

## T-SQL - ORDER BY - Consultas com ordenação de Colunas - SQL Server

A cláusula `ORDER BY` é usada para ordenar os resultados da consulta por uma ou mais colunas.

**Exemplo de código:**

```sql
-- Ordena os clientes pela coluna 'cidade' em ordem alfabética
SELECT nome, cidade
FROM clientes
ORDER BY cidade;

-- Ordena os clientes pela coluna 'nome' em ordem decrescente
SELECT nome, cidade
FROM clientes
ORDER BY nome DESC;
```

Entenda melhor a cláusula `ORDER BY` com o vídeo abaixo:

<iframe width="560" height="315" src="https://www.youtube.com/embed/HNZxBgHW_VY?si=LUoS8Gvcri9_X2TE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---

## T-SQL - TOP - Especificar número de registros a retornar - SQL Server

O comando `TOP` limita o número de registros retornados pela consulta.

**Exemplo de código:**

```sql
-- Seleciona os 5 primeiros clientes da tabela 'clientes'
SELECT TOP 5 nome, cidade FROM clientes;

-- Seleciona os 10 primeiros clientes ordenados por cidade
SELECT TOP 10 nome, cidade
FROM clientes
ORDER BY cidade;
```

Confira o vídeo sobre o comando `TOP`:

<iframe width="560" height="315" src="https://www.youtube.com/embed/YaCfy6PvzAE?si=FoWiT3N8IDtp6c6D" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Próximos Passos

Parabéns pelo progresso! Agora que você conhece as principais sintaxes SQL, vamos seguir para o próximo conteúdo e continuar avançando em nosso aprendizado.
