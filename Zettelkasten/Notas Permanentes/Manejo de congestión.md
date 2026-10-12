---
id: 202610121103
fecha: 12-10-2026
estado: completo
tags:
  - Comms
---
# Congestión
## La idea en una oración
---
> La congestión es manejada por TCP usando mensajes ICMP, ventanas de congestión, Prevención de Congestión por Decremento Multiplicativo y Slow-start
## Desarrollo
---
La congestión es la sobrecarga de datagramas en la red, que causa que los routers encolen datagramas a enviar. Llega un punto donde no se pueden encolar más y se pierden algunos

En TCP, esto se ve como un retraso más, por lo que se trata reenviando datagramas. Esto causa que más datagramas entren a la red, congestionándola más. Si esto continúa, se entra en un *colapso por congestión*, donde la red está tan sobrecargada que se vuelve inútil

Por ello, se implementan varias medidas para manejarlo y evitarlo:
- **Mensajes ICMP** para notificar de una congestión
- **Ventanas de congestión adaptativas**, usando una *ventana de congestión*. El cálculo se vuelve siendo `vent_nueva = min(vent_ack, vent_congestion)`, donde en circunstancias normales estas dos son iguales, pero en caso de congestión, se reduce la ventana
- **Prevención de Congestión por Decremento Multiplicativo** para ir reduciendo la ventana de congestión y aumentando el temporizador de back-off
- **Slow-Start** para retornar poco a poco a un ritmo anterior una vez la congestión se alivia
## Conexiones
- [[Prevención de congestión por decremento multiplicativo]]
- [[Slow-start]]
- [[Random Early Discard]]
