---
id: 202607231325
fecha: 23-07-2026
estado: completo
tags:
  - EDyAII
---
# Leftist heap para garantía de camino corto
## La idea en una oración
---
> Un leftist heap tiene el beneficio de garantizar un camino corto en la espina derecha. Es simple de implementar, pero es necesario llevar cuentas de cada rango al insertar
## Desarrollo
---
Un leftist heap es un montículo con los siguientes invariantes
- Para cada nodo, su valor es menor o igual (o mayor o igual) que el valor de sus hijos
- Para cada nodo, el `Rank` del hijo derecho es menor o igual al `Rank` del hijo izquierdo

Como consecuencia, este montículo tiene ciertas propiedades:
- La espina derecha es el camino más corto a un nodo vacío
- Los elementos de la espina derecha están ordenados
- Siendo $n$ la cant. de nodos, el rango es a lo sumo $lg(n+1)$

```Haskell
type Rank = Int
data Heap a = E | N Rank a (Heap a) (Heap a)

rank :: Heap a -> Rank
rank E = 0
rank (N r _ _ _) = r

merge :: Ord a => Heap a -> Heap a -> Heap a
merge h1 E = h1
merge E h2 = h2
merge h1@(N r1 a1 l1 r1) h2@(N r2 a2 l2 r2)
	| r1 < r2 = makeH r1 a1 (merge r1 h2) 
	| otherwise = makeH r2 a2 (merge h1 r2)
	where
		makeH r a b =
			if rank a > rank b then N (rank b + 1) r a b
			else N (rank a + 1) r b a
```
## Conexiones
- [[Montículos]] 
