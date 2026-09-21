---
id: 202608141622
fecha: 14-08-2026
estado: borrador
tags:
  - TBD
---
# Bases del modelo Entidad-Relación 
## La idea en una oración
---
> El modelo entidad-relación representa la realidad en entidades, atributos a los mismos y las relaciones entre ellas
## Desarrollo
---
Hay 3 constructores en este modelo:
- Entidad (Rectángulo): Objetos diferenciables de las demás con existencia propia. Un conjunto del mismo representa entidades del mismo tipo. Un ejemplo es `ESTUDIANTE`
- Atributo (Óvalo): Propiedad descriptiva que todas las instancias comparten, como para un `ESTUDIANTE` que tiene `dni`, `nombre` y `fecha-de-nacimiento`. Su dominio son los valores posibles para un atributo, restringiendo los valores a tomar. Cómo construir cada tipo (String, tupla de elementos, enteros) depende del diseño. Hay simples y compuestos, monovaluados y multivaluados, derivados y almacenados, etc ***(EXPANDIR)***
- Relación (Rombo): Asociación de instancias entre dos o más entidades. Cada relación tiene un nombre descriptivo. Su *grado* indica cuántas entidades se involucran, su *rol* indica qué función cumple en la entidad, indispensables en *relaciones recursivas* 
Luego, las líneas conectan estos elementos entre sí
## Conexiones
- [[Entidad]]
- [[Atributo]]
- [[Relación]]
- [[Claves]]
