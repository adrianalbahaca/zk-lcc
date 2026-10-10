---
id: 202609221022
fecha: 22-09-2026
estado: completo
tags:
  - Comms
---
# Link Logical Control: LCC 
## La idea en una oración
---
> La subcapa superior LLC le da una interfaz entre la capa de red y la capa física, incluyendo control de errores y flujo
## Desarrollo
---
La subcapa LLC ofrece servicios de control de flujo y control de errores. Los 3 servicios esenciales que recibe son:
- **Sin conexión ni confirmación de recepción**: La capa no da esfuerzo en recuperar paquetes posiblemente perdidos. Se usa cuando la tasa de error en la transmisión es baja
- **Sin conexión, con confirmación de recepción:** Se usa en canales no confiables, donde se les da a cada trama un requisito de confirmación al emisor
- **Con conexión y confirmación de recepción:** Se requiere un handshake previo antes de enviar tramas, y cada trama es numerada, para confirmar la llegada y el orden. Se usa en enlaces largos y poco confiables
## Conexiones
- [[Entramado en LLC]]
- [[Control de errores en LLC]]
- [[Control de flujo en LLC]]
