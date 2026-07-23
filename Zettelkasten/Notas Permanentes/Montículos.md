---
id: 202607231341
fecha: 23-07-2026
estado: borrador
tags:
  - EDyAI
  - EDyAII
---
# Montículos o Heaps: Rápido acceso al máx. o min. de los datos almacenados 
## La idea en una oración
---
> Un montículo es un árbol binario que siempre guarda en su raíz el elemento máximo o mínimo del conjunto de datos
## Desarrollo
---
Un montículo es una estructura de datos que guarda elementos en un árbol binario. Su invariante es: *Para todo nodo, su valor es el máximo o mínimo que el de sus hijos*

Sus ventajas son las que sigue:
- Permite una extracción del máximo o mínimo del conjunto de datos con coste $O(1)$
- Su inserción y eliminación suele ser eficiente, con coste posible de $O(lg(n))$
- Es más "barato" de implementar, ya que no garantiza orden en todos los datos, sólo la relación padre - hijos

Sin embargo:
- Buscar un elemento arbitrario en el mismo es ineficiente, siendo su coste de $O(n)$
- El árbol no suele ser balanceado, abriendo la posibilidad de que se degenere a una lista enlazada

Se usa en los siguientes casos:
- **Colas de prioridad:** La extracción del máximo o mínimo se vuelve veloz
- **Algoritmo de Dijkstra:** Es posible implementar un heap para obtener todos los caminos de un grafo, y poder extraer el de costo mínimo
- **Scheduler:** En Sistemas Operativos, un scheduler puede obtener las tareas de máxima prioridad a través de un montículo
## Conexiones
- [[Leftist Heap]]
- [[Skew Heap]]
