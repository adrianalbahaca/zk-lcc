---
id: 202606282232
fecha: 28-06-2026
estado: completo
tags:
  - SistOpI
---
# Cola FIFO para el recorrido de procesos
## La idea en una oración
---
> *Cada proceso se atiende por su orden de llegada*
## Desarrollo
---
Se forma una cola de semáforos para denotar el orden de los recursos que van entrando. Cada proceso tiene su semáforo, y no comparten uno

```C
typedef struct Sem_Nodo{
	sem_t sem;
	struct Sem_Nodo* sig;
} Sem_Nodo

typedef struct {
	Sem_Nodo head;
	Sem_Nodo tail;
} Sem_Cola;

sem_t mutex_estado;
```

Asumiendo funciones clásicas para encolar y desencolar, cada proceso tiene lo siguiente:

```C
// Proceso X. Considere `cola` como una cola global thread-safe que se puede usar entre nodos
sem_wait(&mutex_estado);

Sem_Nodo s = sem_nodo_create(0); // Se inicia un nodo con estado inicial 0

sem_nodo_enqueue(&cola, &s);
if ((t = sem_nodo_peek(&cola)) == s && recurso_disponible(&c))
	sem_post(&s.s);
sem_post(&mutex_estado);

sem_wait(&s.s);

// Trabajo del proceso X

sem_wait(&mutex_estado);
sem_nodo_dequeue(&c, &s.s); // Sacar el semáforo de la cola
if (!sem_nodo_empty(&c))
	&sem_post(&primer_sem_cola);
sem_post(&mutex_estado);
```

Esta solución es una de las alternativas para la versión justa del problema de los lectores y escritores
## Conexiones
- [[Problema de los lectores y escritores]] 
