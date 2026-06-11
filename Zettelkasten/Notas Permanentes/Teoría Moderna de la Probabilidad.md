---
id: 202604181905
fecha: 18-04-2026
estado: completo
tags:
  - PyE
---
# Teoría Moderna de la Probabilidad como generalización 
## La idea en una oración
---
> Sea $\epsilon$ un experimento aleatorio sobre un espacio muestral $S$ correspondiente. $\mathcal{A}$ un conjunto no vacío de subconjuntos de $S$. Entonces $\mathcal{A}$ es una álgebra de subconjuntos de $S$ si cumple las dos reglas fundamentales de pertenencia de $A$ y pertenencia de la unión
## Desarrollo
---
Después de un tiempo, se ha logrado redefinir la frecuencia anterior para que sea sólo un caso particular de algo más grande. Se define como sigue:

*Sea un experimento aleatorio con su espacio muestral correspondiente, sea $\mathcal{A}$ un conjunto no vacío de subconjuntos de $S$, entonces $\mathcal{A}$ será una álgebra del espacio muestral si cumple que:* 
1. $A \in \mathcal{A} \Rightarrow \bar{A} \in \mathcal{A} \forall A \in \mathcal{A}$ 
2. $A_i \in \mathcal{A} \forall i = 1,2,3,...\Rightarrow \cup ^{n} _{i=1} A \in \mathcal{A}$ 

De esta forma, podemos declarar con axiomas a la probabilidad, y tenemos que la *Frecuencia Relativa* es, en realidad, un caso particular de esta definición

*Sea $\epsilon$ un experimento aleatorio con su espacio muestral $S$ correspondiente. Sea $\mathcal{A}$ una álgebra o una $\sigma$-álgebra de subconjuntos de $S$, entonces la probabilidad $P:\mathcal{A} \rightarrow [0,1]$ se define como sigue:*
1. $P(S) = 1$
2. $P(A) \ge 0 \forall A \in \mathcal{A}$
3. $A_i \cap A_j = \emptyset \Rightarrow P(A_i \cup A_j) = P(A_i) + P(A_j)$ 

Note como, en este caso, podemos pensar a $\mathcal{A}$ como subconjuntos finitos para calcular la Frecuencia Relativa
## Conexiones
- [[Def. de una Álgebra]]
- [[Def. de una Sigma-Álgebra]]
- [[Frecuencia Relativa]]
- [[Def. de Suceso en Estadística]]
- [[Def. de Espacio Muestral en Estadística]]
- [[Propiedades de la Probabilidad Moderna]]
- [[Probabilidad condicional]]
