---
id: 202608241305
fecha: 24-08-2026
estado: borrador
tags:
  - ALP
---
# Parsers esenciales 
## La idea en una oración
---
> Un parser se construye a base de parsers esenciales, como el que lee un caracter, el que siempre falla o siempre tiene éxito
## Desarrollo
---
Para poder armar un parser complejo, se debe de basar sobre parsers más esenciales para construirlo

```Haskell
-- Se declara como newtype para definir un nuevo sinónimo de tipo
newtype Parser a = P (String -> [(a, String)])
```

El más esencial es el que lee un caracter
```Haskell
item :: Parser Char
item = P(\s -> if case s of
			    [] -> [] -- No se lee nada, es una falla
			    (x:ys) -> [(x, ys)]) -- Se guarda el caracter procesado
```

Luego, el siguiente es el que falla siempre y el que tenga siempre éxito
```Haskell
failure :: Parser a
failure = P (\_ -> [])

success :: a -> Parser a
success x = P (\s -> [(x, s)])
```

El operador `<|>` 
```Haskell
(<|>) :: Parser a -> Parser a -> Parser a
p <|> q = P (\s -> case parse p s of
					[] -> parse q s
					[(x, xs)] -> [(x, xs)])
```

La unión entre parsers se puede representar como `>>=`
```Haskell
(>>=) :: Parser a -> (a -> Parser b) -> Parser b
(p >>= f) s = case (parse p s) of
				[] -> []
				[(v, out)] -> parse (f v) out
```

Y usando secuenciamiento, es posible conectar varios parsers entre sí, como una lista de parsers secuenciados entre sí asociando a derecha. Su valor devuelto va a ser el devuelto por el último parser de la secuencia. Esta notación no es propia del operador `>>=` sino de cualquier mónada
```Haskell
do v1 <- p1
   v2 <- p2
   ...
   vn <- pn
   return (f v1 v2 ... vn)
```
## Conexiones
- [[]] 
