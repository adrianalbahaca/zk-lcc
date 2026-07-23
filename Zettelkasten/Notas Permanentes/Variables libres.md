---
id: 202607101653
fecha: 10-07-2026
estado: completo
tags:
  - Lógica
---
# Conjunto de variables libres
## La idea en una oración
---
> Las variables libres son aquellas tales que no están atadas a ningún cuantificador 
## Desarrollo
---
Debido a la captura de variables libres en una fórmula, una sustitución puede cambiar el significado completo de una fórmula

Entonces, una variable $x$ es *libre* en la fórmula $\phi$ si es que $x$ es una hoja del árbol de parseo tal que no haya camino hacia arriba con un nodo $\forall x$ o $\exists x$. De lo contrario, este elemento está *ligada*

Se puede definir el conjunto de forma recursiva como sigue:
$$
\begin{align*}
	FV : FORM \rightarrow 2^{Var} \\
	
\end{align*}
$$
## Conexiones
- [[]] 
