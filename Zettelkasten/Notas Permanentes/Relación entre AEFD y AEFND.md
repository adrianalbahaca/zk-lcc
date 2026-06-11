---
id: 202605142226
fecha: 14-05-2026
estado: completo
tags:
  - LFyC
---
# AEFD y AEFND 
## La idea en una oración
---
>  Los AEFD y AEFND están relacionados entre sí, y pueden representar los mismo lenguajes
## Desarrollo
---
Un AEFD es un caso especial de un AEFND, donde, para que una palabra sea aceptada, *sólo existe un camino desde el estado inicial a un estado de aceptación*, mientras que en un AEFND *existen uno u más caminos*

Además, un lenguaje que pueda ser verificado con un AEFND también puede ser verificado por un AEFD. Esto quiere decir que se puede transformar un AEFND en un AEFD para un mismo lenguaje. El proceso consiste en armar un AEFD con estados que sean conjuntos de estados

Recuerda que $\delta(P, w)=\cup _{q en P} \delta(q, w)$. O sea, unimos todos los estados en un conjunto mientras procesamos la cadena

> Sea M = ($S,\Sigma,\delta,\sigma,F$) AEFND, se crea un AEFD nuevo $M'=(S',\Sigma,\delta',\sigma',F')$, donde $S'=P(S)$, $F$ es todo subconjunto de estados de $M$ que contenga un estado inicial, $\sigma'=\{ \sigma \}$ y $\delta'([p_1, p_2,...p_k], a) = [q_1, q_2,...,q_n] \iff \delta(\{ p_1, p_2, ..., p_k\}, a) = \{q_1, q_2,..., q_n\}$   
> 
> Luego, se tiene que demostrar, por inducción sobre el largo de la cadena, que $\delta'(\sigma', w) = [q_1,q_2,...,q_k] \iff \delta(\sigma,w) = \{ q_1, q_2, ..., q_k \}$, haciendo la unión consecutiva de los estados en $\delta$ mientras se procesa $w$. 
> 
> Finalmente, para concluir, se menciona que $\delta'(\sigma', w)$ termina en $F'$ exactamente cuando $\delta(\sigma, w)$ contenga un estado de aceptación. Así se concluye que $L(M) = L(M')$  $\blacksquare$ 
## Conexiones
- [[Autómatas de estado finito determinista]] 
- [[Autómata de estado finito no determinista]]
- [[Círculo de lenguajes regulares y autómatas finitos]]