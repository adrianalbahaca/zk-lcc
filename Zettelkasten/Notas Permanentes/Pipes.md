---
id: 202605031558
fecha: 03-05-2026
estado: completo
tags:
  - SistOpI
---
# Pipes: Ventajas y desventajas
## La idea en una oración
---
> Los pipes son un camino unidireccional entre procesos, para enviar y escribir datos. Práctico de manejar pero no puede mandar elementos de forma unidireccional
## Desarrollo
---
Un *pipe* es un elemento de comunicación entre dos procesos que funciona de forma unidireccional. El extremo 1 es de escritura, mientras que el extremo 0 es de lectura. Es una forma práctica de poder enviar elementos entre procesos
Se puede crear y asignar file descriptors de la siguiente forma:

```
#include <unistd.h>
int fd[2]
pipe(fd)

close(fd[0]) // Cerrar extremo del pipe
dup2(fd[1], STDOUT_FILENO) // Asignar un nuevo file descriptor
```

Los pipes son muy prácticos de usar, permitiendo usar file descriptors para que dos procesos se envíen y reciban elementos, pero suelen ser algo restringidos por ser unidireccionales
Es responsabilidad del programador cerrar los extremos una vez no se usen
## Conexiones
- [[Procesos en Linux]] 
