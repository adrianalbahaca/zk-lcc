---
id: 202605161750
fecha: 16-05-2026
estado: completo
tags:
  - PyE
---
# Dist. Binomial: Casos de uso y def.
## La idea en una oración
---
> La distribución binomial ocurre en aquellas variables aleatorias discretas que sean *la cantidad de veces que ocurre el suceso A en las $n$ repeticiones del experimento $\epsilon$*
## Desarrollo
---
La fórmula que denota una variable $X \sim Bi(n,p)$ es la siguiente:
$$
P(X=x) = \binom{n}{x}p^x(1-p)^{n-x} \text{ , } k = 0,1,...,n
$$

Por ejemplo, considere una fábrica donde se tiene productos que pueden ser *defectuosos* ($D$) o *no defectuosos* ($N$), de los cuales se saca una muestra de 3 productos. Si las probabilidades que un producto sea defectuoso es independiente de los demás, podemos representar este modelo con esta distribución

Esperanza: $E(X) = np$
Variancia: $V(X) = np(1-p)$ 

*Ejemplo:* Ej.6 de la práctica 3, con $X$ siendo "número total de artículos defectuosos en una muestra de 3 productos con construcción independiente"

Una variación de esto es cuando la muestra sea de 1 elemento, siendo la *distribución de Bernoulli*
## Conexiones
- [[Distribución de Bernoulli]] 
