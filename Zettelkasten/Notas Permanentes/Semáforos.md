---
id: 202605251656
fecha: 25-05-2026
estado: completo
tags:
  - SistOpI
---
# Def. y uso de los semáforos
## La idea en una oración
---
> Los semáforos son instrumentos de coordinación entre hilos que imitan un entero que sólo se puede incrementar y decrementar de a uno
## Desarrollo
---
Un semáforo sólo tiene 3 características:
- Al inicializarlo, se puede iniciar en un cierto valor entero, pero sólo se puede incrementar y decrementar. No se puede leer el valor del semáforo
- Al decrementar, se reduce de a uno el valor del mismo antes de dejar que el hilo continue. Si llega a cero o menor que ello, el hilo se bloquea hasta que alguien incremente el semáforo
- Si se incrementa, y antes estaba en cero, se libera nada más uno de los hilos en el incremento hasta que el valor sea positivo
Hay unas consecuencias dadas de esta definición
- Al incrementar y liberar uno de los hilos, no se sabe exactamente cuál se va a liberar, o si es que ya había una bloqueada previamente
- Si el valor del semáforo era mayor a 1 y se decrementa, el hilo seguirá adelante, siendo el siguiente hilo que decremente que se bloquee
- Al inicializar, se puede empezar con un valor positivo para permitir ciertos hilos que pasen, o un valor negativo (Como una *barrera*), para que se bloqueen cierta cantidad de hilos a incrementar hasta que se llegue a algo mayor a cero y se continue todos a la vez
Esta herramienta permite resolver varios problemas planteados
## Conexiones
- [[Deadlock y Livelock]]
- [[Problema de la barbería]]
- [[Problema de los productores y consumidores]]
- [[Problema de los lectores y escritores]]
- [[Diferencias entre semáforos y var. condición]]
- [[Problema de los filósofos]]
- [[Algoritmo de Peterson]]
- [[Algoritmo de la Panadería]]