---
id: 202610041537
fecha: 04-10-2026
estado: completo
tags:
  - Comms
---
# Use Datagram Protocol 
## La idea en una oración
---
> UDP es un protocolo poco confiable que no es orientado a la conexión para el envío de paquetes en la capa de transporte
## Desarrollo
---
***UDP*** es un protocolo que usa el envío de paquetes IP para enviar sus paquetes
Por su naturaleza poco confiable y de no conexión, los paquetes pueden perderse, llegar duplicados o no llegar en orden. Por eso, el servicio que use este protocolo es responsable de verificar sus paquetes, ordenarlos, y solicitar reenvío si se pierde alguno
Su cabecera tiene 4 campos de 16 bits: El puerto origen, que es opcional; el puerto destino, el largo del mensaje UDP y un checksum para verificar que se envía al destinatario correcto
## Conexiones
- [[Pseudo-cabecera de UDP]] 
- [[Multiplexación con puertos en UDP]]