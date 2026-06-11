---
id: 202605251201
fecha: 25-05-2026
estado: completo
tags:
  - SistOpI
---
# Semáforos vs. Variables de condición
## La idea en una oración
---
> Los semáforos se piensan en *recursos disponibles* mientras que las variables de condición se piensan en *estados del programa* 
## Desarrollo
---
Considerando el *problema de los productores y consumidores*, nos muestra dos lados de los semáforos y las variables de condición
- Los semáforos se enfocan en la *cantidad de recurso disponible*, y deja que los hilos compitan por ellos. Es más pragmático, pero no deja la condición por la cual se frena el programa de forma explícita. Por ejemplo, para el problema mencionado, se tiene dos semáforos que contabas cuántos espacios habían libres y cuántos estaban ocupados, dejando que los hilos compartan entre ellos
- Las variables de condición se enfocan en *el estado del programa en sí*, turnando los hilos cuando cambien los estados. Es más binario y muestra cuándo cambia el estado, pero no tiene esas zonas grises que tiene los semáforos. Por ejemplo, en el problema anterior, se crean dos variables de condición que avisan cuándo el buffer *no está lleno* y cuando *no está vacío*
## Conexiones
- [[Problema de los productores y consumidores]]
- [[Variables de condición]]
- [[Semáforos]]
