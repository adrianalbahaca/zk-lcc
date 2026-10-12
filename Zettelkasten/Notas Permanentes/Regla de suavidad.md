---
id: 202610121540
fecha: 12-10-2026
estado: completo
tags:
  - EDyAII
---
# Regla de suavidad
## La idea en una oración
---
> Sea $f$ suave, $g$ eventualmente no decreciente y $b \ge 2$, entonces $g(b^k) \in \Theta (f(b^k)) \Rightarrow g(n) \in \Theta (f(n))$ 
## Desarrollo
---
Al cumplir estas 3 condiciones, es posible simplificar los pisos y techos en una recurrencia eligiendo un $n = b^k$ conveniente

Por ejemplo, considere la recurrencia del Merge Sort
$$
W_{sort}(n) = 
\begin{cases}
	c_0 \text{ si } n = 0 \\
	c_1 \text{ si } n = 1 \\
	W_{sort}(\lfloor n/2 \rfloor) + W_{sort}(\lceil n/2 \rceil) + W_{split}(n) + W_{merge}(n) \text{ en otro caso}
\end{cases}
$$
Ahora, considerando $n = 2^k, k \in \mathbb{N}$, podemos simplificar la función como $W_{sort}(n) = 2W_{sort}(n/2) + O(n) \in O(n \log n)$. Luego, como $W_{sort}$ es una función eventualmente no decreciente, demostrable por inducción sobre $n$, podemos determinar que $\forall n \in \mathbb{N}, W_{sort}(n) \in O(n \log n)$ . Esto nos también con la recurrencia final
$$
W(n) = 2W(n/2) + W_{split}(n) + W_{merge}(n)
$$
## Conexiones
- [[]] 
