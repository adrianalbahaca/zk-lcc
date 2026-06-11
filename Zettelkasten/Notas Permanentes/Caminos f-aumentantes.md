---
id: 202603282052
fecha: 28-03-2026
estado: borrador
tags:
  - CompMatI
---
# Def. de camino $f$-aumentante
## La idea en una oración
---
> Sea un flujo factible $f$, un camino $f$-aumentante es un camino simple en la red $G$ tal que $f(e)<c(e)$ para aristas propias o $f(e)>0$ para aristas impropias
## Desarrollo
---
Para resolver el problema del flujo máximo en una red, se ha descifrado un algoritmo que se basa en una búsqueda de caminos especiales en una red: Los caminos $f$-aumentantes
Esto se debe a que un flujo máximo no contiene tales caminos, por lo que se usan para poco a poco expandir el flujo a uno nuevo más grande a partir de uno antiguo
## Conexiones
- [[Creación de flujos nuevos a partir de flujos viejos]]
- [[Algoritmo de Ford-Fulkerson]]
- [[Construcción de estructuras]]
