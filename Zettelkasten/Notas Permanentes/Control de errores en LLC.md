---
id: 202609221131
fecha: 22-09-2026
estado: completo
tags:
  - Comms
---
# Cómo se detecta los errores en LLC
## La idea en una oración
---
> El LLC usa una combinación de tramos de control, temporizadores y números de secuencia para detectar que cada paquete haya llegado, y saber cuándo solicitar el reenvío de una trama
## Desarrollo
---
Primero, para poder verificar conexión y confirmación de recepción, se usa *tramas de control*. Ahora, para proteger ante la posibilidad de que alguno de los lados se quede esperando infinitamente tales tramas, se usan *temporizadores* para parar la espera en caso de que se acabe el tiempo. Por último, en caso de reenvío accidental de tramas, se usan *números de secuencia* para distinguir entre tramas nuevas y tramas reenviadas 
## Conexiones
- [[]] 
