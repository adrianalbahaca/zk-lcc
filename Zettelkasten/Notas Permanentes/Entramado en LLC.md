---
id: 202609221126
fecha: 22-09-2026
estado: completo
tags:
  - Comms
---
# Cómo funciona el entramado en LLC
## La idea en una oración
---
> El primer objetivo involucra delimitar las tramas del mensaje a enviar, para asegurarnos de que lleguen todos los paquetes
## Desarrollo
---
El entramado usa un mecanismo de *suma de verificación*, un cálculo que hace al recibir los paquetes que asegura que se compara el número recibido con el resultado esperado, usando la disparidad para detectar errores. Ahora, para dividir los paquetes, se usan varios métodos
- **Conteo de bytes:** El encabezado especifica el número de bytes que hay en la trama. Este usa muy poco ancho de banda pero tal encabezado puede ser corrompido en la transmisión
- **Byte banderas y relleno de bytes:** Se usa un byte delimitador para sincronizar al receptor, como banderas. Para evitar que se mezcle en los datos, se usan bytes de escape para delimitarlos de los bandera
- **Violaciones de codificación:** En casos como el *4B/5B*, la capa física puede delimitar ciertos patrones específicos que se deben de recibir para garantizar el envío correcto de paquetes
## Conexiones
- [[4B-5B]] 
