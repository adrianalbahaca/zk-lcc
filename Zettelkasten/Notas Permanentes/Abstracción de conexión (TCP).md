---
id: 202610051111
fecha: 05-10-2026
estado: completo
tags:
  - Comms
---
# Abstracción de conexión 
## La idea en una oración
---
> La abstracción de conexión usa el concepto de conexiones en un circuito virtual usando la dirección IP y puerto como terminales
## Desarrollo
---
Usando el concepto de un circuito virtual, las conexiones se reconocen por sus terminales, pares de tipo `(Dir. IP del host, puerto)`, que son únicos *en conjunto*. Esto permite que varias computadoras puedan tener un único receptor sin que el receptor abra un puerto por conexión. Además, permite la comunicación *concurrente*. Un ejemplo de esto es el email 
## Conexiones
- [[Concurrencia]] 
