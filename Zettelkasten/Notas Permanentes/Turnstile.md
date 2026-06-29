---
id: 202606282216
fecha: 28-06-2026
estado: completo
tags:
  - SistOpI
---
# Turnstile o Molinete 
## La idea en una oración
---
> *Como un molinete en un metro, sólo uno puede pasar a la vez*
> *Como un molinete con ticket. Sólo puede pasar uno con el ticket a la vez*
## Desarrollo
---
El Turnstile es una estructura muy sencilla y que parece redundante en un principio. Su patrón se ve así

```C
sem_t turnstile;
sem_init(&turnstile, 0, 1);
```

```C
// Checkpoint del proceso N

sem_wait(&turnstile);
sem_post(&turnstile);
```

Este patrón también nos permite darle prioridad a cierto proceso usando otro elemento en el medio

```C
// Checkpoint del proceso X
sem_wait(&turnstile);
sem_wait(&esperarRecurso); // Se aplica alguna condición
sem_post(&turnstile);
```

Este patrón se usa en varias soluciones a varios problemas de semáforos
## Conexiones
- [[]] 
