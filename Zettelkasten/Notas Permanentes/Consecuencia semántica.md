---
id: 202605231958
fecha: 23-05-2026
estado: completo
tags:
  - Lógica
---
# Consecuencia semántica y análisis de la misma 
## La idea en una oración
---
> La consecuencia semántica conecta dos proposiciones sobre una valuación donde si una es cierta, entonces la otra debe ser cierta
## Desarrollo
---
La consecuencia semántica se define formalmente como la relación $\vDash \in P(PROP) \times PROP$ , donde $\Lambda \vDash \phi \iff \forall v, [[\Lambda]]_v = T \Rightarrow [[\phi]]_v = T$ 

Esta relación es esencial en la afirmación de proposiciones, y tiene una relación esencial con $\vdash$, a través del teorema de correctitud y de soundess

Usando esta definición en $PROP$, se descompone como sigue
$$
\begin{align*}
[[p \land q]]_v = T \iff min([[p]]_v, [[q]]_v) = T \\
[[p \lor q]]_v = T \iff max([[p]]_v, [[q]]_v) = T \\
[[p \implies q]]_v = T \iff [[p]]_v \le [[q]]_v \\
[[\neg p]]_v = T \iff [[p]]_v = F
\end{align*}
$$
## Conexiones
- [[Teorema de Soundess]]
- [[Teorema de Correctitud]]
- [[Tautología]]
- [[Contradicción]]
- [[Satisfactibilidad]]
