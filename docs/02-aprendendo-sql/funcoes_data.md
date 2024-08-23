# Funções de Data e Conversões de Tipos de Dados

No SQL Server, funções de data e conversões de tipos de dados são essenciais para manipular e transformar informações. Vamos explorar algumas funções comuns e como usá-las em suas consultas.

## Funções de Data

1. **GETDATE()** - Retorna a data e hora atuais do sistema.

```sql
SELECT GETDATE() AS CurrentDateTime;
```

2. **DATEDIFF(datepart, startdate, enddate)** - Calcula a diferença entre duas datas.

```sql
-- Diferença em dias entre duas datas
SELECT DATEDIFF(day, '2024-01-01', '2024-12-31') AS DaysDifference;
```

3. **DATEADD(datepart, number, date)** - Adiciona um intervalo a uma data.

```sql
-- Adiciona 10 dias à data atual
SELECT DATEADD(day, 10, GETDATE()) AS NewDate;
```

4. **DATEPART(datepart, date)** - Extrai uma parte específica de uma data, como ano, mês ou dia.

```sql
-- Extrai o ano da data atual
SELECT DATEPART(year, GETDATE()) AS CurrentYear;
   ```

## Conversão de Tipos de Dados

1. **CAST()** - Converte uma expressão de um tipo de dados para outro.

```sql
-- Converte uma string para um tipo de dados DATE
SELECT CAST('2024-08-23' AS DATE) AS ConvertedDate;
   ```

2. **CONVERT()** - Converte uma expressão de um tipo de dados para outro, com a opção de formato.

```sql
-- Converte uma data para uma string com formato específico
SELECT CONVERT(VARCHAR, GETDATE(), 103) AS FormattedDate;
```

### Vídeos Explicativos sobre Funções de Data e Conversões

Para entender melhor como usar essas funções, veja os vídeos abaixo:

#### 1. SQL SERVER - 16 - Funções de Data (GETDATE, DATEDIFF, DATEADD e DATEPART)

<iframe width="560" height="315" src="https://www.youtube.com/embed/WYdZhR1V99Q?si=YZt3RBMjQH5JvDvx" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

#### 2. Conversão de Tipos de Dados no SQL Server com CAST e CONVERT

<iframe width="560" height="315" src="https://www.youtube.com/embed/NlqVbtoQubA?si=pEGh6SB-E_JaBsHS" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

#### 3. Curso (PADAWAN) de SQL Server - Aula 07 - Funções SQL - CAST / CONVERT / YEAR / MONTH / DATEPART

<iframe width="560" height="315" src="https://www.youtube.com/embed/cpKewuzfpcU?si=fseQCFKakFn_mHhS" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---

## Próximos Passos

Essas funções e conversões são fundamentais para manipular datas e transformar tipos de dados em SQL Server, permitindo que você realize uma variedade de operações em suas consultas.
