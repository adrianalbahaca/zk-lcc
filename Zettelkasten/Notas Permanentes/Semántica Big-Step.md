---
id: 202608311510
fecha: 31-08-2026
estado: completo
tags:
  - ALP
---
# Big-step 
## La idea en una oración
---
> La semántica big-step oculta el paso a paso que se ha aplicado para llegar al resultado final
## Desarrollo
---
Piénsalo como un "salto en el tiempo" donde desde unos *términos* se llega a un *valor*. Entonces, queda los siguientes conjuntos
```
T => t ::= T | F | if t then t else t
V => v ::= T | F
```

Nota que `t` y `v` son *metavariables*, variables donde una representa el mismo objeto, pero que entre sí no necesariamente representen objetos distintos
## Conexiones
- [[]] 
