---
id: 202603132302
fecha: 13-03-2026
estado: completo
tags:
  - CompMatI
---
# Alg. de Kruskal y casos de uso
## La idea en una oración
---
> El Algoritmo de Kruskal se basa en ordenar las aristas por su peso, e ir eligiendo desde la más ligera hasta la más pesada, sin crear ciclos, hasta formar un árbol del grafo
## Desarrollo
---
Con un grafo disperso, puede ser más práctico buscar el árbol recubridor de peso mínimo a partir de las aristas. Acá es donde llega este algoritmo
El algoritmo es *voraz (greedy)* y encuentra un árbol recubridor de peso mínimo en el grafo conexo. Su pseudocódigo se ve así

```
Alg-Kruskal(Grafo_Conexo_Ponderado G) {
	E <= E(G)
	E' <= []
	Ordernar E por el peso de las aristas
	V' <= []
	while (V' != V(G)) {
		e <= pop(E)
		if (!cycle([E' e]))
			E' <= [E' e]
		if (end_a(e) not in V') {
			V' <= [V' a]
		}
		if (end_b(e) not in V') {
			V' <= [V b]
		}
	}
	
	return E'
}
```

Este algoritmo se basa más en las aristas del grafo conexo, ordenándolas en una *estructura Union-Find* para después retornar las aristas que pertenecen al árbol recubridor buscado. Es mejor para grafos más dispersos, aquellos que no tienen demasiadas aristas
## Conexiones
- [[Programación greedy]] 
