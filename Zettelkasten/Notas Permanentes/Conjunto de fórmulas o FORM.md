---
id: 202607101647
fecha: 10-07-2026
estado: completo
tags:
  - Lógica
---
# FORM y TERM juntos
## La idea en una oración
---
> Una vez definido $TERM$, lo usamos como base para definir $FORM$
## Desarrollo
---
El conjunto de fórmulas con los conjuntos $(\mathcal{F}, \mathcal{P})$ se define a partir del conjunto de términos apropiado de forma inductiva

Sea $FORM_{(\mathcal{F}, \mathcal{P})}$ el mínimo conjunto tal que:
- $P \in \mathcal{P} : ar(P) \ge 0, t_1, t_2, .. t_n \in TERM_F \Rightarrow P(t_1, t_2, ..., t_n) \in FORM$
- $\phi, \rho \in FORM \Rightarrow \phi \land \rho, \phi \lor \rho, \phi \rightarrow \rho, \neg \phi \in FORM$
- $\phi \in FORM, x \in Var \Rightarrow \forall x \phi, \exists x \phi \in FORM$ 

Recuerda que para definir los conjuntos $\mathcal{P}$ y $\mathcal{F}$ depende de *conocimiento específico de un área*
## Conexiones
- [[Conjuntos Inductivos]]
- [[Variables libres]]
