---
id: 202605231820
fecha: 23-05-2026
estado: completo
tags:
  - Lógica
---
# Def. de secuencia de formación
## La idea en una oración
---
>  Una secuencia $\phi_1 \phi_2 ... \phi_n$ es una secuencia de formación para $\phi$, si $\phi_n = \phi$ y cumple que las anteriores $\phi_i$ son atómicas, o vienen de la composición de anteriores $\phi_j$
## Desarrollo
---
De forma formal, la secuencia será de formación si
- $\phi_n = \phi$
- $\forall i \ge n, \phi_i$ es atómica o 
	- $\phi_i = (\phi_j \square \phi_k), j,k < i$ 
	- $\phi_i = \neg \phi_j, j<i$ 

La secuencia de formación y el conjunto $PROP$ están relacionados por un *teorema*
> $\phi$ tiene una secuencia de formación $\iff$ $\phi \in PROP$ 
> $\Rightarrow)$ Demostrar por inducción sobre el tamaño de la secuencia
> $\Leftarrow)$ Demostrar sobre el PIP del conjunto $PROP$ 
## Conexiones
- [[Conjunto PROP]] 
