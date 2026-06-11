---
id: 202603192108
fecha: 19-03-2026
estado: borrador
tags:
  - SistOpI
---
# Si ocurre, el kernel los mata (deah)
## La idea en una oración
---
> Si el padre termina antes que el child, el kernel los adopta para terminar con ellos (re sádico esta película)
## Desarrollo
---
En caso de que el padre termine antes que los hijos, el *kernel* los toma y ejecuta un `wait()` para recibir la señal de los hijos cuando terminen, y así eliminarlos
En realidad, el kernel hace estas llamadas periódicas para cada hijo que no tenga padres, ya que, de no hacerlo, los hijos terminan en estado *zombie*, consumiendo espacio que otros procesos pueden tomar
## Conexiones
- [[]] 
