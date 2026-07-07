---
id: 202605041314
fecha: 04-05-2026
estado: completo
tags:
  - SistOpI
---
# Var. de condición para Hilos
## La idea en una oración
---
> Una variable de condición permite frenar hilos hasta que se cumpla una cierta condición
## Desarrollo
---
Una variable de condición bloquea el transcurso de los hilos hasta que se llegue a una cierta condición preestablecida. Se basa en dos operaciones, que son el `wait`, donde se espera a que se mande la señal para desbloquear el mutex dado, y el `signal`, donde se envía la señal a *uno* de los hilos que están esperando. Si se quiere enviar la señal a *todos* los threads esperando, se usa `broadcast`

Esto permite el evitar el *busy waiting*, bloqueando a nivel del sistema sin problemas

Es especialmente útil en el *Problema de productor - consumidor* o en el *Thread Pool*

Proceso de uso:
`Mutex -> while() -> cond_wait(&cond, &mutex) -> Región crítica -> unlock -> Signal de chequeo` <- Ya que nada me garantiza de que se cumpla (Semántica de Mesa)

Lógica usada: **Lógica de Mesa**, pero también se puede pensar como Lógica de Hoare
## Conexiones
- [[Lógica de Hoare]] 
- [[Ejemplo: Thread Pool y epoll para servidor]]
