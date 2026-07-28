---
id: 202607281257
fecha: 28-07-2026
estado: completo
tags:
  - ArquiComp
---
# La pila en Assembly x86-64
## La idea en una oración
---
> La pila interna en cada función es determinada por los arreglos `%rbp` y `%rsp`. Permiten guardar variables locales, datos temporales, y enviar los argumentos 7mo en adelante 
## Desarrollo
---
En cada llamada, tenemos los registros acordes para mantener la base y el tope de la pila, `%rbp` y `%rsp` respectivamente. Tienen instrucciones asociadas
- `push` que resta 8 a `%rsp` y guarda su valor allí. Su equivalente es `%subq $8 %rsp | movq %rax (%rsp)`
- `pop` que lee de donde se apunta en `%rsp` y le suma 8 para reducir el espacio. Su equivalente es `movq (%rsp), %rax | addq $8 %rsp`
Debido a el tamaño de los movimientos, explica por qué la pila debe estar alineada a 8 bytes para evitar desincronizaciones en llamadas a funciones
## Conexiones
- [[]] 
