---
id: 202610271145
fecha: 27-10-2026
estado: completo
tags:
  - Comms
---
# Querying en DNS
## La idea en una oración
---
> Cuando se hace un query, un resolver se encarga de atenderla, haciendo varios requests iterativos y recursivos para dar la respuesta
## Desarrollo
---
Suponga que quiere buscar la dirección de la página `fred.example.com.`:
1. El navegador hace el request al *stub-resolver*, y este verifica en su caché si se ha hecho esta búsqueda antes
2. Sino, se delega al *DNS resolver* del ISP para que haga el **Query Recursivo**, es decir, que obtenga la respuesta final o un error. Este hace el primer request en el root `.`, usando un **Query iterativo**
3. El root le contestará con un *referral* al servidor TLD `.com`. El resolver le consulta de la misma forma y recibe otro *referral* al servidor de `example.com`
4. Finalmente, se le hace la consulta a estos servidores y le contestan con un *Record* de nivel *A* (O *AAAA* si se usa IPv6) para obtener la dirección IPv4
5. El resolver guarda en su caché `fred.example.com. = x.x.x.x`, y se lo pasa al stub-resolver, que hará lo mismo
6. La respuesta final llega al navegador y el mismo puede establecer una conexión a la dirección IP recibida

Note la jerarquía entre servidores. Se ha iniciado con el **Query Recursivo** desde el *Resolver* del ISP, a múltiples servidores con **Query Iterativo**. Si en algún momento los queries iterativos retornaran un error, su respuesta final al navegador sería algún `NXDOMAIN` u otro error que indique qué pasó
## Conexiones
- [[]] 
