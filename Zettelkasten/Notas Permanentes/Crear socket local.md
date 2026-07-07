---
id: 202605031802
fecha: 03-05-2026
estado: borrador | completo
tags:
---
# `socketpair`: Creación de sockets locales sin tanto ajuste
## La idea en una oración
---
> `socketpair` es una función que crea dos sockets locales para que dos procesos se puedan comunicar entre sí de forma bidireccional
## Desarrollo
---
Los pipes son útiles como avenida de comunicación entre dos procesos, pero tiene la desventaja de que es unidireccional, por lo que dos procesos no podrán hablarse entre sí ida y vuelta

Si ambos procesos tienen una relación de paternidad entre sí, se puede usar esta función para crear sockets anónimos entre ellos, retornados en un arreglo de enteros de tamaño par

```C
#include <sys/socket.h>

int socket(int dominio, int tipo, int protocolo, int sockets[2]);
// Devuelve el estado de la operación y recibe el dominio a usar, su tipo, y el protocolo, además de un arreglo de enteros para los file descriptors a usar como sockets
```
## Conexiones
- [[Pipes]] 
