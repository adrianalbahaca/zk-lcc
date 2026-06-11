---
id: 202604301946
fecha: 30-04-2026
estado: borrador
tags:
  - SistOpI
---
# Garantías del SO al usar procesos 
## La idea en una oración
---
> El SO garantiza que los procesos están aislados entre sí, que el scheduler va a ser justos con cada proceso, y que hay mecanismos para que se comuniquen entre sí
## Desarrollo
---
La programación congruente suele ser algo engañosa, sin muchas garantías entre procesos. Para mitigar esto, se han definido unas garantías para cada proceso
1. Cada proceso está aislado del otro, y quiere decir que ningún proceso puede acceder a otro así como sí sin compartir memoria
2. Se garantiza que el scheduler le va a dar su tiempo a cada proceso y va a ser justo con la ejecución de cada proceso
3. Se asegura que cada proceso empiece con los recursos necesarios, y que se liberen completamente al finalizar el proceso
4. 
## Conexiones
- [[]] 
