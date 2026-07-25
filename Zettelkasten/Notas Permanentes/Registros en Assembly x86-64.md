---
id: 202607251827
fecha: 25-07-2026
estado: completo
tags:
  - ArquiComp
---
# Registros de propósito general en Assembly x86-64
## La idea en una oración
---
> Hay 15 registros a usar en Assembly x86-64, donde algunos de ellos son de uso especial, como para la pila, números flotantes, etc
## Desarrollo
---
Los registros disponibles en Assembly x86-64 son los siguientes: `%rax, %rbx, %rcx, %rdx, %rsi, %rdi, %rbp, %rsp, %r8 - %r15`. Dentro de los mismos, tenemos que
- `%rbp` es el registro para la base de la pila y `%rsp` representa su tope. El último se mueve de forma dinámica, ajustando espacio en la pila para guardar variables locales, mientras que el primero se mantiene estático para usarlo como referencia al buscar
- Los registros `%xmm0 - %xmm7` se usan para trabajar con números flotantes, disponibles en algunos CPUs
Cada uno de estos registros tiene tamaños de 64 bits (`%rax`, `%rsi`, `%r8`), 32 bits (`%eax`, `%esi`, `%r8d`), 16 bits (`%ax`, `%si`, `%r8w`), y la parte alta y baja de 8 bits (`%ah` | `%al`, `%sil`, `%r8b`)
El comando `info registers` nos permite ver los contenidos de los registros en GDB
## Conexiones
- [[]] 
