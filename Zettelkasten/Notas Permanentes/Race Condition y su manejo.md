---
id: 202605112133
fecha: 11-05-2026
estado: borrador | completo
tags:
---
# Condición de carrera: Qué es y cómo evitarlo
## La idea en una oración
---
> La condición de carrera es un error de código que ocurre cuando el resultado de un código depende del orden impredecible de llegada de eventos
## Desarrollo
---
Durante los eventos concurrentes de un programa donde se tiene memoria compartida entre procesos, la categoría de error más sutil y letal es la *condición de carrera*, donde el resultado de un programa depende del orden impredecible donde los procesos acceden a memoria. Suele ocurrir porque las operaciones hechas sobre la memoria no suelen ser *atómicas*

Por ejemplo, considera el problema del productor y consumidor. Mientras que un productor puede estar creado un dato en un espacio de memoria *v*, tal espacio de memoria puede ser consumido a la vez, si no se sincronizan entre sí, causando resultados inesperados

Para lidiar con esto, es necesario crear un sistema de sincronización u exclusión mutua entre los procesos
## Conexiones
- [[Operación atómica]]
- [[Exclusión mutua]]
