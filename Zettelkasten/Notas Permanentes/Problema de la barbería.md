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
Para este problema, se tiene el barbero y el cliente
- El barbero se duerme mientras no haya clientes en las sillas
- Si llega uno, se despierta y lo atiende, cortándole el pelo y cobrándole acorde
- El cliente toma asiento en la silla si el barbero está ocupado
- Si no hay espacio disponible, el cliente se va

La solución a este problema puede ser usando un mutex y, o unos *rendez-vous* usando semáforos, o una *barrera de 2 procesos* para el cliente y el barbero
## Conexiones
- [[Rendez-vous]] 
