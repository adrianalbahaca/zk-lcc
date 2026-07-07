---
id: 202603152154
fecha: 15-03-2026
estado: completo
tags:
  - CompMatI
---
# Def. de Alg. de Dijkstra y sus caso de uso 
## La idea en una oración
---
> El algoritmo de Dijkstra crea una estructura que contiene caminos mínimos desde cualquier punto hasta cualquier otro. Esto es súper útil, a pesar de que es un algoritmo medio tedioso. **Estate muy pendiente de la tabla**
## Desarrollo
---
 No siempre queremos focalizarnos en un punto de entrada único para conseguir el camino menos pesado. A veces, queremos tener todos los caminos posibles
 Acá llega este algoritmo *voraz*, que descubre todos estos caminos. La idea es guardar poco a poco el peso de cada paso a hacer, consiguiendo el camino para cada vecino de cada vértice
 Acá está el pseudocódigo

```
Alg_Dijkstra(Grafo_Conexo_Ponderado G, Vertice v in V(G)) {
	visitado[V(G)] = false
	dist[V(G)] = Infinity
	padre[V(G)] = NULL
	
	dist[origen] = 0
	
	while (visitado[v] for all v in V(G)) {
		u in V(G) : min(dist[u])
		visitado[u] = true
		
		for (v in V(G) : uv in E(G)) {
			if (dist[u] + peso(u ,v) < dist[v]) {
				dist[v] = dist[u] + peso(u, v)
				padre[v] = u
			}
		}
	}
	
	return padre
}
```

Este algoritmo puede ser tedioso, por lo que **se tiene que estar muy pendiente de cómo se desarrolla el algoritmo con una tabla que mantenga el sucesor y el peso actual guardado**, pero este algoritmo puede conseguir caminos mínimos desde y hasta cualquier punto
## Conexiones
- [[Programación greedy]] 
