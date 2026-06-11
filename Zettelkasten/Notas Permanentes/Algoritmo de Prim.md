---
id: 202603132319
fecha: 13-03-2026
estado: completo
tags:
  - CompMatI
---
# Alg. de Prim y casos de uso
## La idea en una oración
---
> El algoritmo de Prim es un algoritmo voraz que crea un árbol recubridor de peso mínimo empezando desde su inicio y poco a poco añadiendo las aristas de menor peso entre los vecinos de cada vértice
## Desarrollo
---
Si el grafo es demasiado denso, conseguir el árbol recubridor de peso mínimo usando el algoritmos de Kruskal puede ser una tarea demasiado tediosa, ya que obtener y ordenar todas las aristas consume bastante tiempo
Acá llega el algoritmo de Prim, un algoritmo *voraz* donde se basa en sólo buscar la arista de menor peso entre los vecinos de los vértices en el árbol y los vértices que no están aún en el árbol
Su pseudocódigo se ve así:

```
Alg_Prim(Grafo_Conexo_Ponderado G, Vertice origen in V(G)) {
	in_arbol[V(G)] = false
	dist[V(G)] = Infinity
	padre[V(G)] = NULL
	
	dist[origen] = 0
	
	while (in_arbol[v] for all v in V(G)) {
		u in V(G) : min(dist[u])
		in_arbol[u] = true
		
		for (v in V(G); uv in E(G)) {
			if (!in_arbol[v] and peso(u, v) < dist[v]) {
				dist[v] = peso(u, v)
				padre[v] = u
			}
		}
	}
	
	return padre
}
```

Este algoritmo nos permite demostrar que, si todos los pesos de las aristas son distintos entre sí, existe un único árbol recubridor de peso mínimo en el grafo
## Conexiones
- [[Programación greedy]] 
- [[Árbol recubridor de peso mínimo único]]
