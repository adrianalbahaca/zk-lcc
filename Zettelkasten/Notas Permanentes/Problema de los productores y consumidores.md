---
id: 202605251702
fecha: 25-05-2026
estado: completo
tags:
  - SistOpI
---
# Productores y consumidores
## La idea en una oración
---
> Una $M$ cantidad de productores crean recursos, mientras que una $N$ cantidad de consumidores los usa. Se sincronizan entre sí usando variables de condición o semáforos
## Desarrollo
---
En este problema, tenemos $M$ productores que crean recursos a guardar en un buffer y $N$ consumidores que usan los recursos creados. Este buffer se comparte entre los productores y consumidores de forma concurrente

Si asumimos que el buffer se define como una estructura de datos finita, como una *Cola circular*, tenemos dos soluciones

- **Con semáforos:** Se crea dos semáforos, ambos miden la cantidad de espacios disponibles u ocupados que hay en el buffer

```C
sem_t espacios_libres, espacios_ocupados;
sem_init(&espacios_libres, 0, N); // Siendo N la cantidad de espacios en el buffer
sem_init(&espacios_ocupados, 0, 0);
```

```C
// En el productor...
sem_wait(&espacios_libres);

// Producir recurso e insertarlo

sem_post(&espacios_ocupados);
```

```C
// En el consumidor
sem_wait(&espacios_ocupados);

// Consumir recurso

sem_post(&espacios_libres);
```

- **Con variables de condición:** Se crea dos variables de condición y un mutex, donde las variables evalúan el estado del buffer acorde

```C
pthread_cond_t no_lleno, no_vacio;
pthread_mutex_t m;
```

```C
// En el productor
pthread_mutex_lock(&m);
while (buffer_lleno)
	pthread_cond_wait(&no_lleno, &m);

// Producir recurso

pthread_cond_signal(&no_vacio);
pthread_mutex_unlock(&m);
```

```C
// En el consumidor
pthread_mutex_lock(&m);
while(buffer_vacio)
	pthread_cond_wait(&no_vacio, &m);

// Consumir recurso

pthread_cond_signal(&no_lleno);
pthread_mutex_unlock(&m);
```

Nótese como, en los semáforos, se mide la *cantidad de espacios*, ya sean ocupados o libres, mientras que, en las variables de condición, se evalúa *el estado actual del buffer*, si no está lleno o no está vacío
## Conexiones
- [[Exclusión mutua]]
- [[Cola circular]]
- [[Multiplex]]
