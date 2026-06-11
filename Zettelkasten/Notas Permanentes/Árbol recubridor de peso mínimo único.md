---
id: 202603152151
fecha: 15-03-2026
estado: completo
tags:
  - CompMatI
---
# Un árbol ponderado con pesos distintos en aristas tiene único árbol recubridor de peso mínimo
## La idea en una oración
---
> Usando *inducción* y el *Algoritmo de Prim*, se puede demostrar que todo grafo conexo ponderado con aristas de distinto peso tiene único árbol recubridor de peso mínimo 
## Desarrollo
---
Esto tiene una prueba inductiva sobre las aristas que tiene el grafo conexo, empezando desde la primera arista hasta la última
-  Sea G un grafo conexo ponderado donde todas las aristas tienen pesos distintos:
	1. **Caso base:** Considere el árbol de una sola arista. Como sólo se elige la arista de peso mínimo, hasta acá, el árbol tiene peso mínimo. Si hubiera dos de peso mínimo iguales, entonces habrían dos aristas del mismo peso, y por hipótesis, no es posible, por lo que es único
	2. **Caso inductivo:** Asume que el árbol T recubridor de peso mínimo es único con hasta $k$ aristas.  Según el Algoritmo de Prim, se inserta la siguiente arista de un vecino de un vértice en el árbol con un vértice que no está en el árbol. De ahora tener más de un árbol recubridor de peso mínimo con $k+1$ aristas, entonces, deberían haber dos aristas de peso iguales, pero esto no es posible por hipótesis, por lo que el árbol recubridor de peso mínimo con $k+1$ aristas sigue siendo único
	3. Como vale para un caso base y para el caso inductivo, vale para todo grafo conexo ponderado con pesos distintos en sus aristas
## Conexiones
- [[Algoritmo de Prim]] 
- [[Principio de Inducción Primitiva]]
