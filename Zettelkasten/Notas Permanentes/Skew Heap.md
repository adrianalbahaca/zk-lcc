---
id: 202607231317
fecha: 23-07-2026
estado: completo
tags:
  - EDyAII
---
# Skew Heap para merge sencillo 
## La idea en una oración
---
> Un Skew Heap, o montículo sesgado, permite tener un costo de $O(lg(n))$ sesgado en cada inserción y eliminación en el heap
## Desarrollo
---
Una de las estrategias para hacer un merge en un heap es *siempre* intercambiar las ramas de forma incondicional, como ocurre en el **Skew heap**. De esta forma, su costo de inserción y eliminación se queda de forma amortizada en $O(lg(n))$, en promedio ese es el costo pero no siempre

Los invariantes del Skew Heap son:
- Para cada nodo, su valor es menor o igual (o mayor o igual) al de todos sus hijos

```Haskell
data Heap a = E | N (Heap a) a (Heap a)

-- Ejemplo para un MinHeap
merge :: Ord a => Heap a -> Heap a -> Heap a
merge h1 E = h1
merge E h2 = E
merge h1@(N l1 a1 r1) h2@(N l2 a2 r2) =
	| a1 < a2 = N (merge r1 h2) a1 l1
	| otherwise = N (merge h1 r2) a2 l2 
```

De esta manera, no es necesario mantener contado los niveles del heap durante las pasadas

Ventajas:
- Implementación sencilla en ausencia de un contador de niveles
- Coste amortizado de $O(lg(n))$
Desventajas:
- En el peor de los casos, puede degenerar a una lista simplemente enlazada, causando costos de $O(n)$ 
## Conexiones
- [[Montículos]] 
