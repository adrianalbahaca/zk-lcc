---
id: 202607141644
fecha: 14-07-2026
estado: completo
tags:
  - Lógica
---
# Modelos y entornos: Cómo se asocian entre sí 
## La idea en una oración
---
> Sea una signatura $(\mathcal{F}, \mathcal{P})$, un modelo da una serie de elementos y significado a las funciones y predicados de la signatura, mientras que el entorno reemplaza las variables por los valores del entorno
## Desarrollo
---
Formalmente, sea una signatura $(\mathcal{F}, \mathcal{P})$, un modelo $\mathcal{M}$ consiste de
- Un conjunto no vacío de elementos $A$
- Para cada función $f \in \mathcal{F} : ar(f) = 0$, un elemento $f^{\mathcal{M}} \in A$
- Para cada función $f \in \mathcal{F} : ar(f) = n > 0$, otra función $f^{\mathcal{M}} : A^ n \rightarrow A$ 
- Para cada predicado $P \in \mathcal{P} : ar(P) = n > 0$, un conjunto $P^{\mathcal{M}} \subseteq A$. Se puede graficar cada relación con un *grafo dirigido*

Luego, un entorno se puede pensar como una *tabla hash* de variables y valores, pero formalmente es una función $s : Var \rightarrow A^{\mathcal{M}}$ 
## Conexiones
- [[]] 
