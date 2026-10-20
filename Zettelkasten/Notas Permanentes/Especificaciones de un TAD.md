---
id: 202605131659
fecha: 13-05-2026
estado: completo
tags:
  - EDyAII
---
# Especificación del TAD
## La idea en una oración
---
> La especificación dicta qué devuelve cada operación según cómo se construyó el TAD
## Desarrollo
---
Una especificación solo describe qué estructuras se devuelven al aplicar una operación. Su conjunto de comportamientos es el que define las políticas de la misma. Recuerda que no se puede asumir nada de cómo se *implementa* la estructura en sí *(Los sets ordenados puede que no estén en orden de fila, una cola puede o no ser una lista)*

Una especificación es correcta si vale sus especificaciones base

Existe 2 especificaciones que se verán en la cátedra:
- Las **especificaciones algebraicas** son sobre ecuaciones donde sólo aparece operaciones del TAD y variables libres, que se suponen cuantificadas universalmente. Puede quedar comportamiento sin definir
- Las **especificaciones de modelo** se representa por un modelo matemático existente. Por ejemplo, para una cola, se puede usar una secuencia $(x_0,x_1,...,x_n)$ y definir las especificaciones sobre la misma. A cada TAD se le corresponde un modelo $[c]$, y cada operación $[op]$ tiene que trabajar sobre el modelo, por lo que
$$
[op \, c] = [op][c]
$$
> [!error] Atención
 ***No confundas especificación con implementación.*** No puedes asumir nada de cómo es la estructura en sí (un set ordenado puede no ser una lista o arreglo ordenado. Una cola puede implementarse de otra forma que no sea una lista simple). Sólo sabes como se comporta y ya
## Conexiones
- [[Especificación de costo]] 
