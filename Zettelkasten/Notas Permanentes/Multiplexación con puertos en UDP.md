---
id: 202610041553
fecha: 04-10-2026
estado: completo
tags:
  - Comms
---
# Cómo se multiplexa con puertos
## La idea en una oración
---
> El mecanismo de puertos es un ejemplo práctico de multiplexación en la capa de transporte
## Desarrollo
---
La capa de transporte con UDP *multiplexa* usando su mecanismo de puertos. Cuando recibe un paquete IP en su cola, revisa si el puerto destino está en uso, para saber si se le da al proceso que lo use o descartar el datagrama si no lo está usando más o si el proceso está muy ocupado. De esta forma, un paquete puede tener la misma dirección IP pero ir a dos procesos distintos

Para asignar puertos a las aplicaciones, se puede tener un estándar central de puertos predeterminados en el sistema o asignarlos dinámicamente. En la práctica, se hace un híbrido entre los dos
## Conexiones
- [[]] 
