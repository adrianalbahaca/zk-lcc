---
id: 202610091818
fecha: 09-10-2026
estado: completo
tags:
  - Comms
---
# ACK y retransmisión
## La idea en una oración
---
> Debido a que los datos tienen tamaño variable, el ACK se hace sobre el prefijo contiguo más largo recibido, mandando el siguiente número de secuencia que se espera
## Desarrollo
---
Como los datos a enviar son de largo variable y pueden haber retransmitidos extra, no es posible hacer un ACK exclusivamente sobre segmentos o datagramas, ya que no sabemos cómo se divide. Por ello, el paquete se arma en orden usando el *número de secuencia* y el ACK se hace por *el prefijo contiguo más largo recibido*, enviando el siguiente número de secuencia que se espera
Es cumulativo, por lo que es fácil de generar e inambiguo, y si se pierde un ACK no quiere decir que se solicitará retransmisión ya que el emisor recibe feedback constante de otras transmisiones de datos, pero no se envía info de transmisiones exitosas en sí, sólo su posición en el stream, y en caso de timeouts, o se tiene que reenviar todo o se reenvía los pedazos faltantes, ambos ineficientes
## Conexiones
- [[]] 
