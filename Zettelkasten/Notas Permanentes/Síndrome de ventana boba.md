---
id: 202610151054
fecha: 15-10-2026
estado: borrador
tags:
  - Comms
---
# Síndrome de ventana boba: Causante y prevención
## La idea en una oración
---
> El Síndrome ocurre cuando hay una diferencia notable entre las ventanas de las computadoras, haciendo que el envío termine degradándose a un envío de paquetes muy chicos
## Desarrollo
---
El *Sindrome de ventana tonta* ocurre cuando las ventanas entre las computadoras en sí son de tamaños desiguales. Entre cada `ACK` que envía de vuelta la computadora con la ventana más chica, avisa del poco espacio disponible en la misma, haciendo que el emisor envíe paquetes cuya relación entre el tamaño del header a de los datos sea grande **(Se termina consumiendo más bando de ancha mandando el header que los datos!)**

Para evitar esto, se implementa mecanismos entre receptor y emisor:
- El receptor mantiene un récord de la ventana disponible y retrasa el aviso de aumento de ventana hasta que sea *significante*, o sea hasta que el buffer tenga *suficiente* espacio libre, esto último significando algo distinto entre sistemas. TCP lo estandaría como `min((tam_buffer)/2, max_tam_segmento)`
  Esto reduce el tráfico en la red permite piggy back en el segmento, pero si el retraso es muy grande puede causar retransmiciones accidentales, confundiendo el estimado para el temporizador del backoff
- El emisor espera acumular la cantidad de datos *suficientes* según el rendimiento de la red (**Self-clocking**)
## Conexiones
- [[]] 
