# Junções (JOINS)

No SQL, as junções (JOINS) são usadas para combinar linhas de duas ou mais tabelas com base em uma condição de relacionamento entre elas. Aqui está uma visão geral dos tipos mais comuns de junções:

### Tipos de Junções

1. **INNER JOIN** - Retorna apenas as linhas que têm correspondência em ambas as tabelas.
2. **LEFT JOIN (ou LEFT OUTER JOIN)** - Retorna todas as linhas da tabela da esquerda e as linhas correspondentes da tabela da direita. Se não houver correspondência, os resultados da tabela da direita terão valores `NULL`.
3. **RIGHT JOIN (ou RIGHT OUTER JOIN)** - Retorna todas as linhas da tabela da direita e as linhas correspondentes da tabela da esquerda. Se não houver correspondência, os resultados da tabela da esquerda terão valores `NULL`.
4. **FULL OUTER JOIN** - Retorna linhas quando há uma correspondência em uma das tabelas. Retorna todas as linhas da tabela da esquerda e da direita, com valores `NULL` onde não há correspondência.

### Exemplos de Código

#### INNER JOIN

```sql
-- Retorna funcionários e os departamentos aos quais estão associados
SELECT funcionarios.nome, departamentos.nome
FROM funcionarios
INNER JOIN departamentos
ON funcionarios.departamento_id = departamentos.id;
```

#### LEFT JOIN

```sql
-- Retorna todos os funcionários e os departamentos aos quais estão associados, mesmo que não tenham um departamento
SELECT funcionarios.nome, departamentos.nome
FROM funcionarios
LEFT JOIN departamentos
ON funcionarios.departamento_id = departamentos.id;
```

#### RIGHT JOIN

```sql
-- Retorna todos os departamentos e os funcionários associados, mesmo que não haja funcionários no departamento
SELECT funcionarios.nome, departamentos.nome
FROM funcionarios
RIGHT JOIN departamentos
ON funcionarios.departamento_id = departamentos.id;
```

#### FULL OUTER JOIN

```sql
-- Retorna todos os funcionários e departamentos, incluindo aqueles sem correspondência em uma das tabelas
SELECT funcionarios.nome, departamentos.nome
FROM funcionarios
FULL OUTER JOIN departamentos
ON funcionarios.departamento_id = departamentos.id;
```

---

### Vídeos Explicativos sobre Junções

Para aprofundar seu entendimento sobre junções no SQL, confira os vídeos a seguir:

#### 1. T-SQL - JOINS e INNER JOIN - Selecionar dados de duas ou mais tabelas

<iframe width="560" height="315" src="https://www.youtube.com/embed/4nbECYDlAwc?si=oJfn5rqeUGLu_yot" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

#### 2. T-SQL - OUTER JOINS - LEFT e RIGHT - Selecionar dados de várias tabelas

<iframe width="560" height="315" src="https://www.youtube.com/embed/mGbOaA1xWwk?si=qcW_zc_E0EOg2dUy" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

#### 3. T-SQL - FULL OUTER JOIN - Selecionar dados de várias tabelas

<iframe width="560" height="315" src="https://www.youtube.com/embed/8-DM11P8EhA?si=SrnWnUKJzgDfHx3H" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

#### 4. SQL SERVER - JOINs - Relacionamento entre tabelas (Inner Join, Right Join, Left Join e outros)

<iframe width="560" height="315" src="https://www.youtube.com/embed/HmFUrlQcCJ0?si=M9i0nVTwpDCK_kg0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---

## Próximos Passos

Essas junções são fundamentais para combinar e analisar dados que estão distribuídos em diferentes tabelas. Utilize-as para obter insights mais completos e realizar análises detalhadas em seus bancos de dados.
