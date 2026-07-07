---
id: 202603121351
fecha: 12-03-2026
estado: borrador
tags:
  - EDyAII
---
# En qué se basa el Modelo de costo
## La idea en una oración
---
> El modelo de costo se basa en la cantidad de procesadores a usar en un algoritmo. Denotamos $W$ el costo de hacer el trabajo con un procesador, o el *costo secuencial*, y $S$ el costo de hacer el trabajo con infinitos procesadores, o el *costo paralelo*
## Desarrollo
---
El modelo de costo será una herramienta que vamos a usar para medir la eficiencia de algoritmos en situaciones particulares, en nuestro caso, cuando trabajemos con un procesador o con varios procesadores. Estos casos se denotan como **Costo secuencial** ($W$) y **Costo paralelo** ($S$, de *span*) respectivamente
Para poder calcular estos costos, se diseña un pseudo-lenguaje, similar a Haskell, con las siguientes definiciones:
$$
$$

## Conexiones
- [[Costo secuencial]]
- [[Costo paralelo]]
- [[Notación Asintótica]]
## Fuente / origen de la idea
---
