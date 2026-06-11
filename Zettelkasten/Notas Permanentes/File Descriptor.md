---
id: 202603192037
fecha: 19-03-2026
estado: borrador
tags:
  - SistOpI
---
# Def. del File Descriptor
## La idea en una oración
---
> El *File Descriptor* designa un entero positivo a un archivo abierto para su uso. Cada proceso tiene una tabla para todos los archivos abiertos del proceso
## Desarrollo
---
A cada archivo abierto en un proceso se le designa un *File Descriptor*, un entero positivo
**Por ejemplo:** `stdin` es 0, `stdout` es 1 y `stderr` es 2
Estos `fd`s están guardados en una tabla que se le designa a cada proceso, que es el *File Descriptor Table*
## Conexiones
- [[File Descriptor Table]] 
