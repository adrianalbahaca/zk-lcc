---
id: 202603192048
fecha: 19-03-2026
estado: completo
tags:
  - SistOpI
---
# Aplicación del cambio de contexto
## La idea en una oración
---
> El *cambio de contexto* ocurre cuando es necesario guardar el estado de un proceso para continuar con otro. Esta parte es fundamental para dar la ilusión de simultaneidad en las computadoras
## Desarrollo
---
Aunque parezca que la computadora está haciendo todo a la vez, en realidad, está *cambiando de contexto* entre cada proceso de forma efectiva, pausando un proceso y guardando su estado como sus registros, memoria y pila en el PCB para continuar con otro proceso
A pesar de que esto es costoso para algo que no es útil a simple vista, permite dar la ilusión de que todo lo que ocurre en una compu es a la vez
Estos cambios de contexto ocurren por alguna señal enviada, por alguna planificación del CPU, porque se cambia entre modos usuario/kernel o llega una tarea de alta prioridad que el *Scheduler* necesita ejecutar
## Conexiones
- [[Scheduler]] 
