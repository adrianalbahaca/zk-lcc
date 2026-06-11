---
id: 202605251702
fecha: 25-05-2026
estado: completo
tags:
  - SistOpI
---
# Productores y consumidores
## La idea en una oración
---
> El problema de los productores y consumidores se refiere al problema cuando una cierta cantidad de productores crean elementos a guardar en un buffer global, de donde los consumidores toman
## Desarrollo
---
Su solución involucra el uso de dos semáforos, uno `libre -> N_BUFFER` y otro `ocupado -> 0` que cuenta la cantidad de espacios libres y ocupados
- Cuando el consumidor quiere consumir algo, hace un `sem_wait(&ocupado)` antes de consumirlo seguramente, y después ejecuta un `sem_post(&libre)`
- El productor ejecuta `sem_wait(&libre)` antes de guardar el elemento en el buffer, y después ejecuta `sem_post(&ocupado)`

El buffer suele ser una *cola circular*, con una cantidad finita de espacio, que tiene que ser protegida con su *mutex* acorde
## Conexiones
- [[Exclusión mutua]]
- [[Cola circular]]
