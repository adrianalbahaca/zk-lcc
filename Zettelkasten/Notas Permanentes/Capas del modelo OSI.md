---
id: 202609031210
fecha: 03-09-2026
estado: borrador
tags:
  - Comms
---
# Capas del modelo OSI
## La idea en una oración
---
> El modelo OSI tiene 7 capas: La capa física, la capa de enlace de datos, la capa de red, la capa de transporte, la capa de sesión, la capa de presentación y la capa de aplicación
## Desarrollo
---
El modelo OSI tiene 7 capas bien definidas:
1. **Capa física:** Se encarga de la transmisión de bits puro y crudo. Se especifica con la mecánica, eléctrica, temporización y medio físico
2. **Capa de enlace de datos:** Transforma el medio de transmisión puro en una línea de transmisión sin errores. Se hace dividiendo los datos en tramas y mandando secuencialmente y, si el servicio es confiable, se espera un mensaje de confirmación de recepción. Se debe considerar los casos de inundación de datos y el acceso al canal compartido
3. **Capa de red:** Se encarga del enrutamiento de los datos, ya sea de forma estática o dinámica. La congestión de la red, formas de los paquetes entre redes y demás se determina acá
4. **Capa de transporte:** Se encarga de "empacar" y "desempacar" los datos a la y desde la capa de red. Asegura un tipo de servicio de conexión y mantiene una tasa de error lo sufic. baja como para ignorarla en la práctica
5. **Capa de sesión:** Mantiene las sesiones entre computadoras, ofreciendo control de diálogo, manejo de tokens y sincronización
6. **Capa de presentación:** Verifica el formato y semántica de cada mensaje, viendo qué estructura de datos se intercambia
7. **Capa de aplicación:** Contiene la variedad de protocolos que los usuarios necesitan, como el *HTTP*
   
Note como cada capa se define de forma certera, sin ambigüedad entre las mismas
## Conexiones
- [[]] 
