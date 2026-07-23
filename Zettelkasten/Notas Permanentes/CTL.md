---
id: 202607151840
fecha: 15-07-2026
estado: completo
tags:
  - Lógica
---
# CTL: Lógica de árbol computacional 
## La idea en una oración
---
> CTL toma el tiempo como un árbol que se desenvuelve en ramas, considerando que el futuro no es determinado o lineal
## Desarrollo
---
CTL es una rama de lógica temporal que nos permite analizar el tiempo como un árbol infinito con ramas que se extienden. Se considera que el tiempo no es algo determinado, y cada estado del modelo es un punto en el tiempo donde se cumplen ciertas propiedades. Cada camino es una posibilidad, donde el camino 'actual' es alguno de los que están en el árbol

Tiene los operadores siguientes:
- $\mathcal{M}, s \vDash \forall \bigcirc \psi: \text{Cada sucesor de s cumple } \psi$
- $\mathcal{M}, s \vDash \exists \bigcirc \psi: \text{Algún sucesor de s cumple } \psi$
- $\mathcal{M}, s \vDash \forall [\phi \mathbb{U} \psi]: \text{Para cada traza que empieza con s, existe i} \in \mathbb{N} \text{ tal que } \mathcal{M} ,s_i \vDash \psi, \mathcal{M}, s_k \vDash \phi (k < i)$
- $\mathcal{M}, s \vDash \exists [\phi \mathbb{U} \psi]: \text{Hay una traza que empiece con s tal que haya i} \in \mathbb{N} \text{ tal que } \mathcal{M}, s_i \vDash \psi, \mathcal{M}, s_k \vDash \phi (k < i)$
- $\mathcal{M}, s \vDash \forall \diamond \psi = \forall [\phi \mathbb{U} \psi]$
- $\mathcal{M}, s \vDash \exists \diamond \psi = \exists [\phi \mathbb{U} \psi]$
- $\mathcal{M}, s \vDash \forall \square \psi = \neg \exists \diamond \neg \psi$
- $\mathcal{M}, s \vDash \exists \square \psi = \neg \forall \diamond \neg \psi$
## Conexiones
- [[Algoritmo SAT]] 
- [[Concurrencia]]
