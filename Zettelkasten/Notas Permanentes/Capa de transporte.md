---
id: 202610041535
fecha: 04-10-2026
estado: completo
tags:
  - Comms
---
# Capa de transporte
## La idea en una oración
---
> La capa de transporte se encarga de determinar una entrega punto a punto por datagramas o circuitos virtuales, independiente de las redes físicas
## Desarrollo
---
La capa de transporte hace una abstracción entre la capa de aplicación y capa de red, a pesar de que interactúa de forma bastante cercana con la última. Ofrece un servicio de entrega punto a punto, dado en el kernel por bibliotecas de funciones. En otras palabras, funciona como un chequeo extra para verificar que las computadoras del medio no hayan saltado pasos. En TCP/IP, esta comunicación es entre *aplicaciones*

Ahora, debido a la computación paralela, una computadora puede tener múltiples *procesos* o *aplicaciones* por las cuales mandar datos. Por ello, se usa el concepto de *puerto* como una forma de destino abstracto para cada proceso en sí. Mientras que la capa de red se encarga de determinar **A cuál computadora enviar?**, la capa de transporte se encarga de determinar *A cuál proceso de la computadora enviar?*
## Conexiones
- [[UDP o User Datagram Protocol]]
- [[TCP o Transmission Control Protocol]]
