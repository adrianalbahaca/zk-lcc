---
id: 202605131443
fecha: 13-05-2026
estado: completo
tags:
  - PyE
---
# Def. y uso de Distribución exponencial
## La idea en una oración
---
> Modela tiempo entre eventos que ocurren de manera aleatoria. Se simboliza como $X~Exp(a)$
## Desarrollo
---
$$
f(x) = \begin{cases}
	ae^{-\alpha x} \text { si } x > 0\\
	0 \text{ en otro caso}
\end{cases}
$$

Ej.: Tiempo hasta que llegue el colectivo en una parada
$$
F(x) = \begin{cases}
	1-e^{-\alpha t} \text{ si } x \ge 0\\
	0 \text { Sino}
\end{cases}
$$
Esperanza: $1\over \alpha$ 
Desvío estándar: ${1} \over {\alpha ^2}$

Cumple con la propiedad de *falta de memoria*, donde no importa donde empiezo, sino que importa donde llegue
$$
P(X > s+t / X > s) = P(X > t)
$$
## Conexiones
- [[Propiedad de falta de memoria]] 
