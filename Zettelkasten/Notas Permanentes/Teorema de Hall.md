---
id: 202603231942
fecha: 23-03-2026
estado: borrador
tags:
  - CompMatI
---
# Teorema de Hall: Demo. inductiva y usos
## La idea en una oración
---
> Sea $G[X,Y]$ grafo bipartito. Existe un $M$ matching que sature a $X$ $\iff$ para todo $S \subseteq X$, cumple que $|N(S)| \ge |S|$
## Desarrollo
---
Este teorema se demuestra por construcción e inducción sobre los vértices de $G$

> $\Rightarrow )$ Sea $G[X,Y]$ grafo bipartito tal que existe un matching máximo que sature a $X$ Entonces, se cumple el otro lado trivialmente
> $\Leftarrow )$ Sea $G[X,Y]$ grafo bipartito tal que, para todo $S \subseteq X$, cumple que $|N(S)| \ge S$. Asume que no existe tal matching y considera $u \in X$ no saturado por $M$ matching máximo. Mira los vértices *alcanzables por $u$ usando caminos $M$-alternantes*. Haz la intersección con $X$ e $Y$, nota lo que pasa con $N_G(Y')$ y verás que se contradice la hipótesis, por lo que existe un $M$ matching máximo que satura a $X$. $\blacksquare$ 

Este teorema nos permite verificar si es posible saturar todo un lado de un grafo bipartito, viendo que, sino, hay un subconjunto tales que sus vecinos son menores que sus vértices
**Importante:** Para demostrar, mira los vértices alcanzables por $u$ libre por caminos $M$-alternantes
## Conexiones
- [[]] 
