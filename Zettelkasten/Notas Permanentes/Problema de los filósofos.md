---
id: 202606290938
fecha: 29-06-2026
estado: completo
tags:
  - SistOpI
---
# Problema de filósofos: Exclusión mutua en una tabla circular
## La idea en una oración
---
> En una mesa circular de $N$ filósofos, cada uno toma los cubiertos en un cierto orden, come, los deja, y después se ponen a pensar. Cómo evitamos que todos tomen los cubiertos y nadie deje para el otro
## Desarrollo
---
### Descripción del problema
---
En una mesa circular de 5 filósofos, pasan la vida alternando entre comer y pensar. Comen un tipo de pasta que requiere dos tenedores. Acuerdan el tomar el tenedor derecho, y después el izquierdo antes de comer, y después dejar ambos en el mismo orden para después pensar. Si no consiguen los dos tenedores, deben esperar a que el otro esté disponible
### Posibilidad de Deadlock
---
Si todos los filósofos toman el tenedor derecho a la vez, se quedarán esperando infinitamente a que el otro suelte el tenedor izquierdo, causando que nunca coman y se mueran de hambre
### Soluciones
---
- *Uno de los filósofos sea zurdo:*
  Asuma que esto no resuelve el problema y que todos los filósofos tomen el tenedor derecho. El filósofo zurdo empezaría tratando de tomar el tenedor izquierdo, pero no podría porque su compañero lo toma, por lo que tendrá que esperar, pero eso deja que el tenedor derecho del filósofo zurdo siempre esté disponible
- *Sólo $N-1$ filósofos pueden comer a la vez*:
  Siempre dejando un espacio para que nunca se tomen todos los tenedores, permite que todos los filósofos coman sin problema
### Trampas
---
- *ˀ¿Y si sueltan el tenedor derecho cuando no esté disponible y esperan un poco?:* No es muy efectivo, ya que todavía existe la posibilidad de que todos los filósofos tomen el tenedor derecho a la vez, causando que lo suelten al ver que no está el izquierdo y que se queden esperando. Esto causaría un Livelock 
## Conexiones
- [[Mutex]]
- [[Multiplex]]
- [[Deadlock y Livelock]]