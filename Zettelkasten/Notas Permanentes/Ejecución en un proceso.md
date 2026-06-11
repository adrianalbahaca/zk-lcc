---
id: 202603192103
fecha: 19-03-2026
estado: borrador
tags:
  - SistOpI
---
# `exec()` y ejecución de instrucciones
## La idea en una oración
---
> `exec()` se usa para cambiar todas las instrucciones de un proceso, empezando las instrucciones de cero
## Desarrollo
---
```
#include <unistd.h>

exec(char* pathname, char** argv)
```

Una vez dividido los procesos, se puede usar el comando `exec(camino_al_archivo, argumentos)` que recibe la dirección de dónde están las instrucciones para reemplazar el proceso actual y los argumentos a llevar para `argc` y `argv`
## Conexiones
- [[]] 
