---
id: 202610091829
fecha: 09-10-2026
estado: completo
tags:
  - Comms
---
# Algoritmo de Kahn para backoff timeout
## La idea en una oración
---
> Ya que medir la muestra de tiempo de envío de trama es ambiguo, se decide empezar con un límite e ir aumentándolo con cada transmisión
## Desarrollo
---
En teoría, medir una muestra de tiempo en envío de datos es fácil, pero como TCP usa ACK por el punto de armado del paquete y no de la trama en sí, el contenido entre ambas es igual, por lo que no se pueden diferenciar entre envíos primerizos u retransmisiones

Asumir más a que sean los originales puede causar que $RTT$ crezca sin límites con cada pérdida, causando un ciclo vicioso. Asumir que es retransmisión causaría que, en picos de retrasos, $RTT$ se achique para otras transmisiones

Por ello, el Algoritmo de Kahn empieza con un cierto timeout, y lo aumenta con cada retransmisión. Para la siguiente transmisión que se reciba a la primera, se resetea el timeout. La fórmula es
$$
T_n = \gamma \times T_v
$$
donde $\gamma$ empieza siendo 2
## Conexiones
- [[]] 
