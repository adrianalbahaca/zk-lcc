---
id: 202603092123
fecha: 09-03-2026
estado: borrador | completo
tags:
  - CompMatI
---
# Todo par de vértices en un árbol está conectado con un único camino
## La idea en una oración
---
> En todo árbol, existe único camino entre cualquier par de vértices 
## Desarrollo
---
Su demostración es muy simple:
$\rightarrow$ Asuma que no es así, y que T es un árbol con un par de vértices $u,v$ que tiene dos caminos para llegar entre sí. Ahora, considera los vértices $u',v'$ tales que son los vértices donde ambos caminos empiezan y terminan respectivamente, los cuales pueden ser el par de vértices original. Ahora, con el primer camino $u'-v'$ y el camino $v'-u'$ se tiene un ciclo, pero T es un árbol, lo cual lleva a una contradicción
Por lo tanto, sólo puede haber un camino único entre cada par de vértices
## Conexiones
- [[Árboles]] 
## Fuente / origen de la idea
---
