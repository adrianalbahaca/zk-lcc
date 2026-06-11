---
id: 202603181331
fecha: 18-03-2026
estado: completo
tags:
  - CompMatI
---
# Una desigualdad para verificar planaridad rápido
## La idea en una oración
---
> Sea $G$ grafo simple y planar con al menos 3 vértices, entonces $|E(G)| \le 3|V(G)| - 6$
## Desarrollo
---
Este teorema viene del Teorema de Euler como un corolario, y sirve como una forma rápida de verificar si un grafo puede ser planar o no lo es

> Sea $G$ grafo planar, simple y conexo tal que $|V(G)| \ge 3$, entonces, por el teorema de Euler, tenemos que $|V(G)|-|E(G)|+|C(G)|=2$
> Por proposición, también vale que $\sum_{caras} long(c) = 2|E(G)|$ 
> Ahora, por la cant. de vértices, cada cara debe tener por lo menos 3 fronteras, por lo que $\sum_{caras} long(c) = 2|E(G)| \ge 3|C(G)| \rightarrow |C(G)| \le 2/3 |E(G)|$ 
> Queda en el Teorema de Euler:
> $|C(G)|=2+|E(G)|-|V(G)| \rightarrow 2/3|E(G)|\le2+|E(G)|-|V(G)|$
> Y al simplificar, se llega a que $|E(G)|\le3|V(G)|-6$ $\blacksquare$ 

Esta desigualdad nos sirve en varios ejercicios teóricos
## Conexiones
- [[Teorema de Euler]] 
- [[Cotas ceñidas]]
