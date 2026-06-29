---
id: 202606282258
fecha: 28-06-2026
estado: completo
tags:
  - SistOpI
---
# Multiplex: Mutex para varios procesos
## La idea en una oración
---
> Región crítica para hasta N procesos
## Desarrollo
---
Usando la idea del semáforo como mutex, se puede expandir inicializandolo con un número mayor a 1

```C
sem_t multiplex;
sem_init(&multiplex, 0, N);
```

Ahora, esto permite que *como máximo* N procesos estén en la misma región crítica a la vez
## Conexiones
- [[]] 
