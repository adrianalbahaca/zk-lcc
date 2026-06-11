---
id: 202604182024
fecha: 18-04-2026
estado: borrador | completo
tags:
---
# Def. de un Socket 
## La idea en una oración
---
> El Socket es un medio de comunicación bidireccional entre procesos. Permite enviar y recibir paquetes a través del SO como en el correo
## Desarrollo
---
En ciertos casos, es necesario que dos procesos se comuniquen entre sí. A pesar de que se puede compartir memoria entre procesos, esto puede ser muy delicado y algo laborioso, por lo que se suele disponer de otras herramientas para enviar paquetes entre procesos

Para esto, una opción es un *Socket*, un elemento similar a un Pipe que envía paquetes de forma bidireccional entre procesos, siendo sus extremos File Descriptors

Comparado con el Pipe, este permite que dos procesos envíen y reciban paquetes entre sí, en vez de forzar que uno envíe paquetes a otro de forma bidireccional

Ahora, hay distintos protocolos, que son el **UDP** y el **TCP**, protocolos distintos para casos distintos
## Conexiones
- [[File Descriptor]]
- [[Protocolo UDP]]
- [[Protocolo TCP]]
- [[Proceso para manejar sockets]]
