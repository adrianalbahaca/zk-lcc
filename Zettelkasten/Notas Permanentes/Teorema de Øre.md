---
id: 202603262209
fecha: 26-03-2026
estado: borrador
tags:
  - CompMatI
---
# Demo. y idea del teorema de Øre
## La idea en una oración
---
> Sea $G=(V,E)$ grafo simple, $|V| \ge 3$ y $gr(v)+gr(u) \ge |V|$, entonces $G$ tiene un ciclo hamiltoniano
## Desarrollo
---
Se basa con construcción de un camino hamiltoniano maximal y contradicción sobre el mismo

> Primero, si $G$ no fuera conexo, nota lo que pasa al sumar el grado posible de $v \in C_1$ y $u \in C_2$
> Ahora, asumiendo que $G$ con tales características no contenga un ciclo hamiltoniano
> Se arma $H$ subgrafo añadiendo aristas hasta que $H$ forme un ciclo hamiltoniano si se le añade una arista $xy$
> Luego, $H$ contiene un camino hamiltoniano $P_H$ desde $x$ hasta $y$
> Ahora, considere los posibles vértices $xv_{t}$ y $v_{t-1}y$. *Puede haber una o ninguna*, ya que, si hay ambas, el ciclo $xv_{2}...v_{t-1}yv_{n}...v_{t}$ sería ciclo hamiltoniano
> Mira las posibles $i$ opciones que $x$ e $y$ y mira sus grados. Verás una contradicción
> Por lo que $G$ tiene un ciclo hamiltoniano

Esta demostración es difícil de visualizar, pero cuando lo tienes, puedes usar esta estrategia para visualizar otras demostraciones por caminos hamiltonianos
## Conexiones
- [[Cond. suficiente de suma de grados para camino hamiltoniano]] 
