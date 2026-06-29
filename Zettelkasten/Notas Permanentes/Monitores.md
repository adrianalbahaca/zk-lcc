---
id: 202605041312
fecha: 04-05-2026
estado: borrador | completo
tags:
  - SistOpI
---
#   
## La idea en una oración
---
> Un monitor es una estructura de sincronización para evitar race conditions en hilos. Permiten a los hilos renunciar a un mutex momentáneamente
## Desarrollo
---
El monitor es un *TAD* abstracto que sirve como caja negra para definir operaciones con exclusión mutua sobre datos compartidos. Todo proceso que quiera operar sobre los datos compartidos debe de hacerlo a través del monitor. Los datos locales del monitor sólo pueden ser operados por las funciones locales del mismo, y provee exclusión mutua a las funciones definidas incluso si no las tiene por predeterminado
## Conexiones
- [[Variables de condición]] 
- [[Monitor de Mesa]]
- [[Monitor de Hoare]]
