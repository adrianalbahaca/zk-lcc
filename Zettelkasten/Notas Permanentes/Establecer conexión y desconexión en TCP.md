---
id: 202610131343
fecha: 13-10-2026
estado: completo
tags:
  - Comms
---
# Conexión y desconexión en TCP
## La idea en una oración
---
> La conexión y desconexión en TCP se establece con un *Handshake de 3 pasos* 
## Desarrollo
---
Establecer una conexión con TCP se puede hacer desde ambos extremos o empezando con uno. No hay una dinámica Maestro - Esclavo como la hay en BlueTooth

Al iniciar una conexión, se usa un *handshake* de 3 pasos: Primero, se envía un paquete con el bit `SYN` con un número de secuencia $x$. El receptor envía de respuesta un mensaje `ACK` con el siguiente número de secuencia esperado $x+1$ más otro mensaje `SYN` con el número de secuencia del receptor $y$. Finalmente, se envía un `ACK` del núm. de secuencia $y+1$ y se empieza el envío de datos

Este proceso es similar en el cierre, pero se usa el bit `FIN` y no se envía una respuesta de una vez, ya que puede que sea necesario procesar datos faltantes en parte del receptor antes de continuar. En el reseteo de una conexión, se usa el bit `RST` que no espera al usuario
## Conexiones
- [[BlueTooth]] 
