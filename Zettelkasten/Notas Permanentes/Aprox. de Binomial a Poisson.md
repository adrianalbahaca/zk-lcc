---
id: 202605161830
fecha: 16-05-2026
estado: completo
tags:
  - PyE
---
# De Dist. Binomial a Dist. Poisson 
## La idea en una oración
---
> Si la probabilidad $p$ es muy baja y la cant. de experimentos $n$ es muy grande, hace que si $X \sim Bi(n,p)$ tienda a ser $X \sim Po(\lambda)$, donde $\lambda = np$ 
## Desarrollo
---
Asuma que tengamos una central telefónica, de la cual queremos ver la cantidad de llamadas que se recibe en un intervalo de 180 minutos. Para obtener la probabilidad $p$ y la cant. de llamadas en un intervalo $n$, podemos dividir el intervalo en pedazos más y más pequeños. De esta forma, se ve que $n$ comienza a crecer más y más mientras que $p$ decrece más y más

Se puede demostrar empíricamente que, con $X \sim Bi(n, p)$, tenemos que:
$$
\lim_{n \rightarrow \infty} P(X=k) = {{e^{\lambda}\lambda^k}\over{k!}} \text{ , } \lambda = np \text{ } (p \rightarrow 0)
$$
## Conexiones
- [[]] 
