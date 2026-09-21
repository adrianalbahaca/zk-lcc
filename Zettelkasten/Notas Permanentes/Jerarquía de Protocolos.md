---
id: 202608171550
fecha: 17-08-2026
estado: borrador
tags:
  - Comms
---
# Arquitectura de la Red y Jerarquía de protocolos 
## La idea en una oración
---
> La jerarquía de protocolos especifica una pila de capas que se pueden comunicar por interfaz de manera vertical o por protocolo de manera horizontal entre iguales
## Desarrollo
---
En una arquitectura de red, su diseño se divide en capas, una basada de la que está abajo, para ofrecer servicios entre sí, abstrayendo las implementaciones entre cada capa

La pila de *protocolos* son los acuerdos que se tienen sobre cómo los *iguales* se van a comunicar entre sí. No hay transferencia de datos entre capas entre sí per se, sino que se descompone la información entre capas hasta llegar al *medio físico*

Entre capas, se usa una *interfaz* que define las operaciones y definiciones que ofrece la capa de abajo a la capa de arriba. De esta manera, una interfaz bien definida evita tener que cambiar todo un protocolo o implementación, si se le ofrece a la capa de arriba las mismas funciones y definiciones

Entonces, el protocolo se encarga de los acuerdos entre iguales y la interfaz se encarga de la comunicación física entre capas.

Nota que cada protocolo es independiente de los demás si no cambia la interfaz. Note además que las capas "hacen de cuentas" que se comunican directamente entre sí por el protocolo a través de la interfaz, pero es una comunicación *lógica*. La comunicación *física* se hace entre capas. El protocolo sólo es la *"regla del juego"* para que dos iguales se acuerden para entenderse

En general, una arquitectura de red bien diseñada tiene como características la *confiabilidad*, que la info. no se vea afectada fácilmente por interferencias, *evolución*, que se pueda expandir la red fácilmente, *asignación de recursos*, manejar los casos donde hay un emisor que manda a lo loco y un receptor que recibe poco, y *seguridad*
## Conexiones
- [[Aspectos de diseño para capas de una red]] 
