---
id: 202610271154
fecha: 27-10-2026
estado: completo
tags:
  - Comms
---
# Cómo actualizar una zona de DNS 
## La idea en una oración
---
> Para actualizar la zona, se usa la dinámica de *Maestro-Esclavo* que tienen estos servidores, usando mensajes, IZT o actualizaciones dinámicas
## Desarrollo
---
Una *zona* es el dominio bajo una administración a través del archivo de zona. Este contiene *Resource Records* que describen al dominio o sub-dominio. Para que un servidor esclavo se actualice, hay 3 métodos:
- **Actualización de Zona Completa:** El servidor esclavo pide los *RR* al servidor maestro y compara los números seriales. Si el que recibe es mayor al que tiene, actualiza sus datos
- **Actualización de Zona Incremental:** Aplica un mecanismo similar usando una tasa de *refresh* para que el esclavo solicite los RR al maestro, y permite sólo actualizar aquellos RR que hayan sufrido cambios. De esta manera, no se transfieren archivos excesivamente grandes en cada actualización, pero ambos servidores deben ser compatibles
- **NOTIFY:** Para evitar que el esclavo tenga que tomar la iniciativa para pedir las actualizaciones y que corra el riesgo de demoras en la información, el maestro puede mandar una notificación a los esclavos para que pidan actualizaciones
- **Actualizaciones dinámicas:**
## Conexiones
- [[]] 
