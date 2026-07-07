---
id: 202603251521
fecha: 25-03-2026
estado: borrador
tags:
  - CompMatI
---
# Def., demo. y usos del Teorema de König-Egérvary
## La idea en una oración
---
> Sea $G$ un grafo bipartito, entonces $\alpha '(G) = \beta(G)$ 
## Desarrollo
---
Este teorema se basa en uno ya visto para grafos generales, donde $\alpha '(G) \le \beta (G)$ y extrapola la igualdad a grafos bipartitos

> Sea $G[X,Y]$ grafo bipartito, se sabe que $\alpha '(G) \le \beta (G)$ para todo grafo
> Basándonos en $C$ cubrimiento de aristas por vértices óptimo, se construye un matching con el mismo tamaño
> Considera $L=C \cap X$ y $R = C \cap Y$, y sean los grafos inducidos $H=G[L \cup (Y-R)]$ y $H'=G[R \cup X-L]$
> Nota que ambos grafos son separados entre sí. No comparten vértices por el cubrimiento $C$
> Luego, se tiene que demostrar que $H$ y $H'$ cumplen el teorema de Hall para saturar $L$ y $R$ respectivamente
> Finalmente $|M|=|L|+|R|=|C|$ y se concluye que $\alpha '(G)=\beta (G)$ $\blacksquare$ 

De esta forma, si el grafo es bipartito, entonces es posible determinar $\alpha '$ con $\beta$ y viceversa
## Conexiones
- [[Matching]]
- [[Cubrimiento de aristas por vértices]]
