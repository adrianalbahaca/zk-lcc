---
id: 202605131239
fecha: 13-05-2026
estado: borrador
tags:
  - EDyAII
---
# Árboles Red-Black inmutables 
## La idea en una oración
---
> Al insertar un elemento en un RBT, el rebalanceo se hace *de vuelta hacia la raíz* durante la copia del camino, de forma natural
## Desarrollo
---
Un Red-Black Tree es un árbol binario autobalanceable que cumple 2 invariantes:
- Ningún nodo de color rojo tiene un hijo de color rojo
- Todo camino de la raíz a una hoja tiene la misma cantidad de nodos negros. A esto se le llama altura negra

Como árbol inmutable, su inserción se vuelve más sencilla
```Haskell
data Color = R | B
data RBT a = E | T Color (RBT a) a (RBT a)

insert :: Ord a => a -> RBT a -> RBT a
insert a t = makeBlack(ins x t)
	where
		ins x E = T R E x E
		ins x (T c l a r)
		| x < y = balance c (ins x l) a r
		| x > y = balance c l a (ins x r)
		| otherwise = T c l a r
		makeBlack E = E
		makeBlack (T _ l a r) = T B l a r
```

Luego, usando como referencia la solución de Oyasaki, tenemos que el rebalanceo cuando un nodo rojo tiene algún hijo rojo queda como sólo 4 casos:

```Haskell
balance :: Ord a => Color -> RBT a -> a -> RBT a
balance B (T R (T R a x b) y c) z d = T R (T B a x b) y (T B c z d)
balance B (T R a x (T R b y c)) z d = T R (T B a x b) y (T B c z d)
balance B a x (T R (T R b y c) z d) = T R (T B a x b) y (T B c z d)
balance B a x (T R b y (T R c z d)) = T R (T B a x b) y (T B c z d)
balance c l a r = T c l a r
```
## Conexiones
- [[Árboles Red-Black]] 
