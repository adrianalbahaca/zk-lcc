---
id: 202606291240
fecha: 29-06-2026
estado: completo
tags:
  - SistOpI
---
# Computación paralela y OMP 
## La idea en una oración
---
> La computación paralela es una dinámica donde cada proceso comparte una memoria, y se ejecutan de forma independiente
## Desarrollo
---
En la computación paralela, varios procesos se ejecutan con una memoria compartida, usada para intercambiarse información entre sí

Ya que los conflictos entre memoria pueden ser comunes, se suele usar librerías como lo son `omp.h`, que usan una estrategia de *Fork-Join*, en una región del programa, se aplica el uso de múltiples hilos para ejecutar un código, y después se retorna el control al hilo maestro
## Conexiones
- [[]] 
