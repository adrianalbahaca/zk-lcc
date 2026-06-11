---
id: 202603192100
fecha: 19-03-2026
estado: completo
tags:
  - SistOpI
---
# Procesos en Linux
## La idea en una oración
---
> Linux tiene una forma más manual de crear, cerrar y trabajar con procesos
## Desarrollo
---
Durante este tema, se va a trabajar con `unistd.h`, una librería que contiene las funciones principales para crear, trabajar con y cerrar procesos
Algo a tomar en cuenta es que Linux tiene una forma... inusual de trabajar con procesos. Mientras que en Windows es más directa, Linux pide mayor cantidad de pasos para trabajar. Esto da más libertad pero hace el proceso un toque más tedioso

```
#include <unistd.h>

int pid = fork() // Divide el proceso en un proceso padre e hijo
getppid() // Obtener PID del padre
getpid() // Obtener PID del proceso en sí 
```

Al invocar tales funciones, el hijo siempre se le asigna el número de proceso `0` dentro del flujo del programa
## Conexiones
- [[Creación y cierre de procesos]]
- [[Ejecución en un proceso]]
- [[Espera en un proceso]]
