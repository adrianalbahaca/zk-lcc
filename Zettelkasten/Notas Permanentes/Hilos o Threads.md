---
id: 202604240957
fecha: 24-04-2026
estado: completo
tags:
  - SistOpI
---
# Hilos: Programación multi-tarea 
## La idea en una oración
---
> Los *hilos* o *threads* son subprocesos en un proceso, que se pueden ejecutar en múltiples procesadores del CPU en la computadora. Suelen ser mejores que la memoria compartida pero está sujeta al *race condition*
## Desarrollo
---
A pesar de que la programación congruente con procesos ha sido uno de los conceptos que ha revolucionado la computación, debido a que los procesos son independientes por los requisitos del SO, suele dificultarse el compartir datos de forma segura y libre entre procesos

Para ese caso, programar con *hilos* o *threads* suele ser una mejor alternativa

En síntesis, es una tarea que puede ser ejecutada al mismo tiempo que otra tarea a través del uso de múltiples procesadores del CPU y/o con un manejo eficiente del Scheduler, saltando entre tareas

Es mucho mejor que compartir memoria entre procesos, y suele ser más seguro que ello, pero suele aparecer el problema del *race condition*, un problema que suele ser demasiado difícil de percatarse por la sutileza del problema
## Conexiones
- [[Procesos vs. Hilos]]
- [[Race Condition y su manejo]]
- [[Ejemplo del uso de threads en un servidor]]
- [[Exclusión mutua]]
- [[Operación atómica]]
- [[Procesamiento asíncrono]]
- [[Ejemplo: Thread Pool y epoll para servidor]]
- [[Hilos en C]]
- [[Variables de condición]]
- [[Ejemplo de uso - OpenMP]]
