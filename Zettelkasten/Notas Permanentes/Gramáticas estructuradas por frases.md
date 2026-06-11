---
id: 202606051001
fecha: 05-06-2026
estado: borrador | completo | pendiente
tags:
---
# Título de la idea (en forma de afirmación) 
## La idea en una oración
---
> Una gramática estructurada por frases son aquellas donde no hay restricciones sobre las reglas de producción. Es decir, las producciones se pueden ver como $\alpha \rightarrow \delta$ donde $\alpha \in (N \cup T)^*$ y $\delta \in (N \cup T)^*$
## Desarrollo
---
Esta es la gramática más fuerte comparada con las anteriores

Para determinar que una palabra *no* pertenece al lenguaje de una gramática estructurada por frases, se puede buscar en forma de árbol, y podar. Es mucho más complejo determinar si una palabra *si* pertenece

Note que $\lambda \notin (N \cup T)^* - T^*$, por lo que no puede haber reglas como $\lambda \rightarrow \delta$

Ya de acá en adelante, no hay algoritmos que pueda decidir si una palabra pertenece o no a cualquier lenguaje, que es base para demostrar que hay un límite para computar problemas
## Conexiones
- [[]] 
