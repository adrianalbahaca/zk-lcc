---
id: 202608201929
fecha: 20-08-2026
estado: borrador
tags:
  - LFyC
---
# Máquinas de Turing 
## La idea en una oración
---
> Las máquinas de Turing se representan por la tupla $(S, \Sigma, \Delta, \delta, \sigma_o, \sigma_f)$ donde $S$ es un conjunto finito de estados, $\Sigma$ es el conjunto de símbolos legibles por la máquina, $\Delta$ son los símbolos de la cinta que incluyen a los de $\Sigma$, $\delta : \Sigma \times S - \{\sigma_f\} \rightarrow \Sigma \times S \times M$, donde $M = \{\leftarrow, \rightarrow, n\}$ es la función de transición, $\sigma_o$ es el estado inicial y $\sigma_f$ es el estado final o "de parada"
## Desarrollo
---
La máquina de Turing se considera la máquina ampliamente aceptada como la que tiene mayor poder de expresividad. Se piensa como una máquina que lee a través de un visor a una cinta de longitud infinita dividida en casillas, y que mantiene un contador de estados
Durante cada transición desde un estado $q$, la máquina lee el símbolo $s$ en la casilla y hace 3 acciones:
- Sustituye o "estampa" el símbolo $s$ con un símbolo nuevo, ya sea otro distinto, $s$ mismo o $\square$, o "blanca"
- Se mueve a la derecha, la izquierda, o se queda quieta en esa casilla
- Cambia a algún estado
La máquina va a continuar desde el estado inicial a seguir los pasos, hasta llegar al estado "de parada", donde allí se detiene. Toma nota de esto, que esto puede indicar que la máquina puede seguir indefinidamente y no parar si está mal dseñada
## Conexiones
- [[Problema de la parada]]
- [[]]
