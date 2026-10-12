---
id: 202610121111
fecha: 12-10-2026
estado: borrador
tags:
  - Comms
---
# PCDM 
## La idea en una oración
---
> Por cada retransmisión, la ventana de congestión se reduce y el temporizados de backoff aumenta
## Desarrollo
---
Si ocurre un caso de retraso donde se tiene que retransmitir un paquete, se reduce la *ventana de congestión* a la mitad y se aumenta el backoff timer de forma exponencial, haciendo esto por cada retransmisión necesaria. La ventana tendrá un mínimo de reducción de 1 segmento
Esto permite adaptar de forma automática el envío de paquetes acorde a las condiciones de la red
## Conexiones
- [[Timeout y retransmisión]] 
