---
id: 202605221457
fecha: 22-05-2026
estado: borrador
tags:
  - PyE
---
# Coeficiente de correlación
## La idea en una oración
---
> El coeficiente de correlación nos indica qué tan relacionados están las dos variables aleatorias. Varía en el intervalo $[-1, 1]$
## Desarrollo
---
$$
\rho _{XY} = {{Cov(X,Y)}\over{\sqrt{V(X)V(Y)}}}
$$
En nuestro caso, la *covarianza* para el coeficiente de correlación lineal se define como 
$$
Cov(X,Y) = E(XY)-E(X)E(Y)
$$
Esto es una "varianza" entre la distancia de las dos variables. De por sí sola, la covarianza no nos podría decir mucho, por lo que por eso lo dividimos con la raíz del desvío estándar para relativizarlo

En el caso de que $\rho_{XY} \in \{-1,1\}$, mientras que si $X,Y$ son independientes, $\rho_{XY} = 0$ pero *no vale siempre la inversa*, se puede decir que no hay correlación

Ahora, para esto, se requiere calcular $E(X), E(Y), E(X^2), E(Y^2), E(XY), V(X), V(Y)$, lo cual es un montón. **ATENTI**
## Conexiones
- [[Covarianzas distintas]]  (Posible -> Investigar)
- [[Esperanza y Varianza en vector aleatorio continuo]]
