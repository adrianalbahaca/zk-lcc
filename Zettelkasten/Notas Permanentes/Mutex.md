---
id: 202606282252
fecha: 28-06-2026
estado: completo
tags:
  - SistOpI
---
# Mutex con semáforo 
## La idea en una oración
---
> Imitar un mutex con un semáforo implica inicializarlo con 1
## Desarrollo
---
El semáforo puede ser una alternativa para el mutex de C, simplemente iniciándolo desde cero
```C
sem_t mutex;
sem_init(&mutex, 0, 1);
```

Ahora, un simple post o wait se vuelven las operaciones básicas

```C
sem_wait(&mutex) // -> pthread_mutex_lock(&mutex)
sem_post(&mutex) // -> pthread_mutex_unlock(&mutex)
```

Esta alternativa permite que *como máximo* 1 recurso pueda acceder a una zona crítica
## Conexiones
- [[]] 
