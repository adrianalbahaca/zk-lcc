---
id: 202603152230
fecha: 15-03-2026
estado: borrador
tags:
  - SistOpI
---
# Qué es un proceso y por qué se divide las cosas en procesos
## La idea en una oración
---
> Un proceso es una entidad abstracta, donde el kernel le designa recursos para ejecutar un programa
## Desarrollo
---
Para poder hacer un programa que haga múltiples cosas a la vez, es necesario dividir la tarea para que se haga cada parte simultáneamente. Discord, por ejemplo, tiene varios procesos para recibir los mensajes, mandarlos, mostrar las cosas lindas en pantalla, y más
Esto se hace a través de *procesos*, dividiendo el programa en entidades abstractas que contienen el algoritmo a ejecutar. Los procesos permiten manejar varias cosas a la vez, gracias a cómo el kernel y el *Scheduler* los programa
## Conexiones
- [[Procesos en Linux]]
- [[Scheduler]]
- [[Concurrencia]]
- [[Cambio de contexto]]
- [[File Descriptor]]
- [[Kernel]]
- [[Padre termina antes que el nene]]
- [[Estados de un proceso]]
- [[Garantías del SO]]