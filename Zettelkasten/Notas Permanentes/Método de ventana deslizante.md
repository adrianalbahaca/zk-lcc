---
id: 202610051039
fecha: 05-10-2026
estado: completo
tags:
  - Comms
---
# Sliding Window para envío simultáneo 
## La idea en una oración
---
> Para usar todo el ancho de banda y no perder tiempo con cada ACK, se usa una *ventana* de paquetes a enviar que se desliza mientras recibe cada ACK
## Desarrollo
---
Usando el sistema de ACK positivo puro, se pierde demasiado tiempo y se desperdicia mucho ancho de banda el estar esperando por cada ACK individual para enviar el siguiente paquete
Por ello, se diseña una *ventana* de paquetes que se envía, donde esta ventana se *desliza* con cada ACK que recibe para enviar el siguiente paquete. Esto restringe los reenvíos necesarios a los paquetes en la ventana, donde cada paquete sigue manteniendo sus timers individuales
De esta forma, se satura el ancho de banda con paquetes acorde al tamaño de la ventana a usar, aprovechándolo mucho más 
## Conexiones
- [[]] 
