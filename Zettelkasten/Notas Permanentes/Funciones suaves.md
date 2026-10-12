---
id: 202603232152
fecha: 23-03-2026
estado: borrador
tags:
  - EDyAII
---
# Def. de funciones suaves y usos
## La idea en una oración
---
>Una función es suave si es *b-suave* para todo $b \in \mathbb{N}$
## Desarrollo
---
Para definir una función suave, se es necesario definir una función *b-suave*

> Una función $f: \mathbb{N} \rightarrow \mathbb{R}^+$ es *b-suave* si $f$ es eventualmente no decreciente y $f(bn) \in O(f(n))$

Esto nos indica que la función no crece de forma explosiva. De multiplicarse por $b$, la salida sólo se multiplica por una constante a lo sumo

Para determinar la suavidad de una función, se usa el lema siguiente

> Si $f$ es b-suave para $b \le 2$, entonces es suave
> 
> $D/$ Suponga una función b-suave con $b \le 2$. Entonces es eventualmente no decreciente y $f(bn) \in O(f(n))$. En otras palabras, $\exists n_0 \in \mathbb{N}, c \in \mathbb{R}^+$ tal que $\forall n \ge n_0, f(bn) \le cf(n)$. Si se elige una constante tal que $k \le b$, tenemos que $f(kn) \le f(bn) \le cf(n)$, por lo que también cumple que $f(kn) \in O(f(n))$. Si $k > b$, se elige $m = min\{ j \in \mathbb{N}, b^j \ge k \}$, luego para $n$ suficientemente grande $f(kn) \le f(b^m n) \le f(b(b^{m-1} n)) \le cf(b^{m-1}n) ... \le k^m f(n)$, concluyendo que $f(kn) \in O(f(n))$. Como cumple para todo $k$, se determina que $f$ es suave $\blacksquare$
## Conexiones
- [[Funciones eventualmente no decrecientes]]
- [[Regla de suavidad]]
- [[Teorema Maestro]]
