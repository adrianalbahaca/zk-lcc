---
id: 202603172215
fecha: 17-03-2026
estado: completo
tags:
  - CompMatI
---
# El grafo $K_5$ no es planar
## La idea en una oración
---
> El grafo $K_5$ no es planar. No tiene ninguna inmersión planar. Es uno de los grafos no planares minimales
## Desarrollo
---
Curiosamente, hay grafos pequeños de los cuales es imposible tener una inmersión planar, como lo es el $K_5$

> Vamos a *reducir al absurdo*. Sea $K_5$, tiene los vértices $\{v_1, v_2, v_3, v_4, v_5\}$
> Se arma un ciclo con $v_1, v_2, v_3$, y luego se trata de considerar qué pasa con los otros dos vértices
> - Si $v_4$ está adentro del ciclo, entonces $v_5$ tiene que quedar afuera, por lo que los cruces van a ser inevitables. Si $v_5$ está adentro de alguna de las caras internas, se va a tener que cruzar una arista para poder conectar las del ciclo
> - Si $v_4$ está afuera, entonces, alguno de los vértices del ciclo va a quedar adentro otra vez. Ocurren problemas similares con en punto anterior
> Por estos motivos, es imposible hacer una inmersión planar del grafo, por lo que $K_5$ no es planar

Cada uno de sus subgrafos puede ser planar, ya que nos sacamos la molestia del quinto vértice en adelante
Además, por este mismo motivo, se puede considerar $K_5$ como un *grafo planar minimal*, del cual podemos usar para verificar si otros grafos son no planares
## Conexiones
- [[Reducción al absurdo]] 
