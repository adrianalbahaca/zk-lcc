---
id: 202605131659
fecha: 13-05-2026
estado: borrador
tags:
  - EDyAII
---
# Def. de especificación
## La idea en una oración
---
> La especificación se refiere a qué operaciones tiene el TAD y cómo se comportan. Es única
## Desarrollo
---
La especificación sólo garantiza su especificación, pero la especificación no es lo mismo que implementación. Las especificación son sólo operaciones matemáticas o de modelo. No es posible suponer algún orden o resultado

Una especificación es correcta si vale sus especificaciones base

Las especificaciones algebraicas son sobre ecuaciones donde sólo aparece operaciones del TAD y variables libres, que se suponen cuantificadas universalmente. Puede quedar comportamiento sin definir

Las especificaciones de modelo se representa por un modelo matemático existente. Por ejemplo, para una cola, se puede usar una secuencia $(x_0,x_1,...,x_n)$ y definir las especificaciones sobre la misma. A cada TAD se le corresponde un modelo $[c]$, y cada operación $[op]$ tiene que trabajar sobre el modelo, por lo que
$$
[op \, c] = [op][c]
$$
(Repasar más esta parte)
*Cada TAD tiene múltiples implementaciones posibles*
## Conexiones
- [[Especificación de costo]] 
