---
id: 202608051746
fecha: 05-08-2026
estado: completo
tags:
  - ArquiComp
---
# Cómo acceder a memoria en ARM y operar sobre elementos 
## La idea en una oración
---
> Ya que no es posible acceder a memoria directamente con instrucciones, se debe cargar valores primero, operar sobre ellos, y después guardarlos en memoria
## Desarrollo
---
Debido a la falta de acceso a memoria directa que tiene la arquitectura *Load/Store*, obligando a que las operaciones sean sólo sobre registros, es necesario primero cargar los valores y después guardarlos
- `ldr` para registros, o `vldr` para registros del VFP, permite cargar al registro desde una dirección a memoria
- `str` para registros, o `vstr` para registros del VFP, copia el valor del registro a la dirección a memoria dada
Las formas comunes para dar direcciones son `[r_]`, `[r_, num] (r_ + num`, `[r_, num]! (Copia valor r_ + num a r_)`

Luego de cargar, las operaciones comunes, como `add`, `sub`, `mul`, `umull` pueden ser aplicadas a gusto, para después guardar en memoria
## Conexiones
- [[]] 
