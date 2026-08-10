---
id: 202607302146
fecha: 30-07-2026
estado: completo
tags:
  - ArquiComp
  - Compiladores
---
# Registros generales y sus pseudónimos en ARM 
## La idea en una oración
---
> En ARM, los registros generales van de `r0-r15`, los de VFP para punto flotante van de `s0-s31` 
## Desarrollo
---
Los registros en ARM son mucho más fáciles de visualizar, pero algunos tienen un uso especial
- `r0` se usa como registro de retorno de valores
- La convención de llamada usa los registros `r0-r3` para guardar los argumentos
- `r13` es el *stack pointer*, con sinónimo `sp`, que se usa para indicar el tope de la pila
- `r11` se suele usar como el *base pointer*
- `r14` guarda la dirección de retorno, y se suele llamar tambien `lr`
- `r15` se usa como *program counter*, y se suele llamar como `pc`
- `s0-s15` son registros del VFP para pasar argumentos flotantes a una función, y para retornar el resultado
- `s16-s31` son registros *caller-saved* para FPV
- `d0-d7` sirven para pasar argumentos double a funciones, retornando en `d0`
## Conexiones
- [[]] 
