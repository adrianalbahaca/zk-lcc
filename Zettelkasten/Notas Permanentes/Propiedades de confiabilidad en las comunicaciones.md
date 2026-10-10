---
id: 202610042025
fecha: 04-10-2026
estado: completo
tags:
  - Comms
---
# Propiedades de confiabilidad
## La idea en una oración
---
> Las propiedades de confiabilidad son aquellas que todo protocolo confiable tiene que cumplir para garantizar la llegada adecuada de datos
## Desarrollo
---
Las propiedades se dividen como sigue:
- *Orientación de streams:* Se debe garantizar la llegada ordenada de los bytes o los datos enviados
- *Conexión virtual:* Antes de empezar a enviar datos, se debe solicitar la conexión, que el receptor la reciba, se hagan los ajustes necesarios y se confirme el inicio de envío. Esto también incluye detección de errores
- *Transferencias con buffer:* El protocolo debe poder dividir el paquete a enviar para ajustarlo al buffer eficiente a usar en la red, con una función de push manual
- *Stream sin estructura:* El protocolo no debe depender de la estructura del stream para determinar si es el mensaje correcto. Eso se le deja a manos de la aplicación
- *Conexión full duplex:* Debe garantizar una conexión en ambas direcciones, con la capacidad de pasar a *half duplex* si es necesario, para reducir el tráfico en la red
## Conexiones
- [[]] 
