---
id: 202603191441
fecha: 19-03-2026
estado: completo
tags:
  - CompMatI
---
# $\chi(G)\le5$ para grafos planares 
## La idea en una oración
---
> Sea $G$ un grafo plano, entonces $\chi(G)\le5$ 
## Desarrollo
---
Esta cota permite ceñir incluso aún más al coloreado de los grafos

> Se aplica inducción sobre la cantidad de vértices en el grafo
> **Caso base:** De tener $|V(G)| <= 5$, se puede colorear con hasta 5 colores fácilmente
> **Hipótesis inductiva:** Todo grafo con hasta $k$ vértices es 5-coloreable
> **Paso inductivo:** Sea $G$ grafo planar con $k+1$ vértices, entonces debe tener un vértice tal que $gr(v)\le5$. Con $G-v$ por *H.I*, es 5-coloreable, entonces se agrega $v$ de vuelta
> - Si $gr(v)<5$, entonces se puede colorear con un quinto color
> - Si $gr(v)=5$, sean $v1,v2,v3,v4,v5$ los vecinos de $v$, y piensa en los **Caminos de Kempe** que cruza a $v1, v3$
> 	- Si $v3$ no está incluido, entonces se puede intercambiar los colores del camino de Kempe con $v1$, y se tiene un color libre para $v$
> 	- Si $v3$ está incluido, entonces debe haber un ciclo que pase por $v1$ y $v3$, encerrando a $v2$ e impidiendo que tenga un camino de Kempe que pase por $v4$ sin romper planaridad o el camino de Kempe $v1-v3$, por lo que se intercambian los colores del camino de Kempe con $v2$ y se tiene un color libre para $v$
> De esta manera, $G$ con $k+1$ vértices también es 5-coloreable
> Por inducción, se concluye que todo grafo planar es 5-coloreable $\blacksquare$ 

Esta cota usa los *Caminos de Kempe* para indicar que siempre es posible mover los colores para asegurar un color libre para el vértice suelto
## Conexiones
- [[Caminos de Kempe]] 
