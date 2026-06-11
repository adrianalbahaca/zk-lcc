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
> El *Light Switch* es un *Mutex* y contador combinados que sigue la dinámica de cuando se prende y se apaga una luz en un cuarto
## Desarrollo
---
El Light Switch se puede representar como la siguiente estructura:
```C
typedef struct {
	int contador; // Inicializado en cero
	pthread_mutex_t m; // Inicializar
} LightSwitch;
```

La idea es similar a cómo se tiene que tratar un bombillo con un grupo de personas. La primera persona en entrar prende el bombillo y deja que el resto pase a la habitación. La última persona en salir apaga el bombillo, indicando que el espacio está vacío
## Conexiones
- [[Exclusión mutua]] 
- [[Problema de los lectores y escritores]]
