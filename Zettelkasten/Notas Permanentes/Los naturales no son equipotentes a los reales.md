---
id: 202603071525
fecha: 07-03-2026
estado: completo
tags:
  - LFyC
---
# Los naturales no son equipotentes a los reales
## La idea en una oración
---
> $\mathbb{N} \nsim \mathbb{R}$ . Es un ejemplo perfecto de demostración usando diagonalización
## Desarrollo
---
 $D/$ Primero, como lema, se ve que $(0, 1) \sim \mathbb{R}$ usando la función arco tangente corrida como $f(n) = {{1}\over{\pi}} \times (\arctan(n) + {{\pi}\over{2}})$
 
 Luego, se supone que existe una función biyectiva $f: \mathbb{N} \rightarrow (0,1)$. Esto quiere decir que necesariamente $f$ tiene que ser sobreyectiva
 
 Para cada $n$, se tiene un número infinito $f(n) = 0,d_{n1} d_{n2} d_{n3} d_{n4}...$, creando una lista de números
 Considere $b = 0,x_1x_2x_3x_4...$ tal que sigue que
 $$ x_i = \begin{cases} 2 & \text{Si } d_{ii} = 1 \\ 1 & \text{Si } d_{ii} \neq 1 \end{cases} $$

Para que este número pertenezca a uno de los valores en $f$, tiene que coincidir en todos sus decimales, pero nota que $b$ diviere de cada $f(k_i)$ en su decimal $i$. Además, debido a la exclusividad en la expansión, no es aceptada en las mismas

Ya que no es posible asignarle un número natural tal que $f(n) = b$, la función no es sobreyectiva, y no sería biyectiva, que por la hipótesis es absurdo 

Por lo tanto: $\mathbb{N} \prec (0,1)$

Finalmente, usando la relación de grado, se concluye que $\mathbb{N} \prec \mathbb{R}$  $\blacksquare$ 
## Conexiones
- [[Cardinalidad]]
- [[Propiedades de equipotencia y precedencia]]
## Fuente / origen de la idea
---
