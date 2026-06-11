---
id: 202603122225
fecha: 12-03-2026
estado: borrador
tags:
  - CompMatI
---
# Def. de árbol recubridor
## La idea en una oración
---
> Un árbol recubridor de un grafo conexo es la creación de un subgrafo conexo acíclico por el proceso de eliminar aristas del grafo original. Esto nos permite un recorrido en grafos más eficiente si el árbol tiene peso
## Desarrollo
---
Todo grafo conexo contiene un árbol recubridor, y es posible armarlo eliminando poco a poco las aristas que forman ciclos en el grafo hasta tener un subgrafo acíclico. Este árbol nos permite recorrer todas las aristas con un único camino entre sí. Hay miles de maneras para crearlo, entre ellas el *BFS* y el *DFS*
Es más, tener un árbol recubridor en un grafo pesado nos permite descubrir cosas como caminos de menor peso desde una raíz, gracias al *árbol recubridor de peso mínimo*. No sólo eso, ya que si sólo queremos un camino de menor peso, podremos crearlo usando algoritmos como el de *Dijkstra* 
## Conexiones
- [[Árbol recubridor de peso mínimo]]
- [[BFS]]
- [[DFS]]
- [[Algoritmo de Dijkstra]]