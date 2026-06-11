---
id: 202605191552
fecha: 19-05-2026
estado: borrador
tags:
  - SistOpI
---
# Erlang y su propósito 
## La idea en una oración
---
> Erlang es un lenguaje para computación distribuida, poderoso para ejecutar este tipos de tareas
## Desarrollo
---
Erlang es un lenguaje funcional, de tipado dinámico (como Python), definiendo las funciones con recursión y *pattern matching* (como Haskell), que permite hacer programas concurrentes fácilmente, y es usado para hacer computación distribuida

Erlang no posee *transparencia referencial*, el resultado de una función no siempre depende únicamente de sus argumentos

Erlang se basa en dos principios fundamentales:  Concurrencia y fiabilidad. Los procesos que corren tienen ciertas características. Además, permite ejecutar transparentemente en un sistema distribuido

Como referencia, Whatsapp fue programado en Erlang en sus inicios

En Erlang, hay primitivas para mandar mensajes entre dos procesos del programa
## Conexiones
- [[Ejemplo - Enviar y recibir mensaje en Erlang]] 
