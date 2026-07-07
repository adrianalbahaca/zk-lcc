---
id: 202603232131
fecha: 23-03-2026
estado: borrador
tags:
  - CompMatI
---
# Caminos $M$-aumentantes y Algoritmo de Benge para matching máximo
## La idea en una oración
---
> Un camino $M$-aumentante es un camino que altera entre aristas del matching $M$ empezando y terminando en vértices no saturados. Para conseguir un matching máximo, añades primero una arista y, mientras creas caminos $M$-aumentantes, vas aumentando tal matching por 1 hasta que no sea posible expandirlo a un camino $M$-aumentante o que no haya caminos $M$-aumentantes
## Desarrollo
---
Este algoritmo se basa en un teorema:

> Un $M$ matching es máximo $\iff$ no posee un camino $M$-aumentante

Entonces, el algoritmo se basa en lo siguiente:
- Empieza añadiendo una arista al matching M
- Crea un camino $M$-aumentante y expande el matching, añadiendo las aristas no saturadas de $M$ y removiendo las aristas saturadas de $M$
- Continúa así hasta que no sea posible expandirlo más con caminos $M$-aumentantes, ya sea porque se saturó una de las biparticiones o porque no ha suficientes vértices libres para hacerlo
Este algoritmo es mucho más simple que usar isomorfismos, aunque puede ser que a los profes no les guste y prefieran una demostración más analítica
## Conexiones
- [[]] 
