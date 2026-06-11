---
id: 202605210816
fecha: 21-05-2026
estado: completo
tags:
  - LFyC
---
# Def. de una gramática regular 
## La idea en una oración
---
> Una gramática regular es una tupla $(N, T, P, \sigma)$ donde se permite que los *no terminales* tengan un símbolo y un no terminal, un símbolo o la cadena vacía $\lambda$
## Desarrollo
---
La tupla que contiene la gramática regular tiene los siguientes elementos:

- $N$: Es un conjunto de *no terminales*
- $\sigma \in N$: Es el terminal inicial
- $T$: Es el conjunto de símbolos *terminales* (o el alfabeto)
- $P$: Es el conjunto de *producciones* de la forma siguiente
	- $S \rightarrow xS' \, S,S' \in N, x \in T$ 
	- $S \rightarrow x, S \in N, x \in T$
	- $S \rightarrow \lambda, S \in N$ 

Cada frase definida en una gramática regular debe empezar con $\sigma$, seguir las reglas en $P$

> Sólo porque pueda definir una gramática de forma no regular, no quiere decir que no sea regular. Similar a cómo si defino una función como $FR$ no quiere decir que no sea $FRP$ 

Se define la *evaluación en un paso* $\Rightarrow$ como $(N \cup T) ^* \times(N \cup T)^*$ . Finalmente, la *clausura reflexiva-transitiva de la evaluación en un paso* $\Rightarrow ^*$ es similar a los autómatas

Finalmente, su lenguaje asociado es $L(G) = \{ w \in T^* : S \Rightarrow ^* w \}$   
## Conexiones
- [[Gramática del lenguaje de Romeo]] 
- [[Expresiones regulares]]
- [[Lenguajes regulares]]