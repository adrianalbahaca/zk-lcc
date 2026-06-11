---
id: 202606021659
fecha: 02-06-2026
estado: borrador
tags:
  - EDyAII
---
# La secuencia como un TAD 
## La idea en una oración
---
> Una secuencia es un TAD que contiene las funciones `empty, singleton, length, nth, toSeq, append, take, drop, tabulate` (Aplicando la función de naturales a tipo `a` a todos los elementos de la secuencia) `, map, filter` (Que recibe un predicado) `, foldr (a -> b -> b) -> b -> Seq a -> b` (Una forma de aplicar una función de atrás para adelante de forma recursiva en la secuencia) `, foldl ((b -> a -> b) -> b -> Seq a -> b)` (A definir en clase) `, reduce` (Evalúa suma con respecto a operador de la secuencia)  
## Desarrollo
---
Como notación se tiene:
$$
\begin{align*}
	\text{Longitud = } |s| \\
	\text{Un índice } i \in \mathbb{N} \text{ es válido si } 0 \le i \le |s| \\
\end{align*}
$$
`reduce` tiene algunas características:
- Si `e` es neutro con respecto del operador, actúa como `foldr op e` y `foldl op e`
- Si el operador no es asociativo, se pueden obtener distintos resultados dependiendo del orden de reducción. Esto nos indica que limitarse a funciones asociativas no es una buena idea, y *nos pide cuidado en cómo asociamos las operaciones*. Por lo que, para el TAD, se define un orden de reducción, ya sea transformando la secuencia en un árbol
## Conexiones
- [[Vista de una secuencia como un árbol]]
- [[Operación reduce en Secuencias]]
- [[Operación scan en Secuencias]]
