---
id: 202605251629
fecha: 25-05-2026
estado: completo
tags:
  - SistOpI
---
# Uso del LightSwitch 
## La idea en una oración
---
> *El primero que entra, prende la luz, y el último que sale, apaga la luz*
## Desarrollo
---
El Light Switch sigue una dinámica de un grupo de personas que entran y salen de una luz, y que tienen que apagar y prender la luz acorde. Se puede definir con una estructura como sigue

```C
typedef struct {
	int contador; // Inicializado en cero
	pthread_mutex_t m; // Inicializar
} LightSwitch;

sem_t emptyRoom;
sem_init(&emptyRoom, 0, 1);
```

Ahora, si tenemos una serie de procesos `A` que pueden acceder a un recurso, donde un proceso `B` sólo puede acceder cuando no haya procesos `A` consumiendo el recurso, el proceso `A` se puede turnar como sigue

```C
// Proceso A consumidor
pthread_mutex_lock(&LightSwitch.m);
LightSwitch.contador ++;
if (LightSwitch.contador == 1)
	sem_wait(&emptyRoom);
pthread_mutex_unlock(&LightSwitch.m);

// Trabajo del proceso A

pthread_mutex_lock(&LightSwitch.m);
LightSwitch.contador --;
if (LightSwitch.contador == 0) 
	sem_post(&emptyRoom);
pthread_mutex_unlock(&LightSwitch.m);
```

```C
// Proceso B productor

sem_wait(&emptyRoom);

// Trabajo del proceso B
```

Nótese que este patrón no evita la inanición del proceso al cual se enfoca. Si se busca algo más estable, se tiene que ir con un estilo de recorrido FIFO
## Conexiones
- [[Exclusión mutua]] 
- [[Problema de los lectores y escritores]]
