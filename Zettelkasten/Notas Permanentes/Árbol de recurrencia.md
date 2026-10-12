---
id: 202603212258
fecha: 21-03-2026
estado: completo
tags:
  - EDyAII
---
# Uso del árbol de recurrencia 
## La idea en una oración
---
> El árbol de recurrencia es una herramienta que nos permite visualizar el trabajo hecho o el coste de un algoritmo por cada nivel
## Desarrollo
---
Una forma de determinar cuál función puede ser buena para evaluar notación asintótica de un algoritmo recursivo puede ser ver el resultado del coste al correr el algoritmo en un dato $n$. Para visualizarlo, se usa un *árbol de recurrencia* o un *árbol de recursión*. Permitiendo ver hasta qué nivel termina el algoritmo, y poder tener una sumatoria total del coste del algoritmo

Por ejemplo, considerando la recurrencia $T(n) = 2T({{n}\over{3}}) + cn^2$, cada *nodo* tiene un trabajo de $cn^2$, cada uno tiene $2$ *hijos* y su valor se reduce en ${{n}\over{3}}$ por nivel. Note que la altura del árbol es $\log_3(2)$

![[Pasted image 20261012160248.png]]

Esta estrategia no se usa generalmente para definir cotas, sino para tantear cuál es la más probable antes de verificar con otros métodos
## Conexiones
- [[Método de sustitución]] 
