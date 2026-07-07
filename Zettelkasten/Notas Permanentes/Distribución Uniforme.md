---
id: 202605131414
fecha: 13-05-2026
estado: borrador
tags:
  - PyE
---
# Def. de dist. uniforme y sus uso
## La idea en una oración
---
> La distribución uniforme se representa como una recta entre los puntos $a, b$, donde en los demás valores fuera de ese intervalo vale cero la función
## Desarrollo
---
$$
f(x) = \begin{cases}
	0 \text{ si } x \notin [a,b] \\
	{{1}\over{b-a}} \text{ si } x \in [a,b]
\end{cases}
$$
$F(x)$ es una recta desde $a$ hasta $b$ tal que su área bajo la recta da 1. En el extremo inferior, la función vale 0, y en el extremo superior la función vale 1
$$
F(x) = \begin{cases}
	0 \text{ si } x < a\\
	{{x-a}\over {b-a}} \text{ si } x \in [a, b]\\
	1 \text{ si } x > b
\end{cases}
$$
Esperanza: $E(X)={{a+b}\over{2}}$ 
Desvío estándar: $V(x)={{(b-a)^2}\over{12}}$ 

## Conexiones
- [[]] 
