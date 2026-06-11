---
id: 202605131649
fecha: 13-05-2026
estado: borrador
tags:
  - EDyAII
---
# Def. y utilidad de los tipos abstractos de datos
## La idea en una oración
---
> Un tipo abstracto de dato abstrae las operaciones e invariantes sobre las que se define una estructura, donde el usuario sólo interactúa con tal abstracción
## Desarrollo
---
Si tenemos a la cola, tenemos una serie de operaciones sobre ellas con ciertas invariantes. Definirla así es una definición es *abstracta*, refleja como se comporta, no cómo se implementa

Nuestra idea es *abstraer* detalles de la implementación, donde el usuario sólo usa la abstracción, y el implementador se asegura de que la interfaz cumple con las condiciones necesarias. Es como un contrato

**El usuario sólo puede suponer el comportamiento descripto**

Consiste de un nombre, las operaciones sobre las que se define y la especificación del comportamiento del *TAD*, que puede ser *algebraica*, o sobre ecuaciones, o mediante *modelos*, donde se usa un modelo matemático

Los costos de cada implementación varían, y tendrá su facilidad o dificultad de paralelizar

Ejemplo de definición de una Cola como un *TAD*:
```Haskell
tad Cola(A:Set) where
	import Bool
	empty : Cola A
	queue : A -> Cola A -> Cola A
	dequeue : Cola A -> Cola A
	peek : Cola A -> A
	isEmpty : Cola A -> Bool
```
## Conexiones
- [[Especificaciones de un TAD]]
- [[Cola con dos listas]]
- [[Costo amortizado]] *Ver esto*
- [[Paralelización en TADs]]
- [[Implementación de TAD]]
- [[Razonamiento sobre programas en Haskell]]