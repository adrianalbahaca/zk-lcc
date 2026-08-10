---
id: 202608101327
fecha: 10-08-2026
estado: borrador
tags:
  - ALP
---
# Problema del `else` colgado
## La idea en una oración
---
> El problema del `else` colgado muestra que, en su primera definición, puede haber dos árboles de parseo en la misma expresión
## Desarrollo
---
Tenga las siguientes reglas y las siguientes expresiones:
```
(COMPLETAR GRAMÁTICA)
if exp1 then (if exp2 then stc1 else stc2)
if exp1 then (if exp2 then stc1) else stc2
```

Note que ambas expresiones tienen dos árboles de parseo para la misma expresión pero con significados muy distintos. Para resolver este problema, se puede limitar a que entre `then` y `else` no puede contener un `if then`

```
stm ::= matched | unMatched
matched ::= if exp then matched else matched | ...
unMatched ::= if exp then stm | if exp then matched else unMatched
```

Acá se logra que la gramática tenga la regla que cada `else` esté asociado al `then` más cercano
## Conexiones
- [[Gramática ambigua]] 
