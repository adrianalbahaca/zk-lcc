---
id: 202603271152
fecha: 27-03-2026
estado: completo
tags:
  - CompMatI
---
# Demo. de caract. de circuito euleriano 
## La idea en una oración
---
> Sea $G$ grafo conexo, entonces $G$ tiene un circuito euleriano $\iff$ cada vértice del grafo tiene grado par
## Desarrollo
---
La ida se demuestra de forma directa, mientras que la vuelta construye el circuito euleriano con inducción

> Sea $G$ grafo conexo tal que tiene un circuito euleriano, entonces, por cada vértice que se pasa en el circuito, debe tener una arista de entrada y una arista de salida, y se concluye de allí que su grado debe ser par
> Sea $G$ grafo conexo tal que los grados de los vértices son pares, se hace inducción sobre la cantidad de vértices en el grafo
> - Caso base: Si el grafo tiene un solo vértice de grado par, es trivial que tiene un circuito euleriano
> - Paso inductivo: Sea que todo grafo con $n$ vértices, todos con grado par, contienen un circuito euleriano. Pensando en el $G$ con $n+1$ vértices todos con grado par, al eliminar uno y por H.I, $G-v$ contiene un circuito euleriano. Por lo que, se crea el siguiente circuito entrando y saliendo del circuito anterior por los mismos vértices incidentes a $v$, y esto requiere que tengan grado par

De esta forma, tenemos una caracterización muy fácil para determinar si un grafo tiene circuito euleriano
## Conexiones
- [[]] 
