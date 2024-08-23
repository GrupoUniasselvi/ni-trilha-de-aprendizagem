# Group By e Funções de Agregação

As funções de agregação no SQL são utilizadas para realizar cálculos em um conjunto de valores e retornar um único valor. Elas são frequentemente usadas em conjunto com a cláusula `GROUP BY` para agrupar os resultados de uma consulta com base em uma ou mais colunas.

### Funções de Agregação

1. **SUM** - Soma dos valores.
2. **AVG** - Média dos valores.
3. **COUNT** - Contagem de registros ou valores.
4. **MIN** - Menor valor.
5. **MAX** - Maior valor.

### Exemplos de Funções de Agregação

```sql
-- Soma o total de vendas por produto
SELECT produto, SUM(valor_venda) AS total_vendas
FROM vendas
GROUP BY produto;

-- Calcula a média de idade dos clientes
SELECT AVG(idade) AS media_idade
FROM clientes;

-- Conta o número total de clientes em cada cidade
SELECT cidade, COUNT(*) AS total_clientes
FROM clientes
GROUP BY cidade;

-- Encontra o menor e o maior salário por departamento
SELECT departamento, MIN(salario) AS menor_salario, MAX(salario) AS maior_salario
FROM funcionarios
GROUP BY departamento;
```

---

## STDEVP - Função para Cálculo do Desvio Padrão Populacional

A função `STDEVP` calcula o desvio padrão populacional de um conjunto de valores. Ela pode ser útil quando você quer medir a dispersão ou variação de um conjunto de dados. O desvio padrão é uma métrica importante em estatística para entender a variação em relação à média.

**Documentação Oficial:**

[STDEVP (Transact-SQL) - Documentação Microsoft](https://learn.microsoft.com/pt-br/sql/t-sql/functions/stdevp-transact-sql)

**Exemplo de código:**

```sql
-- Calcula o desvio padrão populacional dos salários dos funcionários
SELECT STDEVP(salario) AS desvio_padrao_salarios
FROM funcionarios;
```

---

### Vídeos Explicativos sobre Funções Agregadas

Para aprofundar seu entendimento, confira estes vídeos que cobrem as funções agregadas `SUM`, `COUNT`, `MAX`, `MIN`, `AVG`:

#### 1. T-SQL - Funções Agregadas - SUM, COUNT, MAX, MIN, AVG - SQL Server

<iframe width="560" height="315" src="https://www.youtube.com/embed/4B3adlQpHSo?si=Ce5PWe-1WzC-fAUk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

#### 2. SQL SERVER - Funções de Agregação (SUM, COUNT, AVG, MAX e MIN)

<iframe width="560" height="315" src="https://www.youtube.com/embed/tBJsOkGe4fE?si=WfgHhFhzHB9oSAaV" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---

## Próximos Passos

Essas funções são essenciais para realizar análises e sumarizar dados em grandes conjuntos de registros. Utilize a cláusula `GROUP BY` sempre que precisar agrupar os resultados por uma ou mais colunas, e aplicar as funções de agregação para gerar resultados relevantes para análises estatísticas ou relatórios.
