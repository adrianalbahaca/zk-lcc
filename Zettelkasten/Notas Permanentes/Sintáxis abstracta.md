---
id: 202608101413
fecha: 10-08-2026
estado: borrador
tags:
  - ALP
---
# Sintáxis abstracta
## La idea en una oración
---
> La sintáxis abstracta se zafa de la ambiguedad ya que tenemos el AST, representando todos con árboles
## Desarrollo
---
En Haskell, se puede usar `data` para determinar una expresión, donde sus elementos son árboles y los nombres de constructores son abstractos

```Haskell
data Exp = Num Int | Sum Exp Exp | Prod Exp Exp | Minus Exp Exp
```


## Conexiones
- [[Árbol de sintáxis abstracto]] 
