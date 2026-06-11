---
id: 202603071552
fecha: 07-03-2026
estado: borrador | completo
tags:
  - LFyC
---
# Título de la idea (en forma de afirmación) 
## La idea en una oración
---
> Para todo conjunto $A$, se tiene que $A \prec \mathcal{P}(A)$ 
## Desarrollo
---
Si tenemos el conjunto de partes de un conjunto infinito $A$, tenemos como función $f: A \rightarrow \mathcal{P}(A)$ inyectiva con ley $f(x) = \{x\}$ 
Luego, asumamos que hay alguna función sobreyectiva $g: \mathcal{P}(A) \rightarrow A$, tal que para cada subconjunto de $A$, los llamaremos $X$, existe algún elemento $a \in A$ tal que $g(a) = X$ 
Ahora, nos hacemos una pregunta inocente: **Para todo $X$, $a \in X$?**
Vamos a definir $y = \{ x \in A \mid x \notin g(x)\}$
Si $g(y) = X$, entonces $x \notin X$, pero si $f(x) \neq y$, entonces $x \in X$... Esto crea un absurdo
Por lo tanto, no existe ninguna función sobreyectiva y $\mathbb{N} \prec \mathbb{R}$ 
Esto nos permite determinar que existe infinitos infinitos, metiendo cada conjunto por partes y determinando su conjunto de partes una y otra vez
## Conexiones
- [[Existen infinitos infinitos]] 
- [[Cardinalidad]]
## Fuente / origen de la idea
---
