---
id: 202605031619
fecha: 03-05-2026
estado: completo
tags:
  - SistOpI
---
# `wait`: Espera a un proceso 
## La idea en una oración
---
> `wait` espera a que el proceso hijo finalice
## Desarrollo
---
```
#include <sys/wait.h>
wait(0) // <- espera a que el hijo finalice
``` 

`wait` es un comando esencial para los procesos. Espera a que un hijo finalice su proceso y se retire
## Conexiones
- [[]] 
