---
id: 202605211422
fecha: 21-05-2026
estado: completo
tags:
  - PyE
---
# Dist. de Pascal: Def. y uso
## La idea en una oración
---
> La *distribución de Pascal* modela sobre una variable $X$ definida como la cantidad de intentos del experimento $\epsilon$ hasta obtener una $r$ cantidad de éxitos
## Desarrollo
---
La fórmula que representa $X \sim Pa(r)$ es la siguiente:
$$
P(X=x) = \binom{x-1}{r-1} p^r (1-p)^{x-r}
$$
Esperanza: $E(X) = {{r} \over {p}}$
Desvío estándar: $\sigma(X)={{r(1-p)}\over{p^2}}$ 

Ejemplo: Se puede aplicar esta distribución si se tiene la variable $X$ como *"Cantidad de artículos producidos de forma independiente hasta conseguir 3 elementos defectuosos"*
## Conexiones
- [[]] 
