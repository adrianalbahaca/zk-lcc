---
id: 202610042022
fecha: 04-10-2026
estado: completo
tags:
  - Comms
---
# TCP
## La idea en una oración
---
> TCP es un protocolo confiable orientado a la conexión que garantiza la llegada de datos sin duplicados y en orden
## Desarrollo
---
Debido a la necesidad de un protocolo que sea agnóstico a la forma de detectar duplicados y falta de info. a nivel aplicación, y necesitando un protocolo confiable orientado a la conexión. 

Se crea el protocolo TCP el cual, para cumplir con las propiedades de confiabilidad, usa protocolos de confirmación en las interacciones para verificar que la información llegue completa y en orden, y dando una interfaz en caso de errores para la aplicación

Esta es una ***especificación*** del formato de datos, reconocimiento entre computadoras, los procedimientos para la correcta recepción de datos, recuperación de errores y duplicación y handshake. La *implementación* se deja al programador del sistema operativo. Permite que las apps se comuniquen de forma *concurrente*
## Conexiones
- [[Propiedades de confiabilidad en las comunicaciones]] 
- [[Reconocimiento positivo con retransmisión]]
- [[Especificaciones de un TAD]]
- [[Concurrencia]]
- [[Abstracción de conexión (TCP)]]
- [[Control de flujo y verificación en TCP]]
- [[ACK y retransmisión]]
- [[Timeout y retransmisión]]
- [[Manejo de congestión]]
- [[Datos fuera de banda]]
- [[Establecer conexión y desconexión en TCP]]