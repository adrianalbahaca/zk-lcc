---
id: 202610091822
fecha: 09-10-2026
estado: borrador | completo | pendiente
tags:
---
# Timeout y retransmisión
## La idea en una oración
---
> Por la varianza del tráfico, no es posible dar un timeout fijo. Tiene que ser adaptativo al tráfico y se usa el algoritmo de Kahn para evitar ambiguedad del ACK
## Desarrollo
---
Debido a lo variado que puede ser el tráfico en el Internet, un ACK puede tomar un camino corto pero otro más largo en la red. Este comportamiento impredecible hace que el timeout no pueda ser fijo. Si es muy largo, se puede perder tiempo en una pérdida genuina, y si es muy corto, se puede retransmitir paquetes innecesarios, causando más tráfico
Por ello, se usa un *timeout adaptativo*. En cada transmisión, se calcula un *tiempo de viaje de trama* ($RTT$) usando el antiguo y se toma la muestra de este envío, usando un promedio como sigue:
$$
RTT = (\alpha \times RTTv) + ((1-\alpha) \times M)
$$
Luego, el timeout para hacer una transmisión es
$$
Timeout= \beta \times RTT
$$
Tome en cuenta que $\alpha$ y $\beta$ son *pesos constantes*. Se recomienda que $\beta = 2$. $\alpha$ se usa para regular qué tan sensible debe ser a retrasos en tiempo real. Ahora, 
## Conexiones
- [[Algoritmo de Kahn]]
- [[Alta varianza en retraso]]
