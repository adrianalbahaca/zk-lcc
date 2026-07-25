---
id: 202607251835
fecha: 25-07-2026
estado: completo
tags:
  - ArquiComp
---
# Convención de llamadas a funciones en registros 
## La idea en una oración
---
> Al llamar una función, es necesario mantener en cuenta los registros *caller-saved* y *callee-saved*, conservando aquellos en la pila de ser necesarios
## Desarrollo
---
Para enviar los argumentos a las funciones, se usa una convención de llamada para los primeros 7 argumentos:
- Del argumento 1 al 7: `%rdi, %rsi, %rdx, %rcx, %r8, %9`
- Del argumento 8 en adelante: Se mete en la pila
- Para los flotantes: `%xmm0 - %xmm7`, el resto se mete en la pila
- Los registros `%rbx, %rbp, %rsp, %r12 - %r15` deben de conservar los mismos valores que tuvieron al llamar la función. Son *callee-saved*
- El resto de los registros (`%rax, %rcx`, etc) pueden cambiar de valor sin tener que conservarlos. Son *caller-saved*
## Conexiones
- [[]] 
