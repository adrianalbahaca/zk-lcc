---
id: 202604092210
fecha: 09-04-2026
estado: borrador
tags:
  - Lógica
---
# Formalización de $PROP$
## La idea en una oración
---
> $PROP$ se define como un conjunto inductivo sobre proposiciones atómicas y operadores como $\vee, \wedge, \rightarrow, \neg$ sobre tales proposiciones atómicas. Es como una gramática libre de contexto 
## Desarrollo
---
Este conjunto sería el mínimo tal que cumple con las siguientes reglas

1. $p_i \in X, i \in \mathbb{N}$ 
2. $\bot \in X$ 
3. $\phi , \varphi \in X$, entonces $\phi \vee \varphi, \phi \wedge \varphi, \phi \rightarrow \varphi \in X$ 
4. $\phi \in X$, entonces $\neg \phi \in X$ 

Ahora, esto, por más que trate de ser un alfabeto, no lo es tanto. Es un *conjunto inductivo*, con su propio $PIP$ y todo, del cual se va a usar para demostrar varias propiedades de este conjunto
## Conexiones
- [[Conjuntos Inductivos]]
- [[Valuación sobre PROP]]
