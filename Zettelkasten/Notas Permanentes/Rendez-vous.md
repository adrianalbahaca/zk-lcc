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
El *rendez-vous* funciona como una barrera de dos procesos, donde los procesos se avisan entre sí cuando llegan a cierta parte.
En este ejemplo, se va a notificar que el proceso A llega hasta cierto punto donde el proceso B debe continuar

```C
// Inicialización de los semáforos
sem_init(&llegadoA, 0, 0);
sem_init(&llegadoB, 0, 1);
```

```C
// Proceso A

// Primer trabajo de A...

sem_post(&llegadoA); // Avisa que A ha llegado
// Agregar función de aviso o similar
sem_wait(&llegadoB); // Espera a que B llegue

// Segundo trabajo de A
```

```C
// Proceso B

// Primer trabajo de B

sem_post(&llegadoB); // Avisa que B ha llegado
// Agregar función de aviso o similar
sem_wait(&llegadoA); // Espera a que A llegue

// Segundo trabajo de B
```

Esta es la solución clave para resolver el problema de la barbería, en combinación con otras estrategias. Entre cada uno de los semáforos, se puede colocar funciones para indicar que se ha llegado hasta allí
## Conexiones
- [[Problema de la barbería]] 
- [[Barreras]]
