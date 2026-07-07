---
id: 202605140951
fecha: 14-05-2026
estado: completo
tags:
  - LFyC
---
# Def. de autómata de estado finito determinista
## La idea en una oración
---
> Un autómata de estado finito determinista, o AEFD, es una tupla $A = (S, \Sigma, f, \sigma, Ac)$, donde $S$ es un conjunto finito de estados, $\Sigma$ es el alfabeto donde se define, $f:S\times \Sigma \rightarrow S$ es la función de transición, $\sigma \in \Sigma$ es el estado inicial y $Ac \in S$ es el conjunto finito de estados de aceptación 
## Desarrollo
---
- *Ejemplo*: Siendo el alfabeto $\Sigma = \{ 0,1 \}$, el lenguaje $A = \{w \in \Sigma ^* : |w| = 3\}$ se puede representar como un *AEFD*

Ya que es *determinista*, la función está definida en todo su dominio, por lo que no debe de haber "casos raros". Cosas como palabras que no se aceptan se pueden mandar a un *estado de rechazo*, donde el análisis se atrapa en un loop infinito de un estado que no sea de aceptación. La *función de transición* se puede representar como una tabla

Esta máquina acepta un programa si el análisis de una palabra del lenguaje termina en un estado de aceptación. En este caso, siempre se puede recorrer el camino hasta tal estado ya que es *determinista*, no hay ambigüedades ni tenemos que elegir caminos. Sale automáticamente 

Se puede representar esta máquina de forma gráfica usando un *grafo* con flechas que contengan el símbolo para hacer la transición entre estados, y donde los estados de aceptación se representa con un nodo especial, y el estado inicial contiene una flecha entrante que no venga de ningún nodo del autómata
## Conexiones
- [[Configuración de un AEFD]]
- [[Lenguaje de un autómata finito]]
