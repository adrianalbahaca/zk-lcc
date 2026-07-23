---
id: 202607101620
fecha: 10-07-2026
estado: completo
tags:
  - Lógica
---
# TERM: Conjunto de términos
## La idea en una oración
---
> El conjunto de términos contiene las variables, funciones constantes, y la composición de funciones respectivamente
## Desarrollo
---
El conjunto de términos se define de forma inductiva de la siguiente manera:

Sea $TERM$ el mínimo conjunto tal que:
- $x \in Var \Rightarrow x \in TERM$
- $f \in \mathcal{F} : ar(f)=0 \Rightarrow f \in TERM$
- $x_1, x_2, ... , x_n \in TERM, f \in \mathcal{F} : ar(f) = n > 0 \Rightarrow f(x_1, x_2, ... x_n) \in TERM$

Note que si se cambia el conjunto $\mathcal{F}$, el conjunto $TERM$ también cambia

Puede pensarse el conjunto de términos como el conjunto de las variables y funciones asociados al universo con el que estamos trabajando
## Conexiones
- [[Conjuntos Inductivos]] 
