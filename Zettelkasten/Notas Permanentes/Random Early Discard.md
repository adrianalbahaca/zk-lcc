---
id: 202610121140
fecha: 12-10-2026
estado: completo
tags:
  - Comms
---
# RED: Protocolo en routers
## La idea en una oración
---
> RED asigna una probabilidad de descartar datagramas dependiendo de qué tan llena esté la cola del router
## Desarrollo
---
Debido a la división entre capas, la comunicación entre las mismas suele ser limitada. TCP no suele recibir información de la red cuando recibe paquetes y no puede enviar información de los paquetes en sí a capas inferiores

Un protocolo común de los routers es el *tail-drop*, descartar datagramas si la cola interna del router está llena. Esto puede causar *sincronización global*, donde un datagrama que contenga datos de N conexiones sea descartado por este protocolo, causando que N conexiones se vean afectadas. Esto TCP no lo puede detectar directamente de las capas inferiores

Para manejar esto, se usa el protocolo *RED*, o *Random Early Discard*. Se obtiene dos límites en la cola, $T_{min}$ y $T_{max}$, y una probabilidad $p$ que se mide como un *promedio con peso* con el cálculo:
$$
p = (1 - \gamma) \times avg_v + \gamma \times Tam_Q
$$
Donde el tamaño de la cola se mide por bytes para que la probabilidad de que se descarte un datagrama sea proporcional a su tamaño. Finalmente, se cumplen 3 reglas
- Si la cola tiene menos de $T_{min}$ bytes en datagramas, se agrega el datagrama nuevo a la cola
- Si la cola tiene más de $T_{max}$ bytes en datagramas, se aplica *tail-drop* y se descarta el datagrama
- Si la cola tiene una cantidad de bytes en datagramas entre $T_{min}$ y $T_{max}$, se descarta el datagrama acorde a la probabilidad $p$
## Conexiones
- [[Timeout y retransmisión]] 
