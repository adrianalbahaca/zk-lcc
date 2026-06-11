---
id: 202603271200
fecha: 27-03-2026
estado: completo
tags:
  - CompMatI
---
# Demo. de caract. de recorrido euleriano
## La idea en una oración
---
> Sea $G$ grafo conexo, entonces $G$ contiene un recorrido euleriano $\iff$ $G$ contiene exactamente dos vértices de grado par
## Desarrollo
---
Se demuestra de forma directa y por construcción

> $\Rightarrow )$ Sea $G$ conexo con recorrido euleriano, para sólo 2 vértices $u,v \in V(G)$ se tiene que entrar y salir respectivamente, por lo que sólo puede tener 2 vértices de grado impar
> $\Leftarrow )$ Sea $G$ conexo con 2 vértices $u,v$ de grado impar. Al añadir $uv$ como arista, todos los vértices terminan con grado par, por lo que habrá un circuito euleriano. Después, al remover $uv$, se rompe el circuito y queda un recorrido euleriano

Toma en cuenta que si tiene sólo 1 vértice de grado impar o más de 2 vértices de grado impar, $G$ no tendrá ni circuito ni recorrido euleriano
## Conexiones
- [[]] 
