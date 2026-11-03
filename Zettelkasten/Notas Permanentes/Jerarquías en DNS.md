---
id: 202610232026
fecha: 23-10-2026
estado: borrador
tags:
  - Comms
---
# Sistema de jerarquías en DNS 
## La idea en una oración
---
> El query empieza desde el *root* para después ser delegado a *gTLD* y/o *ccTLD* para después poco a poco ser delegado a niveles inferiores
## Desarrollo
---
En un query, la búsqueda empieza con una consulta al *root*, el cual es administrado por la organización sin fines de lucro ICANN. Esta otorga a sus otros niveles de forma autoritativa los dominios acordes. De allí, se continúa a los **Top Level Domains**, que se dividen en 2:
- ***gTLD (Generic Top Level Domain):*** Acá se agrupa los dominios como `.com`, `.edu`, `.org`, `.gov`
- ***ccTLD (Country Code Top Level Domain):*** Estos son dados a gobiernos federales para delegar a provincias, estados o por función. Acá se agrupa los códigos de países como `.ar`, `.ve`, `.br`, etc. Además, los gobiernos pueden también delegarlos por funciones como `.co` para compañía, `.ac` para academia, etc

De acá, continúa los niveles inferiores, los cuales contienen el nombre del dominio en sí. Estos pueden ser *SLD (Second Level Domain)* o los terciarios
## Conexiones
- [[Servidores ARPA]] 
