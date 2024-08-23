# Funções Condicionais

As funções condicionais em SQL Server permitem que você execute lógica condicional em suas consultas SQL, o que é útil para criar resultados dinâmicos e personalizados. Aqui estão algumas das funções mais importantes:

## Funções e Estruturas Condicionais

1. **CASE** - Permite executar lógica condicional e retornar valores diferentes com base em condições.

```sql
SELECT 
    Name,
    CASE 
        WHEN Age < 18 THEN 'Minor'
        WHEN Age >= 18 AND Age <= 65 THEN 'Adult'
        ELSE 'Senior'
    END AS AgeGroup
FROM People;
```

2. **IIF** - Uma versão simplificada da função CASE para avaliações de condições simples.

```sql
SELECT 
    Name,
    IIF(Age < 18, 'Minor', 'Adult') AS AgeGroup
FROM People;
```

3. **SUBSTRING()** - Extrai uma parte específica de uma cadeia de caracteres.

```sql
SELECT SUBSTRING(Name, 1, 4) AS ShortName
FROM People;
```

4. **TRIM()** - Remove espaços em branco à esquerda e à direita de uma cadeia de caracteres.

```sql
SELECT TRIM(Name) AS TrimmedName
FROM People;
```

5. **UPPER()** - Converte todos os caracteres de uma cadeia de caracteres para maiúsculas.

```sql
SELECT UPPER(Name) AS UpperCaseName
FROM People;
```

6. **LOWER()** - Converte todos os caracteres de uma cadeia de caracteres para minúsculas.

```sql
SELECT LOWER(Name) AS LowerCaseName
FROM People;
```

7. **TRANSLATE()** - Substitui caracteres específicos em uma cadeia de caracteres por outros caracteres.

```sql
SELECT TRANSLATE(Name, 'aeiou', 'AEIOU') AS TranslatedName
FROM People;
```

## Vídeos Explicativos sobre Funções Condicionais

Para uma explicação mais detalhada e exemplos práticos, assista aos vídeos abaixo:

### 1. SQL SERVER - 22 - Funções de Texto SUBSTRING, TRIM, UPPER, LOWER, TRANSLATE, CASE WHEN e IIF

<iframe width="560" height="315" src="https://www.youtube.com/embed/MtsUr3rMbTY?si=Mgdp5sXoOenw9xlu" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### 2. SQL SERVER - 33 - CASE - Estruturas de decisão para alterar forma de visualização dos dados

<iframe width="560" height="315" src="https://www.youtube.com/embed/V6Bnt6VwH8s?si=TO7iObKmaRpPoOZb" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---

## Próximos Passos

Essas funções e estruturas condicionais são essenciais para realizar análises mais complexas e personalizadas, permitindo que você transforme e formate dados conforme necessário.
