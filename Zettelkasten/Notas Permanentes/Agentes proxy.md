---
id: 202606282223
fecha: 28-06-2026
estado: completo
tags:
  - SistOpI
---
# Agentes proxy para detectar recursos 
## La idea en una oración
---
> *Usa un supervisor extra para detectar ciertas condiciones*
## Desarrollo
---
Los semáforos no están diseñados para recordar o seguir estados, por lo que, para casos donde esperamos ciertas condiciones, es posible que se necesite un agente externo que permita medir cuando las condiciones estén

Asuma que cada proceso necesita dos recursos cada uno `A`, `B` y `C`. El agente que vigila el recurso `A` puede supervisar si también está el `B` o el `C`

```C
bool hayRecursoA = false, hayRecursoB = false, hayRecursoC = false;

sem_t recursoA, recursoB, recursoC;
sem_t recursoAyB, recursoAyC, recursoByC;
sem_t mutex_estado
```

```C
// Agente A. Vigila recurso A y lo matchea con recurso B y C
while (true) {
	sem_wait(&recursoA);
	
	sem_wait(&mutex_estado);
	if (recursoB) {
		recursoB = false;
		sem_post(&recursoAyB);
	}
	else if (recursoC) {
		recursoC = false;
		sem_post(&recursoAyC);
	}
	else
		recursoA = true;
	sem_post(&mutex_estado);
}
```

Esta es la pieza esencial para resolver el problema de los fumadores
## Conexiones
- [[Problema de los fumadores]] 
