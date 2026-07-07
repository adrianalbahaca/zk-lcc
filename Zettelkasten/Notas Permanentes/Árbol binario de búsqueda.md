---
id: "202605131138"
fecha: 13-05-2026
estado: completo
tags:
  - EDyAI
  - EDyAII
---
# Def. y uso de ABB
## La idea en una oración
---
> Un árbol binario de búsqueda es un árbol tal que cada nodo tiene hasta 2 hijos, donde el valor de los elementos en el subárbol izquierdo son menores o iguales al valor de la raíz, y los valores de los elementos en el subárbol derecho son mayores al valor de la raíz
## Desarrollo
---
Si consideras la búsqueda en un arreglo ordenado, puede verse de una forma recursiva. Se ve el elemento de la mediana, luego se va al sub-arreglo izq. o der. dependiendo del tamaño del valor buscado

Esto se puede representar como un *árbol binario de búsqueda*, donde cada nodo tiene un elemento y puede tener hasta dos hijos. Cumple con los siguientes invariantes:
- Cada nodo es una hoja o contiene uno u dos subárboles
- Si $y$ es un elemento del subárbol izquierdo, entonces $y < raíz$
- Si $x$ es un elemento del subárbol derecho, entonces $x > raíz$ 
## Conexiones
- [[Operaciones en ABB]]