---
id: 202609211329
fecha: 21-09-2026
estado: borrador
tags:
  - Comms
---
# Balanceo de señal
## La idea en una oración
---
> Una señal balanceada es aquella tal que el promedio de los voltajes enviados sea de cero. Esto evita que haya un componente CD en la señal
## Desarrollo
---
Hay varios métodos para balancear la señal
- **AMI**: Mientras se envía las señales usando voltajes positivos y negativos, se alterna entre los voltajes para balancear la señal
- **8B/10B**: En cada patrón de 8 bits, 5 bits se asocian a un patrón de 6 bits, y este se concatena con la asociación de los 3 bits restantes con 4 bits. Esta asociación se hace tal que se balancee la señal, guardando la *disparidad* para ir cancelándola. En promedio, la disparidad no supera los 2 bits
## Conexiones
- [[]] 
