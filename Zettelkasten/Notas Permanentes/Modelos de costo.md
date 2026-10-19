---
id: 202610191248
fecha: 19-10-2026
estado: completo
tags:
  - EDyAII
---
# Modelos de costo 
## La idea en una oración
---
> En la practica, se considerará el *Trabajo* $W$, y la *Profundidad* $S$
## Desarrollo
---
Al analizar un algoritmo, su costo se analizará desde 2 perspectivas:
- **El Trabajo**, anotado como $W$, el cual determina el *costo secuencial* de un programa. Es decir, cuál es el costo de correr el programa en un sólo procesador
- **La Profundidad**, anotado como $S$, el cual determina el *costo paralelo*. Se puede pensar desde varias formas
	- Puede pensarse como la relación de dependencia entre cómputos de un programa, ya que, a mayor dependencia, menos puedes dejar trabajos independientes a los procesadores, por lo cual su profundidad aumenta
	- Puede pensarse como el *costo paralelo* de tener infinitos procesadores a la mano. Aunque imposible, se mira más como la consideración de que *si se necesita un procesador, se tiene uno a la mano*
	- Por último, puede pensarse como la máxima cantidad de cómputo que se hará en una rama del programa
## Conexiones
- [[Relación entre Modelo de Costo y Paralelismo]] 
