---
id: 202606031146
fecha: 03-06-2026
estado: completo
tags:
  - SistOpI
---
# Uso del algoritmo de la Panadería 
## La idea en una oración
---
> El Algoritmo de la Panadería de Lamport es una extensión del algoritmo de Peterson a múltiples hilos. Sigue teniendo los problemas del busy waiting y optimizaciones del compilador 
## Desarrollo
---
El *Algoritmo de Lamport de la Panadería* se basa en el sistema de tickets para turnos que ciertas panaderías usan
Su pseudocódigo es como sigue
```C
int turnos[N]; // turnos disponibles para cada hilo
bool esperando[N] // "Clientes que están esperando"
```
## Conexiones
- [[]] 
