---
id: 202606291102
fecha: 29-06-2026
estado: completo
tags:
  - SistOpI
---
# Variables de condición usando semáforos 
## La idea en una oración
---
> Imitar variables de condición con semáforos no es cuestión de sólo usar uno para mantener cuentas de cuántos threads llegan. Se es necesario uno segundo para crear un turnstile
## Desarrollo
---
Para imitar las variables de condición con semáforos, se tiene que implementar un *Rendez-vous* para mantener cuentas de cuántos threads van pasando por el mismo
La estructura se implementa como sigue
```C
typedef struct {
	sem_t condition;
	sem_t leaving;
	int contador;
	pthread_mutex_t m;
} MyCondVar;
```

La operación `pthread_cond_wait(&condVar, &mutex)` usa el Rendez-vous para contabilizar la cantidad de threads que se van yendo de la variable
```C
pthread_mutex_lock(&condVar->m);
condVar->contador++;
pthread_mutex_unlock(&mutex);
pthread_mutex_unlock(&condVar->m);

sem_wait(&condVar->condition); // Se espera a que se cumpla la condición, contando los threads que esperan
sem_post(&condVar->leaving); // Se cuenta cuántos threads en realidad están saliendo, para que no se escape ninguno

pthread_mutex_lock(&mutex);
```

Luego, por ejemplo, para el `pthread_cond_signal(&condVar)`, es cuestión de contabilizar cuántos threads se sueltan y cuántos se tienen que ir

```C
pthread_mutex_lock(&condVar->m);
if (condVar->contador > 0) {
	condVar->contador--;
	sem_post(&condVar->condition); // Se suelta UN thread
	sem_wait(&condVar->leaving); // Se avisa que se va UN thread
}
pthread_mutex_unlock(&condVar->m);
```

`pthread_cond_broadcast(&condVar)` se implementa de forma similar, pero soltando todos los threads y contabilizando cuántos pueden irse en realidad
## Conexiones
- [[]] 
