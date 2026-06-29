---
id: 202605251727
fecha: 25-05-2026
estado: completo
tags:
  - SistOpI
---
# Problema de la barbería
## La idea en una oración
---
> El problema de la barbería consiste en un barbero con una serie de sillas donde los clientes pueden esperar. Se tiene que coordinar el corte y pago entre barbero y cliente 
## Desarrollo
---
### Descripción
---
Hay un barbero dormilón con una sala de espera con $N$ sillas. Si no hay nadie a quien atender, se duerme. Si un cliente entra y ve que el barbero está dormido, lo despierta para pedirle un corte de cabello. Si el barbero está cortando el pelo, y hay espacio para que espere, toma una silla y se sienta, pero sino, se va
### Problema
---
Coordinar entre el barbero y los clientes es una tarea que sólo un semáforo no puede cumplir. Se es necesario un patrón específico
### Solución
---
Se usan 2 *Rendez-vous*. Uno para avisar que llega un cliente y que despierta al barbero, y otro para avisar que el cliente y el barbero están listos
- El primero coordina entre cuando hay un cliente y cuando el barbero está despierto
- El segundo coordina entre cuando el barbero termina de atender un cliente y cuando el cliente termina de pagar
Se puede añadir un mutex con un contador para contar la cantidad de clientes que hay y avisar cuando la sala de espera esté llena
## Conexiones
- [[Rendez-vous]] 
