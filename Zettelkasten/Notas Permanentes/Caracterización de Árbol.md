---
id: 202603092038
fecha: 09-03-2026
estado: borrador
tags:
  - CompMatI
---
# Teorema de caracterización de un árbol
## La idea en una oración
---
> Si el grafo cumple con alguno de las 4 reglas de caracterización, el grafo es un árbol
## Desarrollo
---
Esta propiedad viene de un teorema que dicta:

> Sea $G = (V, E)$ un grafo sin bucles, las siguientes afirmaciones son equivalentes
> 1. $G$ es un árbol
> 2. $G$ es conexo, y borrar cualquiera de sus aristas lo desconecta en 2 subgrafos árboles
> 3. $G$ es acíclico y $|V| = |E| + 1$
> 4. $G$ es conexo y $|V| = |E| + 1$
> 5. $G$ es acíclico, y si $a, b \in V$ y $ab \notin E$, agregarlo al grafo generaría exactamente un ciclo

Su demostración se ve en las hojitas de la profesora. Acá hay unos recordatorios
1. $A \rightarrow B$ : Piensa un grafo árbol y asume que desconectarlo de tal arista fuera conexo. Cuando veas que no sirve, nota que, al ver los vértices que se alcanzan en cada subgrafo, queda un árbol, ya que un ciclo significaría que el grafo del principio no fuera un árbol
2. $B \rightarrow C$ : Si el grafo, contuviera algún ciclo, entonces desconectar una arista haría que siguiera siendo conexo. Luego, como es conexo y acíclico, es un árbol y se cumple la propiedad
3. $C \rightarrow D$ : Siendo acíclico, se suma los vértices de las componentes conexas, para notar que el $r$ se cumple por hipótesis
4. $D \rightarrow E$ : Siendo $G$ conexo con tal suma, si tuviera un ciclo, ya cumpliría con la hipótesis, por lo que se le puede 
5. $E \rightarrow A$ : 
## Conexiones
- [[Árboles]] 
## Fuente / origen de la idea
---
