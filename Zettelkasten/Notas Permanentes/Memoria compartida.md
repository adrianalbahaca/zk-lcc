---
id: 202605031728
fecha: 03-05-2026
estado: completo
tags:
  - SistOpI
---
# Mem. Compartida: Riesgo grande, premio grande
## La idea en una oración
---
> Se puede alocar memoria virtual para que dos procesos relacionados la compartan. **Es riesgoso y propenso a fallos pero puede ser mucho más útil que mandar cosas**
## Desarrollo
---
A pesar de que enviar cosas a procesos puede ser útil, a veces puede ser mejor compartir el elemento directamente entre los procesos

La memoria compartida es una estrategia para ello, donde se aloca un espacio en memoria para guardar elementos donde los procesos pueden agregar al espacio, acceder, y leer de allí libremente

Sin embargo, **es muy riesgoso**. Muchas cosas pueden salir mal si no se tiene cuidado de cómo se maneja este segmento
## Conexiones
- [[Ejemplo de compartir memoria entre procesos]] 
