---
id: 202605122203
fecha: 12-05-2026
estado: completo
tags:
  - EDyAII
---
# Def. y propósito de las estructuras inmutables
## La idea en una oración
---
> Una estructura inmutable es aquella tal que las modificaciones no borran datos de la estructura, sino que copian la estructura con los datos extra
## Desarrollo
---
En `C` y `Python`, se suelen definir estructuras efímeras, de las cuales sólo existe una versión de la estructura, donde cada cambio destruye la versión anterior y da la nueva versión

En cambio, en `Haskell`, toda estructura definida acá es *inmutable*. Cada modificación crea una copia de la estructura a modificar añadiendo la modificación
Esto permite la paralelización más fácilmente, y permite dar varias versiones a la misma estructura, pero es necesario tener un garbage collection **muy** bueno, ya que el uso de la memoria va a ser mayor

Por ejemplo, concatenar dos listas efímeras como `zs = xs ++ ys` hará que `xs` no exista más como variable, y sólo sea `zs` el resultado final. Mientras que, si fueran inmutables, las copias `xs` e `ys` seguirían existiendo, con una copia nueva `zs` de la lista concatenada
## Conexiones
- [[Inmutabilidad en ABBs]]
- [[Inmutabilidad en Red-Black Trees]]
- [[Inmutabilidad en Heaps]]
