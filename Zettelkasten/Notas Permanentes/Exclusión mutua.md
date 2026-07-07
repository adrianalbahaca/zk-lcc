---
id: 202605112148
fecha: 11-05-2026
estado: completo
tags:
  - SistOpI
---
# Problema de la Exclusión Mutua
## La idea en una oración
---
> El problema de la exclusión mutua consiste en garantizar que, a lo sumo, sólo un proceso pueda acceder a la región crítica de un código
## Desarrollo
---
Para asegurar sincronización entre elementos, se deriva al *problema de la exclusión mutua*. Nuestro objetivo es garantizar que sólo un proceso u hilo pueda acceder a la sección crítica de un código

Por ejemplo, si tenemos una pila compartida entre varios hilos, se puede tratar de restringir el uso de los comandos `push`, `pop` o `peek` a un solo hilo a la vez, parando los hilos cuando traten de hacer tales instrucciones si es que hay un hilo ejecutándolo 
## Conexiones
- [[Objetos concurrentes]]
- [[Exclusión mutua en C]]
