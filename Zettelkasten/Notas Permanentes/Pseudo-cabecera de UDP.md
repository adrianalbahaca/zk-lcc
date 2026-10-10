---
id: 202610041541
fecha: 04-10-2026
estado: completo
tags:
  - Comms
---
# Pseudo-cabecera de UDP 
## La idea en una oración
---
> La pseudo-cabecera computa el checksum sobre el mismo añadido al datagrama. Puede mezclarse entre capas
## Desarrollo
---
Para verificar que un paquete llegue al destinatario correcto, se agrega una *pseudo-cabecera* que computa una verificación del destino correcto
Esta contiene 4 campos: La IP de origen, la IP de destino, ceros para alinearlo con 16 bits, el código de protocolo IP (Siendo 17 para UDP), y el largo del paquete UDP
Note que esto causa que la barrera entre capas se difumine un poco, ya que sería necesario que la capa de UDP interactúe con la capa de IP para obtener estos datos. Es un ejemplo práctico de cómo difuminar ciertas fronteras por practicidad
## Conexiones
- [[]] 
