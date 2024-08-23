# Conheça sobre Filtros e Seleção de Intervalos

## T-SQL - BETWEEN - Seleção de Intervalos em Registros - SQL Server

O operador `BETWEEN` é utilizado para selecionar valores dentro de um intervalo definido, incluindo os valores de limite.

**Exemplo de código:**

```sql
-- Seleciona todos os clientes cuja idade está entre 20 e 30 anos
SELECT nome, idade
FROM clientes
WHERE idade BETWEEN 20 AND 30;
```

Assista ao vídeo para uma explicação mais detalhada:

<iframe width="560" height="315" src="https://www.youtube.com/embed/FNFkqa9nvpY?si=UxRnCU9X--GsD46G" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---

## T-SQL - AND e OR - Operadores Lógicos - SQL Server

Os operadores lógicos `AND` e `OR` são usados para combinar múltiplas condições em uma consulta SQL. O `AND` retorna resultados onde todas as condições são verdadeiras, enquanto o `OR` retorna resultados se ao menos uma condição for verdadeira.

**Exemplo de código:**

```sql
-- Seleciona clientes que vivem em 'São Paulo' e têm idade maior que 25 anos
SELECT nome, cidade, idade
FROM clientes
WHERE cidade = 'São Paulo' AND idade > 25;

-- Seleciona clientes que vivem em 'São Paulo' ou têm idade maior que 25 anos
SELECT nome, cidade, idade
FROM clientes
WHERE cidade = 'São Paulo' OR idade > 25;
```

Confira o vídeo para entender melhor o uso de operadores lógicos:

<iframe width="560" height="315" src="https://www.youtube.com/embed/LFAn9e1qC8Q?si=0gHck1tVFziuigrb" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---

## T-SQL - WHERE - Filtrando registros em uma consulta - SQL Server

A cláusula `WHERE` é usada para filtrar registros que atendem a uma condição específica.

**Exemplo de código:**

```sql
-- Seleciona clientes que moram na cidade de 'Rio de Janeiro'
SELECT nome, cidade
FROM clientes
WHERE cidade = 'Rio de Janeiro';
```

Assista ao vídeo para aprender a usar a cláusula `WHERE`:

<iframe width="560" height="315" src="https://www.youtube.com/embed/IpYkzSgAykI?si=1mxINI4o88tL6p5T" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---

## T-SQL - LIKE e NOT LIKE - Filtrar por padrões específicos - SQL Server

O operador `LIKE` é usado para buscar um padrão específico em uma coluna, enquanto o `NOT LIKE` filtra os registros que não correspondem ao padrão.

**Exemplo de código:**

```sql
-- Seleciona clientes cujo nome começa com 'A'
SELECT nome
FROM clientes
WHERE nome LIKE 'A%';

-- Seleciona clientes cujo nome não termina com 'o'
SELECT nome
FROM clientes
WHERE nome NOT LIKE '%o';
```

Veja o vídeo para aprender mais sobre `LIKE` e `NOT LIKE`:

<iframe width="560" height="315" src="https://www.youtube.com/embed/ukrQ6GSxfc4?si=dy2erYxXEzHWkDq4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---

## T-SQL - Operadores IN e NOT IN - Filtros de Múltiplas Condições - SQL Server

O operador `IN` é usado para especificar múltiplos valores em uma condição `WHERE`, e `NOT IN` faz o oposto, filtrando valores fora da lista especificada.

**Exemplo de código:**

```sql
-- Seleciona clientes que vivem em 'São Paulo', 'Rio de Janeiro' ou 'Belo Horizonte'
SELECT nome, cidade
FROM clientes
WHERE cidade IN ('São Paulo', 'Rio de Janeiro', 'Belo Horizonte');

-- Seleciona clientes que não vivem em 'São Paulo' ou 'Belo Horizonte'
SELECT nome, cidade
FROM clientes
WHERE cidade NOT IN ('São Paulo', 'Belo Horizonte');
```

Confira o vídeo para mais exemplos sobre o uso de `IN` e `NOT IN`:

<iframe width="560" height="315" src="https://www.youtube.com/embed/7M9-8yEwIGw?si=JLKBm1ZWoPsA6GCB" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---

## Próximos Passos

Esses conceitos são fundamentais para filtrar registros em consultas SQL e permitem a criação de consultas mais poderosas e eficientes.
