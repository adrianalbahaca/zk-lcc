---
id: 202605251641
fecha: 25-05-2026
estado: completo
tags:
  - SistOpI
---
# Lectores y Escritores 
## La idea en una oración
---
> El problema de los lectores y escritores especifica una habitación donde se va a tener libros, donde se tiene que planificar entre los lectores y escritores para evitar que se crucen entre sí
## Desarrollo
---
### Descripción
---
Hay una habitación donde van a haber libros a presentar y escribir. $N$ lectores y $M$ escritores tienen que turnarse para leer y escribir en el cuarto compartido. Ningún escritor puede escribir mientras haya lectores. Aunque pueden haber varios lectores a la vez en la habitación, sólo puede haber un escritor a la vez
### Problema
---
Cómo se turna múltiples consumidores en un buffer, con los productores uno a uno, para que sigan estas reglas?
### Solución
---
Hay 3 soluciones a este problema, donde involucran Light Switches, Turnstiles, y recorridos FIFO
- **Preferencia a los lectores:**
  En los lectores, se coordina un *Light Switch* para que el primer lector que pase tome un mutex, avisando que el cuarto no está vacío, y el último lo suelte, para avisar que el cuarto está vacía. Cada escritor sólo tomará y soltará este mutex mientras escribe como siempre
- **Preferencia a los escritores:**
  Manteniendo la misma estructura de antes, se implementa un *Turnstile* en lectores y escritores, donde el escritor tiene que pasar en un *Turnstile* con el mutex del cuarto vacío en el medio
- **Nula preferencia:**
  Se usa variables de condición para indicar el estatuto del cuarto. Los lectores usan esta variable y esperan mientras *haya un escritor activo o hayan escritores esperando*, avisando cuando ya no haya lectores en la habitación con un booleano. Cada escritor espera mientras *haya lectores activos o haya un escritor activo*, manteniendo la cuenta de los escritores esperando, y avisando a los lectores cuando salga un escritor
## Conexiones
- [[Light Switch]]
- [[Turnstile]]
- [[Recorrido FIFO]]
