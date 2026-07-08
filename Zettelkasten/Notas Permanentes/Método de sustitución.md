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
Una vez se tenga la intuición de una cota asintótica para la recurrencia, se puede resolver usando el *método de sustitución*. Implica usar recursión para determinar que tal cota es adecuada para la recurrencia dada. Se aplica de la siguiente manera
1. Determina una función para acotar. Esto puede ser más fácil al usar un árbol de recurrencia
2. Inicia el caso inductivo, con hipótesis inductiva fuerte. Donde $\forall m < n$, se cumple la cota. Determina las constantes que afirmen esto
3. Finalmente, considere el caso base, buscando las constantes que afirmen la cota
Es un poco experimental. En caso de no tener resolución directa, se puede usar tal parada como elemento
## Conexiones
- [[Árbol de recurrencia]] 
- [[Estimación muy corta para método de sustitución]]
- [[Estimación muy grande para el método de sustitución]]
- [[Principio de Inducción Primitiva]]