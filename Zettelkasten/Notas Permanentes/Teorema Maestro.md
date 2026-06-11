---
id: 202603232158
fecha: 23-03-2026
estado: completo
tags:
  - EDyAII
---
# Def. y uso del teorema maestro
## La idea en una oración
---
> Sea $T(n)$ una función suave con la forma $T(n) = aT(n/b)+f(n)$ con $a\ge 1$ y $b > 1$, compara $f(n)$ con $log_b(a)$ directamente para tener su respuesta
## Desarrollo
---
Con una función $T(n)$ suave con la forma pedida y $\epsilon >1$, tenemos 3 casos
- Si $f(n) \in O(n^{log_b(a)-\epsilon})$, entonces la función $f(n)$ crece lentamente, y la mayoría del trabajo se acumula en las hojas, por lo que $T(n) \in \Theta (n^{log_b(a)})$ 
- Si $f(n) \in \Theta (n^{log_b(a)})$, entonces la función $f(n)$ crece con la misma magnitud que el trabajo, y se concluye que $T(n) \in \Theta (n^{log_b(a)} * log(n))$ 
- Si $f(n) \in \Omega(n^{log_b(a)+\epsilon})$ y $f(b)$ es suave, entonces $f(n)$ crece más rápido que el trabajo total, haciendo la mayoría del trabajo. Allí, $T(n) \in \Theta(f(n))$ 

De esta manera, no es necesario usar arbol de recurrencia ni método de sustitución. Si la función es suave y tiene la forma pedida, se usa este teorema para tener una notación asintótica
## Conexiones
- [[Funciones suaves]] 
