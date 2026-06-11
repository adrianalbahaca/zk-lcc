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
> El problema de los lectores y escritores especifica una habitación donde se va a tener libros, donde se tiene que planificar entre los lectores y escritores para leer entre ellos
## Desarrollo
---
Hay tres variantes para este ejercicio
1. La primera variante es *Read-Preferring*, es decir, permitir que más de dos lectores puedan leer los libros, sin que los lectores estén allí, mientras que sólo un escritor puede escribir a la vez en la librería, es decir, sólo un escritor por habitación. Puede ocurrir que pasen lectores sin parar, y no haya espacio para escribir nada
2. La segunda variante da *Write-Preferring*, permitiendo varios escritores que escriban en la librería, mientras que sólo es posible haber un lector en la habitación a la vez. Puede ocurrir que pasen puros escritores a escribir, y no haya lectores a leer los libros
3. Finalmente, se tiene la variante *No-Starve*, donde no se da prioridad a ninguno de los dos

Estas invariantes usan el *Light Switch para hacer los cambios pedidos*
## Conexiones
- [[Light Switch]]
- [[Semáforos]]
