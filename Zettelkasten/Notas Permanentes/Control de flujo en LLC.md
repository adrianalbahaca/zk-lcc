---
id: 202609221134
fecha: 22-09-2026
estado: completo
tags:
  - Comms
---
# Cómo se controla el flujo en LLC
## La idea en una oración
---
> Para evitar que el receptor se sature con lo recibido del emisor, se usa un control ya sea en tiempo real o fijo antes de enviar
## Desarrollo
---
Existe la posibilidad de que el emisor sea más potente que el receptor, causando que, cuando el emisor envíe, el receptor se sature, no pueda recibir toda la información y la pierda. Por ello, se tiene dos mecanismos para necogiar el flujo:
- **Control por retroalimentación:** En la señal *ACK* que envía el receptor cada vez que recibe paquetes, se agrega información de saturación del receptor antes de seguir enviando tramas. En tiempo real, el emisor ajusta acorde. Sin embargo, esto consume más ancho de banda
- **Control por tasa:** El receptor negocia la tasa de recepción que tiene, ya sea porque viene con su protocolo u otros, y no avisa de forma activa mientras el emisor manda los datos. Es más simple pero todavía corre el riesgo de que el receptor se sature
## Conexiones
- [[]] 
