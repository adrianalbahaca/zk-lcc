---
id: 202605031741
fecha: 03-05-2026
estado: borrador | completo
tags:
---
# Paso a paso del manejo de un socket
## La idea en una oración
---
> Para el socket de escucha, se crea, luego *se le da un nombre*, y se pone a la escucha. Para el socket de recepción, se acepta y se le envía instrucciones
## Desarrollo
---
La creación de dos sockets para dos procesos que no están relacionados localmente requiere de un cierto paso a paso acorde a unas funciones dedicadas para ello

```C
#include <sys/socket.h>

// -> Primero, se crea el socket de escucha
int listen_sock = socket(AF_INET, SOCK_STREAM, 0)
// Ej. de socket con dominio IPv4, tipo TCP protocolo auto.

// -> Luego, se le "da un nombre", dandole el puerto por el que va a recibir la señar, cómo es el protocolo y qué dirección recibir
struct sockaddr_in sa;
sa.sin_famili = AF_INET;
sa.sin_port = htons(4040);
sa.sin_addr.s_addr = htonl(INADDR_ANY);
// Ej: Recibe en IPv4, por el puerto 4040, cualquier dirección

// Finalmente, se coloca el socket en modo escucha
rc = listen(listen_sock, 10);
// Ej. se queda escuchando el socket y se hace una cola de hasta 10 conexiones

// -> Para el socket de escucha, se acepta la conexión
int connect_sock = accept(listen_sock, NULL, NULL);
// Ej. Se acepta una conexión sin configuración a darle

// -> Finalmente, se puede aplicar las operaciones dadas
// -> Se tiene que cerrar ambas conexiones después
close(connect_sock);
close(listen_sock);
```
## Conexiones
- [[Crear socket local]] 
