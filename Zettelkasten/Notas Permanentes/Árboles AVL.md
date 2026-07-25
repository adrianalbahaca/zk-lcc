---
id: 202607242332
fecha: 24-07-2026
estado: borrador
tags:
  - EDyAI
---
# AVLs para garantizar costes 
## La idea en una oración
---
> Los AVLs son árboles binarios de búsqueda balanceados, que garantizan búsquedas con costes óptimos
## Desarrollo
---
```Haskell
data AVL a = E | N (AVL a) a (AVL a) Int -- Altura de un nodo en particular

altura :: AVL a -> Int
altura E = 0
altura (N _ _ _ i) = i

factorBalance :: AVL a -> AVL a -> Int
factorBalance l r = (altura l) - (altura r)

calcAltura : : AVL a -> a -> AVL a -> AVL a
calcAltura l a r = N l a r (1 + max (altura l) (altura r))
```

```Haskell
rotLL :: AVL a -> AVL a
rotLL (N (N a x b) y c) = calcAltura a x (calcAltura b y c)

rotRR :: AVL a -> AVL a
rotRR (N a x (N b y c)) = calcAltura (calcAltura a x b) y c

rotLR :: AVL a -> AVL a
rotLR (N izq a der) = rotLL(calcAltura (rotRR izq) a der)

rotRL :: AVL a -> AVL a
rotRL (N izq a der) = rotRR (calcAltura izq a (rotLL der))
```
## Conexiones
- [[]] 
