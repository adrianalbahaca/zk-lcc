---
id: 202605142220
fecha: 14-05-2026
estado: borrador
tags:
  - LFyC
---
# Def. de un AEFND
## La idea en una oración
---
> Un AEFND se determina por la tupla $(S, \Sigma, f, \sigma, Ac)$, donde $S$ es el conjunto de los estados, $\Sigma$ es el alfabeto, $f:S \times \Sigma \rightarrow P(S)$ es la función de transición, $\sigma$ es el estado inicial y $Ac$ es el conjunto de estados de aceptación
## Desarrollo
---
Un *autómata de estado finito no determinista*, o *AEFND*, se difiere del AEFD ya que, para cada transición, se retorna un subconjunto de $S$ a donde puede seguirse al siguiente estado. Esto nos dice que, para procesar una palabra y verificar que pertenece a su lenguaje, *se tiene que elegir el camino adecuado para la palabra*
## Conexiones
- [[Relación entre AEFD y AEFND]] 
