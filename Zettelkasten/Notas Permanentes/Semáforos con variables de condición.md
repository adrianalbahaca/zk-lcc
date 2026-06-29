---
id: 202606291115
fecha: 29-06-2026
estado: completo
tags:
  - SistOpI
---
# Imitar un semáforo usando variables de condición
## La idea en una oración
---
> La variable de condición medirá el estado donde el semáforo llegue a cero, y no soltará threads hasta que el contador interno no supere el margen de cero
## Desarrollo
---
Debido a lo general que es una variable de condición, se puede medir directamente el estado del contador, para indicar cuando se libera un thread
La estructura se implementa como sigue
```C
typedef struct {
	pthread_cond_t condition;
	int contador;
	pthread_mutex_t m;
} MySem;
```

Al inicializar con un contador en $N$, las operaciones `wait` y `post` se vuelven simples

```C
// Para sem_wait
pthread_mutex_lock(&mySem->m);
mySem->contador++;
pthread_cond_signal(&mySem->condition);
pthread_mutex_unlock(&mySem->m);
```

```C
// Para sem_post
pthread_mutex_lock(&mySem->m);
while (mySem->contador <= 0)
	pthread_cond_wait(&mySem->condition, &mySem->m);

mySem->contador--;
pthread_mutex_unlock(&mySem->m);
```
## Conexiones
- [[]] 
