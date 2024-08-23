# UNION e EXCEPT

No SQL, `UNION` e `EXCEPT` são operadores usados para combinar ou comparar conjuntos de resultados de consultas. Eles são úteis para unir resultados de diferentes consultas ou para encontrar diferenças entre conjuntos de dados.

### Tipos de Operadores

1. **UNION** - Combina os resultados de duas ou mais consultas `SELECT`. Remove duplicatas por padrão. Para incluir duplicatas, use `UNION ALL`.

2. **EXCEPT** - Retorna os resultados da primeira consulta `SELECT` que não estão presentes na segunda consulta `SELECT`.

### Exemplos de Código

#### UNION

```sql
-- Combina resultados de duas tabelas, removendo duplicatas
SELECT nome FROM clientes
UNION
SELECT nome FROM fornecedores;
```

#### UNION ALL

```sql
-- Combina resultados de duas tabelas, mantendo duplicatas
SELECT nome FROM clientes
UNION ALL
SELECT nome FROM fornecedores;
```

#### EXCEPT

```sql
-- Retorna clientes que não são fornecedores
SELECT nome FROM clientes
EXCEPT
SELECT nome FROM fornecedores;
```

### Vídeos Explicativos sobre UNION e EXCEPT

Para aprofundar seu entendimento sobre `UNION` e `EXCEPT`, confira os vídeos a seguir:

#### 1. T-SQL - UNION - Unir resultados de declarações SELECT

<iframe width="560" height="315" src="https://www.youtube.com/embed/3DzTn4Ff5Mg?si=RVXil40Lie3yhjtQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

#### 2. SQL SERVER - 23 - UNION e UNION ALL

<iframe width="560" height="315" src="https://www.youtube.com/embed/wLwGM60yevA?si=Y_F5iI2xU9c1wYf2" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

#### 3. Mastering the EXCEPT Keyword in SQL Server

<iframe width="560" height="315" src="https://www.youtube.com/embed/95Gsa4tIjlw?si=63HTXMCvYCPMmoMA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---

## Próximos Passos

Esses operadores são essenciais para trabalhar com conjuntos de dados em SQL, permitindo combinar e comparar informações de maneira eficaz. Utilize-os para realizar análises complexas e obter insights detalhados dos seus dados.
