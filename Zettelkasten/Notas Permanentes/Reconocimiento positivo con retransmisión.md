---
id: 202610051035
fecha: 05-10-2026
estado: completo
tags:
  - Comms
---
# ACK positivo con retransmisión
## La idea en una oración
---
> El reconocimiento positivo con retransmisión implica confirmar con un *ACK* cada paquete recibido
## Desarrollo
---
El problema de garantizar confiabilidad se resuelve usando un mecanismo de *reconocimiento* o *Acknowledgment (ACK)* positivo con retransmisión
Es decir, el receptor envía un ACK al emisor por paquete que envíe, y mantiene la cuenta de los paquetes. También, el emisor usa temporizadores para dar una ventana a la recepción del ACK, y reenviar en caso de que no lo reciba antes de tiempo
Para evitar duplicados, se usa número de secuencia en los paquetes y ACK para evitar duplicados
## Conexiones
- [[Método de ventana deslizante]] 
