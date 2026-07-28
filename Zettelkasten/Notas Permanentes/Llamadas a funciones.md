---
id: 202607281311
fecha: 28-07-2026
estado: completo
tags:
  - ArquiComp
---
# Llamadas a funciones externas 
## La idea en una oración
---
> Siguiendo la convención de llamadas a funciones, las instrucciones `call` y `ret` permiten los saltos a funciones acorde 
## Desarrollo
---
Se tiene dos instrucciones clave para hacer las llamadas a funciones:
- `call` pushea la dirección de retorno y hace el salto de línea a donde se quiere hacer. Su equiv. es `pushq %rip_siguiente | jmp funcion`
- `ret` se encarga de popear el valor de retorno para después saltar al mismo. Usa un registro implícito. Su equiv. es `popq %reg | jmp %reg`

Con esto en mente, para llamar a una función, se sigue el siguiente protocolo
- Se guarda los argumentos 1 al 7 siguiendo la convención de llamada
- El resto de los argumentos se meten a la pila con `pushq` *en orden inverso*
- Se usa `call` para llamar la función
- Si hay argumentos en la pila, se buscan desde `16(%rbp)` en adelante
- Finalmente, se cierra la función con `ret`
## Conexiones
- [[Convención de llamada a funciones]] 
