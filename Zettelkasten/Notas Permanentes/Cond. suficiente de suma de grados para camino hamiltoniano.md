---
id: 202603261410
fecha: 26-03-2026
estado: completo
tags:
  - CompMatI
---
# Suma entre grados de vértices y caminos hamiltonianos
## La idea en una oración
---
> Sea $G$ grafo simple, tal que $|V(G)|=n \ge 2$ y $gr(v)+gr(w)\ge n-1, \forall v,w \in V(G)$, entonces $G$ contiene un camino hamiltoniano
## Desarrollo
---
Esta prueba tiene dos partes: Verifica si el grafo es conexo con contradicción y después construye el camino maximal, evitando los ciclos

> Para construir el ciclo, se tiene que tomar el camino $P$ maximal en el grafo, y demostrar que está contenido en un ciclo
> Primero, su extremo sólo puede estar a vértices del camino, ya que, de no ser así, $P$ no sería máximo
> Luego, se ve que debe existir por lo menos una arista de un extremo a un vértice $v_t$ en el camino, y otra arista del extremo opuesto al vértice $v_{t-1}$. De no ser así, la sumatoria de los grados crearía una contradicción con la suma de los grados en la hipótesis
> Con esto, se toma el vértice con el camino más corto posible desde el vértice a $P$ y se rearma, repitiendo este proceso hasta que el camino tenga todos los vértices
## Conexiones
- [[]] 
