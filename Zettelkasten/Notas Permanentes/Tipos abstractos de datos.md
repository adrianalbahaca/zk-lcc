---
id: 202605131649
fecha: 13-05-2026
estado: borrador
tags:
  - EDyAII
---
# Tipos Abstracto de Datos o TADs
## La idea en una oración
---
> Un TAD se encarga de abstraer el comportamiento de una estructura de datos de la implementación a través de una *especificación*
## Desarrollo
---
Si tenemos a la cola, tenemos una serie de operaciones sobre ellas con ciertas invariantes. Definirla así es una definición es *abstracta*, refleja como se comporta, no cómo se implementa

Ese es nuestro objetivo con un **Tipo Abstracto de Datos**, o *TAD*. Queremos abstraer los detalles de la implementación, y definir el comportamiento tal que no dependa del mismo. Así, modulamos el trabajo y las responsabilidades entre usuario e implementador
- El usuario sólo usará la abstracción, y sólo puede asumir el comportamiento definido en la misma. Sin embargo, no necesariamente debe saber la implementación
- El implementador se compromete a que su implementación cumpla con el comportamiento descripto. Tiene la libertad de implementar como quiera siempre y cuando lo que haga cumpla la *especificación*. En casos de comportamiento no descripto, se le da la libertad de que haga lo que quiera

Un TAD se compone de su nombre (`Cola` en este caso), sus operaciones y su *especificación*, o mejor dicho, cómo se comporta el TAD. Por ejemplo:

```Haskell
tad Cola(A:Set) where
	import Bool
	empty : Cola A
	queue : A -> Cola A -> Cola A
	dequeue : Cola A -> Cola A
	peek : Cola A -> A
	isEmpty : Cola A -> Bool

-- Nótese que la política FIFO es *implícita* en las ecuaciones definidas
dequeue (queue x empty) = empty
dequeue (queue y (queue x q)) = dequeue x q
peek (queue x empty) = x
peek (queue y (queue x q)) = peek x q
```
## Conexiones
- [[Especificaciones de un TAD]]
- [[Cola con dos listas]]
- [[Costo amortizado]] *Ver esto*
- [[Paralelización en TADs]]
- [[Implementación de TAD]]
- [[Razonamiento sobre programas]]