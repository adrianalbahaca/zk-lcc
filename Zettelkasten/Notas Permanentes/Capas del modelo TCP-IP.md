---
id: 202609031449
fecha: 03-09-2026
estado: borrador
tags:
  - Comms
---
# Capas del modelo TCP/IP y sus funciones 
## La idea en una oración
---
> El modelo TCP/IP tiene 4 capas: La capa de enlace, la capa de interred, la capa de transporte y la capa de aplicación
## Desarrollo
---
Basándose en las necesidades del *DoD*, se crearon 4 capas en este modelo:
1. ***Capa de enlace:*** Esta capa se definió como una red de conmutación de paquetes basado en una capa sin conexión. Se le piensa más como una *interfaz*
2. ***Capa de interred:*** Se encarga de que el host pueda inyectar paquetes a la interred y que cada paquete pueda viajar de forma independiente hacia el destino dado. Pueden que lleguen en desorden, por lo que se encarga de organizarlos cuando llegan. El formato de paquete se define por el *IP* con *ICMP*
3. ***Capa de transporte:*** Permite la comunicación entre pares como en el modelo OSI. Se tiene el protocolo *TCP*, confiable orientado a la conexión usando mensajes discretos para enviar y un ensamblaje de mensaje al llegar, y control de flujo integrado, o el *UDP*, no confiable sin control de flujo ni asignación de secuencia, dejando esa carga a los pares
4. ***Capa de aplicación:*** Acá están los protocolos de alto nivel, como *TELNET*, *FTP*, *SMTP*, *HTTP*, *DNS* y *RTP*
## Conexiones
- [[HTTP]]
- [[DNS]]
