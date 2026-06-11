---
id: 202605212205
fecha: 21-05-2026
estado: completo
tags:
  - SistOpI
---
# Barrera de 2 procesos con semáforos $\rightarrow$ rendez-vous 
## La idea en una oración
---
> El rendez-vous es una barrera de dos procesos implementado con banderas. Es una pieza esencial para el problema de la barbería
## Desarrollo
---
El uso clásico de un *rendez-vous* viene para el problema de la barbería. Si se tiene las banderas `cliente, barbero, cliente_listo, barbero_listo` inicializadas en cero, para el barbero y cliente se aplica:

```C

// Chequear clientes

sem_post(&cliente);
sem_wait(&barbero);

// Hacer operaciones

sem_post(&cliente_listo);
sem_wait(&barbero_listo);

// Chequear clientes
```

De esta forma, el hilo A tiene que esperar al hilo B hasta que termine, y viceversa
## Conexiones
- [[Problema de la barbería]] 
- [[Barreras]]
