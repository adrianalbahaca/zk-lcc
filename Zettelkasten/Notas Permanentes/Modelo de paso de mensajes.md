---
id: 202605191401
fecha: 19-05-2026
estado: completo
tags:
  - SistOpI
---
# Título de la idea (en forma de afirmación) 
## La idea en una oración
---
> Ya que los procesos no comparten memoria, tenemos un *proceso emisor*, un *proceso receptor* y un *mensaje* a compartir
## Desarrollo
---
Con este modelo, podemos pensar en la sincronización entre el emisor y el receptor

Si es *Sincrónico*, el emisor se bloquea hasta que el receptor acepte el mensaje y el receptor se bloquea hasta recibir el mensaje

Si es *Asincrónico*, se manda el mensaje y se continúa con el proceso. Si llega, joya, pero sino, bueno. Se suele usar un buffer para almacenar los mensajes
## Conexiones
- [[]] 
