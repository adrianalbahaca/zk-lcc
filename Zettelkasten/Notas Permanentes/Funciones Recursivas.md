---
id: 202604240814
fecha: 24-04-2026
estado: borrador
tags:
  - LFyC
---
# Def. de las FR
## La idea en una oración
---
> Una función es FR si se puede construir con funciones FR y con operadores $\phi$, $R$ y $M$ 
## Desarrollo
---
Ya que no es posible representar todas las funciones computables con FRP, se le agrega otro operador: El *Minimizador*

Dada $f^{(n+1)}$, se define $g^{(n)} = M[f^{(n)}]$, donde para $X \in \mathbb{N} \rightarrow g^{(n)}=M_t(f(t, X)=0)$ 

Este operador permite definir funciones parciales sin tener que ir a casos raros como en FRP, y también puede representar a la función de Ackermann
## Conexiones
- [[La función ACK no es FRP]]
- [[La función ACK es FR]]
