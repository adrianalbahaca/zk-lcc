---
id: 202603191431
fecha: 19-03-2026
estado: completo
tags:
  - CompMatI
---
# La primera cota de coloreado para grafos planares fue $\chi(G)\le6$  
## La idea en una oración
---
> Sea $G$ un grafo plano y simple, entonces $\chi(G) \le 6$  
## Desarrollo
---
Esta demostración es por *inducción* sobre la cantidad de vértices en un grafo plano simple

> - Caso base: 
> 	Asuma que el grafo sólo tiene un vértice. En ese caso, $\chi(G) = 1 \le 6$ 
> - Hipótesis inductiva: 
> 	Asuma que, para todo grafo simple y plano tal que $|V(G)|\le n$, $\chi(G)\le6$
> 	Entonces, para el grafo plano simple con $n+1$ aristas, sabemos que existe $v \in V(G)$ tal que $gr(v) \le 5$
> 	Considerando $G-v$, por $H.I$, $\chi(G)\le6$, por lo que al reinsertar $v$, debe tener a lo sumo 5 vecinos, por lo que hay a lo sumo 5 colores distintos
> 	Ahora, con a lo sumo 6 colores a usar, queda siempre un color libre para $v$, por lo que $\chi(G)\le6$
> Por inducción sobre el conjunto de grafos planares simples, se concluye que $\forall G$ plano y simple, $\chi(G)\le6$ $\blacksquare$ 

Ahora, hay una cota aún más ceñida, ya que se puede demostrar que, en realidad, $\chi(G)\le5$ en grafos
## Conexiones
- [[Cota ceñida de coloreado para grafos planares]] 
