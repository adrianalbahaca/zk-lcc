---
id: 202606291244
fecha: 29-06-2026
estado: completo
tags:
---
# Mesa vs. Hoare
## La idea en una oración
---
> La semántica de Hoare le da inmediatamente el control apenas se cumple la condición una vez, mientras que la semántica de Mesa le da el control si y sólo si la condición se mantiene
## Desarrollo
---
Al tener una variable de condición o un monitor, se tiene dos maneras de liberar el proceso que está esperando. Estas semánticas se definen como de Hoare o de Mesa

En la semántica de Hoare, se cumple:
- El control se le otorga al hilo esperando la condición inmediatamente cuando se cumple
- El hilo que hace `signal()` cede su control al hilo que estaba esperando
- Se tiene que asegurar que la condición se siga cumpliendo para la ejecución del hilo esperando
Aunque su accionar es más rápido, es más complejo de implementar. Además, por su misma definición, se implementa con un *if*:
```C
if (!condicion)
	pthread_cond_wait(&condC, &mutex)
```

En la semántica de Mesa, se cumple:
- El hilo que invoca `signal()` sigue ejecutándose
- El hilo esperando la condición tiene que esperar a su turno antes de ejecutarse
A pesar de que esto puede causar latencia entre hilos, es más predecible y se suele implementar en los sistemas modernos
```C
while (!condicion)
	pthread_cond_wait(&condC, &mutex);
```
## Conexiones
- [[Monitor de Mesa]]
- [[Monitor de Hoare]]
