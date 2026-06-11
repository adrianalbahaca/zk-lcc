---
id: 202603121354
fecha: 12-03-2026
estado: completo
tags:
  - EDyAII
---
# Método de sustitución y sus características
## La idea en una oración
---
> El método de selección involucra intuir algún estilo de cota y demostrarlo con inducción matemática. En caso de intuir un valor incorrecto, el error es informativo, indicando si la estimación es muy ceñida o inferior a lo necesitado 
## Desarrollo
---
A veces, requerimos de analizar el coste o trabajo de un algoritmo recursivo. Para esto, tenemos el *método de sustitución*, el cual es un procedimiento para tantear cuál función puede ser buena para tener una notación asintótica del coste. Sigue los siguientes pasos
1. Determina una función para acotar. Esto puede ser más fácil al usar un árbol de recurrencia
2. Usa inducción para demostrar que cumple con la notación asintótica de la función
3. Determina las constantes para el caso base y el caso inductivo
Es un poco experimental, pero si uno se equivoca en la elección de la función, ese error es informativo
## Conexiones
- [[Árbol de recurrencia]] 
- [[Estimación muy corta para método de sustitución]]
- [[Estimación muy grande para el método de sustitución]]
- [[Principio de Inducción Primitiva]]