---
id: 202607261813
fecha: 26-07-2026
estado: borrador | completo | pendiente
tags:
  - ArquiComp
---
# Título de la idea (en forma de afirmación) 
## La idea en una oración
---
> Los movimientos básicos se dan por los comandos `mov`, `add`, `sub`, `mul`, `div`. Imitan operaciones que se dan en C
## Desarrollo
---
Ciertos movimientos en C tienen sus semejanzas en Assembly x86-64
- `mov` permite copiar elementos de un sitio a otro
```x86asm
# int a = b
subq $4, %rsp
movl %ebx, -4(%rbp) # movq
```
- `add`, `sub`, `imul`, `idiv` permite hacer las instrucciones de suma, resta, multiplicación y división acorde
- `inc` y `dec`, permiten incrementar y decrementar acorde
```x86asm
# a++
movl -4(%rbp), %eax
incl %eax
movl %eax, -4(%rbp)
```
## Conexiones
- [[]] 
