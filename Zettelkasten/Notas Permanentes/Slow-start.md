---
id: 202610121114
fecha: 12-10-2026
estado: completo
tags:
  - Comms
---
# Slow-start después de congestión
## La idea en una oración
---
> Una vez la congestión se alivia, se aumenta la ventana de congestión de a un segmento por envío hecho con éxito
## Desarrollo
---
Cuando se detecta que la congestión comienza a reducirse, se aplica un reinicio del flujo normal de datos progresivo. Por cada envío de un paquete exitoso, con ACK recibido, se aumenta la ventana de congestión de a un segmento, para poco a poco retornar la ventana a su estado normal
En caso de que la ventana de congestión se haya reducido hasta la mitad de su valor original, se aumenta de vuelta pero *de a medio datagrama*
Esto permite evitar congestionar la red súbitamente después de un período de congestión o al iniciar una conexión nueva
## Conexiones
- [[]] 
