---
id: 202603152232
fecha: 15-03-2026
estado: borrador
tags:
  - SistOpI
---
# Cómo funciona Linux para crear y cerrar procesos
## La idea en una oración
---
> `fork()` y `exit()` se encargan de crear procesos y de cerrarlos con un código 
## Desarrollo
---
Linux tiene la peculiaridad de no crear procesos para hacer una tarea directamente como lo hace Windows, sino que divide el proceso y después sale de cada uno
`fork()` es un comando que duplica el proceso en memoria. Toda la estructura, *pila*, *heap*, *instrucciones de máquina*, es "duplicada" (No es literalmente así pero se puede pensar de esa manera).
`exit()` cierra el proceso y sale con un  `status` para retornarlo al padre que lo invocó
Linux da unas herramientas para hacer el proceso de crear otros procesos más manual
## Conexiones
- [[]] 
