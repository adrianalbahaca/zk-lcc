---
id: 202607251725
fecha: 25-07-2026
estado: completo
tags:
  - ArquiComp
---
# Not. científica norm.
## La idea en una oración
---
> La notación científica normalizada permite representar números grandes de forma compacta usando la base y un exponente 
## Desarrollo
---
Siendo $\beta$ la base de número, y $e$ el exponente a usar, un número se anota como notación científica de la siguiente forma
$$
N = (-1)^s \times (a_0.a_{-1}a_{-2}...a_{-n}) \times \beta ^e
$$
Tenemos que $1 \le a_0 \le \beta - 1$ y para los números internos se tiene que $0 \le a_i \le \beta - 1 : i = -1,-2,...$. $s$ se vuelve el *signo*, y $e$ se vuelve el *exponente* de la base
Esta notación tiene ciertas características, en el conjunto $\mathbb{F}(\beta, t, L, U)$:
- La cantidad de elementos en $\mathbb{F}$ es de $2(\beta - 1)\beta ^t(U + L + 1)$
- $\beta^{-t} \le x \le (\beta^1 - \beta^t) \beta^U$
- El conjunto está acotado en ambos lados, y existe 5 regiones que no se llega
	- Se tiene *underflow negativo*, cuando el número negativo es menor que $-x_{min}$
	- Hay *overflow negativo*, cuando el número negativo es mayor que $-x_{max}$
	- No se puede representar el cero
	- Existe el *underflow positivo*, cuando el número positivo es menor que $x_{min}$
	- Está el *overflow positivo*, cuando el número positivo es mayor que $x_{max}$
- Los número se espacian de forma equidistada según el exponente
## Conexiones
- [[Estándar de flotantes IEEE 754]] 
