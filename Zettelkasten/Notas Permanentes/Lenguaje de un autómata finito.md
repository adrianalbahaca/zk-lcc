---
id: 202605141029
fecha: 14-05-2026
estado: completo
tags:
  - LFyC
---
# Lenguajes de un autómata finito
## La idea en una oración
---
> Un lenguaje regular es un lenguaje aceptado por un autómata finito $A$. Se define como $L(A) = \{ \alpha \in \Sigma^* : \text{ A acepta } \alpha \}$
## Desarrollo
---
Con una configuración determinada, una palabra será aceptada por un autómata con nombre $A$ $\iff \exists s \in Ac : (\sigma, \alpha) \Rightarrow_A^* (s, \lambda)$

Luego, definimos que el *lenguaje* del autómata $M$, definido como $L(M)$, es el conjunto de las palabras aceptadas por el mismo autómata
## Conexiones
- [[Configuración de un AEFD]] 
