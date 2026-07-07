---
id: 202603092127
fecha: 09-03-2026
estado: completo
tags:
  - CompMatI
---
# Grafo conexo tiene árbol recubridor, y viceversa
## La idea en una oración
---
> Sea $G=(V,E)$ un grafo no dirigido, $G$ es conexo $\iff$ $G$ tiene un árbol recubridor
## Desarrollo
---
Se demuestra usando una *construcción* del árbol recubridor:

$\Rightarrow )$ Primero, si tenemos un grafo $G$ conexo y resulta que $G$ es un árbol, el árbol recubridor es ese mismo. Sino, $G$ debe contener un ciclo. Se considera el subgrafo $G - e$ tal que rompe el ciclo. Si es un árbol, ese es el árbol generador, y si no, se repite el procedimiento anterior, eliminando todos los ciclos
$\Leftarrow )$ Si $G$ es un árbol recubridor de un grafo, entonces, como es subgrafo, todo par de vértices tiene un camino que los conecte. Por lo tanto, $G$ es conexo

Este teorema es bueno para asegurar conexión a partir de un árbol recubridor
## Conexiones
- [[Árboles]] 
## Fuente / origen de la idea
---
