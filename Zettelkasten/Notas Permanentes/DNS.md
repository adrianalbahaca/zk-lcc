---
id: 202610232013
fecha: 23-10-2026
estado: completo
tags:
  - Comms
---
# Domain Name System 
## La idea en una oración
---
> DNS es una implementación de un servidor de nombres que usa jerarquía y delegación para asociar direcciones IP con dominios
## Desarrollo
---
Para evitar manejar con direcciones IP directamente, causando sistemas caóticos y agobiantes, se ha inventado el concepto de **Servidores de Nombres**, los cuales asociaban nombres o *dominios* a direcciones IP a las que ir. Ahora, este sistema tenía 3 problemas
- Buscar por nombre se vuelve lento con el tiempo mientras más datos hay en el servidor
- La carga que debe aguantar cada servidor termina siendo alta
- Quien maneja los nombres termina siendo muy centralizado

Por ello, se ha creado *DNS*, el cual usa un sistema de jerarquías para *delegar* el trabajo de la búsqueda desde la raíz a el servidor de nombre con la dirección IP a buscar. Cada nivel administra autoritativamente al nivel inferior. Cada query usa búsquedas dedicadas, y cachea acorde
## Conexiones
- [[Jerarquías en DNS]]
- [[Queries en DNS]]
- [[DNS Resolver]]
- [[Actualización de zonas en DNS]]
- [[Zone Files]]
- 