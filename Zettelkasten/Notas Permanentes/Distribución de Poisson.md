---
id: 202605161813
fecha: 16-05-2026
estado: completo
tags:
  - PyE
---
# Dist. de Poisson: Casos de uso y def
## La idea en una oración
---
> La distribución de Poisson es el modelo para la variable aleatoria discreta que representa *la probabilidad de que ocurra $n$ veces el evento $A$ en un intervalo* (usualmente de tiempo u espacio)
## Desarrollo
---
Si la variable $X$ sigue una distribución de Poisson con $\lambda > 0$, se representa como $X \sim Po(\lambda)$ y tiene la siguiente fórmula
$$
P(X=k) = {{e^{-\lambda}\lambda^{k}}\over{k!}} \text{ , } k=0,1,2,...,n
$$
Usualmente, se suele usar esta fórmula para representar eventos *poco probables*

Esperanza: $E(X) = \lambda$
Variancia: $V(X) = \lambda$ 

Ejemplo: Si consideramos la cant. de clientes que entra en un negocio cada 2 minutos, podemos definirlo con esta distribución, si tenemos que $\lambda = r$ 
## Conexiones
- [[Aprox. de Binomial a Poisson]] 
