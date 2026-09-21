---
id: 202608241302
fecha: 24-08-2026
estado: borrador
tags:
  - ALP
---
# Parser o analizador sintáctico 
## La idea en una oración
---
> Un parser procesa una cadena de caracteres y lo convierte en una estructura sintáctica
## Desarrollo
---
Un parser se encarga de mostrar la precedencia, orden y forma de lectura de una cadena de caracteres, usando ya sea Árboles de Sintáxis abstractos. Se va a buscar armar una librería para crear parsers

Un parser se puede pensar como sigue
```Haskell
type Parser a = String -> [(a, String)]
-- La lista vacía representa una falla y la unitaria es un éxito
-- a puede ser cualquier cosa, para considerar que el parser retorne distintos tipos de árboles
```
## Conexiones
- [[Parsers básicos]] 
