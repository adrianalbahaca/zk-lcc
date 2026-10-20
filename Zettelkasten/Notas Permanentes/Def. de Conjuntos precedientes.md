---
id: 202610201846
fecha: 20-10-2026
estado: completo
tags:
  - LFyC
---
# Conjuntos precedientes 
## La idea en una oración
---
> Un conjunto $A$ *precede al* conjunto $B$ $\iff \exists f: A \rightarrow B$ inyectiva. Se escribe como $A \preceq B$ o $|A| \le |B|$ 
## Desarrollo
---
La precedencia de un conjunto se describe con una función inyectiva. Implica que, usando la función, tratar de *acoplar* un conjunto sobre el otro dará que *sobren* elementos a relacionar entre cada uno

Por ejemplo, tenemos como precedentes a $|\mathbb{N}| < |\mathbb{R}|$, y que $\forall A, |A| < \mathcal{P}(A)$ 

>[!tip] Importante
>Note que esta relación es de *orden*. Es reflexiva ($|A| < |A|$ usando la función identidad), es *antisimétrica* (Si $|A| < |B|$, quiere decir que no existe función biyectiva, por lo que $|B| > |A|$), y *transitiva* (Si $|A| < |B|$ y $|B| < |C|$, por composición de funciones inyectivas, $|A| < |C|$) 
## Conexiones
- [[Los naturales no son equipotentes a los reales]]
- [[El conjunto de partes precede al conjunto]]
