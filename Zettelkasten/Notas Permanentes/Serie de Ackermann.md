---
id: 202604240818
fecha: 24-04-2026
estado: completo
tags:
  - LFyC
---
# Def. de Serie de Ackermann 
## La idea en una oración
---
> La Serie de Ackermann es una serie total y computable, pero que es muy explosiva. De acá parte la prueba del límite de las FRP
## Desarrollo
---
Tiene como ley lo siguiente:
$$
\begin{align}
	f_0:\mathbb{N} \rightarrow \mathbb{N}, f_0(x) = s(x) \\
	f_{k+1}:\mathbb{N} \rightarrow \mathbb{N}, f_{k+1}(x) = f_k^{x+2}(x)
\end{align}
$$
Esta cosa es muy explosiva, dando números muy grandes con números pequeños
Estas funciones en las series tienen las siguientes propiedades: 
- $\forall k, f_k \in FRP$
- $\forall k, x, x', x > x' \Rightarrow f_k(x)>f_k(x')$
- $\forall k, f_k(x)>x$ 
- $\forall k, \forall x, f_{k+1}(x)>f_k(x)$ 
## Conexiones
- [[Cada función de Ackermann en FRP]]
- [[Propiedades de las funciones de Serie de Ackermann]]
