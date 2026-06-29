---
id: 202606291026
fecha: 29-06-2026
estado: completo
tags:
  - SistOpI
---
# Problema de los fumadores 
## La idea en una oración
---
> Mientras que un agente suelta dos ingredientes a la mesa, los fumadores que requieren tal combinación los toman para poder fumar. La coordinación no es por semáforos directos, pero sí con agentes proxy
## Desarrollo
---
### Descripción
---
Hay 3 fumadores, cada uno con una cantidad infinita de sólo uno de los ingredientes: Tabaco, papel, o fósforos. Un agente periódicamente dejará dos ingredientes al azar sobre la mesa, para que los fumadores compitan a tomar
### Problema
---
De intentar usar dos semáforos por fumador para indicar que hay un ingrediente de la combinación que necesite en la mesa, esto puede causar un deadlock.
Si el fumador que tiene tabaco toma el papel, y el que tiene papel toma los fósforos, esto ocurriendo a la vez, se quedarían esperando entre sí infinitamente
### Solución
---
Se crean 3 agentes proxy que evalúan cuando hay la combinación de ingredientes que cada fumador necesita, creando 3 semáforos más para cada combinación, y booleanos para indicar los ingredientes en la mesa
## Conexiones
- [[Agentes proxy]] 
