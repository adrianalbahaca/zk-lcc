---
id: 202609211257
fecha: 21-09-2026
estado: borrador
tags:
  - Comms
---
# NRZI 
## La idea en una oración
---
> En este caso, cualquier transición se considera el bit 1 mientras que ninguna transición se considera el bit 0
## Desarrollo
---
El NRZI se combina con algún estilo de compactación de bits para poder evitar largas tramas de bits iguales. En nuestro caso, NRZI se combina con *4B/5B*, asegurando que haya transiciones en cada bit 1 y que se controle la cantidad de 0's seguidos
## Conexiones
- [[4B-5B]] 
