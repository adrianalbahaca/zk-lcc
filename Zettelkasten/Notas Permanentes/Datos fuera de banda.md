---
id: 202610121207
fecha: 12-10-2026
estado: borrador
tags:
  - Comms
---
# Señales y datos fuera de banda
## La idea en una oración
---
> En caso de enviar datos fuera de la banda del datagrama, se usa el bit `URG` para activar el modo urgente
## Desarrollo
---
Los datos fuera de banda son aquellos tales que son aparte del datagrama a enviar. Cosas como señales a enviar, por ejemplo `Ctrl-C`
En esos casos, se usa el bit `URG` de urgente más el terreno del puntero de `URGENT`. En el receptor, se detiene recepción de datagramas y se activa el *modo urgente*, sólo recibiendo aquellos datagramas con el bit de `URG` activos. Una vez se maneja todos los datagramas urgente, se retorna al *modo normal*
## Conexiones
- [[]] 
