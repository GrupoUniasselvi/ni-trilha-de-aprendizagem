# Funções de Texto

As funções de texto em SQL Server permitem que você trabalhe com e manipule cadeias de caracteres de várias maneiras. Aqui estão algumas das funções mais comuns e como usá-las:

## Funções Básicas

1. **CONCAT()** - Concatena duas ou mais cadeias de caracteres.

```sql
SELECT CONCAT('Olá, ', 'Mundo!') AS Greeting;
```

2. **CHARINDEX()** - Retorna a posição inicial de uma substring dentro de uma cadeia de caracteres.

```sql
SELECT CHARINDEX('World', 'Hello World') AS Position;
```

3. **LEN()** - Retorna o comprimento de uma cadeia de caracteres.

```sql
SELECT LEN('Hello World') AS Length;
```

4. **LEFT()** - Retorna um número especificado de caracteres a partir do início de uma cadeia de caracteres.

```sql
SELECT LEFT('Hello World', 5) AS Substring;
```

5. **RIGHT()** - Retorna um número especificado de caracteres a partir do final de uma cadeia de caracteres.

```sql
SELECT RIGHT('Hello World', 5) AS Substring;
```

6. **UPPER()** - Converte todos os caracteres de uma cadeia de caracteres para maiúsculas.

```sql
SELECT UPPER('Hello World') AS UpperCase;
```

7. **LOWER()** - Converte todos os caracteres de uma cadeia de caracteres para minúsculas.

```sql
SELECT LOWER('Hello World') AS LowerCase;
```

## Funções Avançadas

1. **REPLACE()** - Substitui todas as ocorrências de uma substring por outra.

```sql
SELECT REPLACE('Hello World', 'World', 'SQL') AS ReplacedString;
```

2. **RTRIM()** - Remove os espaços em branco à direita de uma cadeia de caracteres.

```sql
SELECT RTRIM('Hello World    ') AS TrimmedRight;
```

3. **LTRIM()** - Remove os espaços em branco à esquerda de uma cadeia de caracteres.

```sql
SELECT LTRIM('    Hello World') AS TrimmedLeft;
```

4. **PATINDEX()** - Retorna a posição inicial da primeira ocorrência de um padrão em uma cadeia de caracteres.

```sql
SELECT PATINDEX('%World%', 'Hello World') AS PatternPosition;
```

5. **REPLICATE()** - Repete uma cadeia de caracteres um número especificado de vezes.

```sql
SELECT REPLICATE('Hello ', 3) AS RepeatedString;
```

6. **REVERSE()** - Inverte a cadeia de caracteres.

```sql
SELECT REVERSE('Hello World') AS ReversedString;
```

7. **STRING_AGG()** - Concatena valores de uma coluna em uma única cadeia de caracteres, separados por um delimitador.

```sql
SELECT STRING_AGG(Name, ', ') AS NamesList FROM Employees;
```

8. **SPACE()** - Retorna uma cadeia de caracteres com um número especificado de espaços em branco.

```sql
SELECT SPACE(5) AS Spaces;
```

9. **STUFF()** - Substitui parte de uma cadeia de caracteres com outra cadeia.

```sql
SELECT STUFF('Hello World', 6, 5, 'SQL') AS StuffedString;
```

## Vídeos Explicativos sobre Funções de Texto

Para uma visão mais detalhada sobre como usar essas funções, veja os vídeos abaixo:

### 1. T-SQL - Concatenação de Strings

<iframe width="560" height="315" src="https://www.youtube.com/embed/ghbCZwQPY24?si=AoxU3FtaKWJeMrxE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### 2. SQL SERVER - 17 - Funções de Texto ASCII, NCHAR, CHAR, CHARINDEX, CONCAT, CONCAT_WS e DIFFERENCE

<iframe width="560" height="315" src="https://www.youtube.com/embed/hgX5wwQuriA?si=4ZbXjavO71Gj3R0v" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### 3. SQL SERVER - 18 - Funções de Texto FORMAT, LEFT, RIGHT, LEN, LOWER e UPPER

<iframe width="560" height="315" src="https://www.youtube.com/embed/9s046WsHEbk?si=-Av6u1k6YRfibIEF" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### 4. SQL SERVER - 19 - Funções de Texto LTRIM, RTRIM, PATINDEX, REPLACE, REPLICATE e REVERSE

<iframe width="560" height="315" src="https://www.youtube.com/embed/8gkBIGdmQU0?si=riiBVQaWTgv_mhkb" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### 5. SQL SERVER - 20 - Funções de Texto STRING_AGG, SPACE e STUFF

<iframe width="560" height="315" src="https://www.youtube.com/embed/K_R-uAQmTQU?si=Bx0Hb_1BaPUMkwoq" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---

## Próximos Passos

Essas funções são muito úteis para manipular e processar textos em SQL Server, ajudando a preparar e formatar dados para relatórios e outras operações.
