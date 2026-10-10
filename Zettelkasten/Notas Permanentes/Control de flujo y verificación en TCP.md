---
id: 202610051131
fecha: 05-10-2026
estado: pendiente
tags:
  - Comms
---
# Control de flujo y verif. en TCP 
## La idea en una oración
---
> TCP usa ventanas deslizantes para el envío y recepción de paquetes con tamaño variable acorde al receptor
## Desarrollo
---
TCP tiene control de flujo gracias al buffer dado por la técnica de ventana deslizante que se aplica a nivel octeto. Se usa 3 punteros, donde el primero delimita el lado izq. de la ventana, el segundo delimita los paquetes enviados y a verificar de los no enviados, y el tercero delimita los paquetes que están fuera de la ventana. Cada paquete en la ventana se envía *sin demoras* (<- Preguntar en clase)

Se usa dos ventanas emergentes por conexión para la verificación de llegada de paquetes. También son de *tamaño variable*, acorde a la recepción (<- Preguntar en clase)
## Conexiones
- [[]] 
