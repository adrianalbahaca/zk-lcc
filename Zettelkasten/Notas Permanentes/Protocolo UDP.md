---
id: 202604182033
fecha: 18-04-2026
estado: completo
tags:
  - SistOpI
---
# UDP y casos de uso 
## La idea en una oración
---
> UDP es un protocolo que envía paquetes sin establecer una conexión estable, tal que cada paquete se tiene que enviar a una cierta dirección. Esta forma carga menos la red y es veloz, pero se pueden perder datos y no hay orden de llegada
## Desarrollo
---
La transmisión de video en vivo es un proceso que puede estresar bastante la red, ya que se tiene que enviar un montón de paquetes de un solo coñazo entre los servidores de Twitch y los espectadores. Para esto, se suele usar el protocolo UDP

Este protocolo no aplica una conexión estable antes de enviar los paquetes. Ahora, esto permite cargar menos la red y hace el envío de paquetes mucho más veloz, pero causa que se puedan perder paquetes en el camino, y no admite orden de llegada. Hasta hay veces que puede llegar el mismo paquete dos veces o más repetidos. Sólo se hace en Best Effort Basis
## Conexiones
- [[]] 
