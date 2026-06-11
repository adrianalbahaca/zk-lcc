---
id: 202605041345
fecha: 04-05-2026
estado: borrador
tags:
  - SistOpI
---
# OpenMP: Azúcar sintáctica
## La idea en una oración
---
> OpenMP es una librería que buscará paralelizar todo acorde. Si no es posible, como es agnóstico, puede compilar y correr las cosas en single-thread
## Desarrollo
---
Variables globales compartidas entre threads, y variables explícitamente privadas
`#pragma omp parallel private(x) // <- Variable privada`
Master thread: ID = 0

*(Hacer notas de la librería a usar)*
## Conexiones
- [[]] 
