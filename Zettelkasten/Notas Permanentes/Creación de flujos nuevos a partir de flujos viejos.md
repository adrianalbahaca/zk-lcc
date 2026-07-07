---
id: 202603282105
fecha: 28-03-2026
estado: completo
tags:
  - CompMatI
---
# Cómo se crea flujos nuevos con flujos viejos
## La idea en una oración
---
> Sea $f$ un flujo factible y $P$ un camino $f$-aumentante. Considere $\Delta = min(\epsilon (e) : e \in E(G))$. Entonces el nuevo flujo $f'$ tal que
$$
	f'(uv) =
	\begin{cases}
		f(uv) + \Delta \text{ Si uv es una arista propia}\\
		f(uv) - \Delta \text{ Si uv es una arista impropia}\\
		f(uv) \text{ En cualquier otro caso}
	\end{cases} 
$$
> es un flujo factible
## Desarrollo
---
Se usa analizando directamente si $f'$ cumple con las dos propiedades de un flujo factible
> Primero, se tiene que demostrar que $0 \le f'(e) \le c(e) \forall e \in E(G)$. Considera una arista impropia, y otra arista impropia. Luego, usando el principio de conservación de flujo, trabaja con las desigualdades
> Luego, es necesario demostrar que $\forall v \in V(G), f^+(v) = f^-(v)$. Para esto, suma todos los vértices considerando esta propiedad, y piensa en 4 casos: Cuando hay 2 aristas incidentes y propias en $v$, cuando hay 2 aristas incidentes impropias en $v$, cuando hay 2 aristas incidentes, una propia y otra impropia, y cuando hay 2 aristas incidentes, una impropia y otra propia

Es una demostración larga pero muy importante, ya que de esto se basa el algoritmo necesario para conseguir este flujo máximo
## Conexiones
- [[Algoritmo de Ford-Fulkerson]] 
