---
id: 202605210842
fecha: 21-05-2026
estado: borrador
tags:
  - LFyC
---
# Gramática regular $\iff$ AEF 
## La idea en una oración
---
> Sea $L$ un lenguaje sobre un $\Sigma$, entonces $L$ es regular $\iff$ existe $G$ gramática regular tal que $L(G) = L$ 
## Desarrollo
---
Intuitivamente, desde un AEFD $A$ se puede crear una gramática regular $G$ tal que $L(A) = L(G)$, y se puede crear un AEFND de una gramática regular

> Sea $L$ un lenguaje regular, entonces tiene asociado un AEFD $A$. La idea es construir la transición entre cada estado como una producción, finalizando con la cadena vacía en estados finales
> Formalmente, demostramos que $\delta (S, \alpha) = S' \iff S \Rightarrow \alpha S'$ 
> Luego, la vuelta involucra crear tantos estados como no terminales haya, la regla $\lambda$ se hace estado de aceptación, y las transiciones son entre no terminales asociados 
> Puede quedar un AEFND, pero sabemos que los lenguajes entre AEFD y AEFND son iguales, por lo que podemos transformarlo a un AEFD correspondiente $\blacksquare$  
## Conexiones
- [[Lenguaje de un autómata finito]] 
- [[Relación entre AEFD y AEFND]]
- [[Ciclo de autómatas finitos, expresiones y gramáticas regulares.canvas]]
- [[Lema del bombeo en lenguajes regulares]]