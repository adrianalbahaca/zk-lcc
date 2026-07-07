---
id: 202604240932
fecha: 24-04-2026
estado: borrador
tags:
  - LFyC
---
# $ACK^{(1)}$ no es FRP
## La idea en una oración
---
> Sea $ACK^{(1)}:\mathbb{N} \rightarrow \mathbb{N}$, esta función no es FRP porque no cumple la propiedad de mayora, a pesar de que es computable y total
## Desarrollo
---
Siendo $ACK^{(1)}:\mathbb{N} \rightarrow \mathbb{N}$ con la ley $ACK(n) = f_n(n)+1$, tenemos que, a pesar de que es total y computable, no hay $k$ tal que $f_k(x) \uparrow ACK(x)$, demostrando que $ACK \notin FRP$ 
Esta se demuestra por contradicción y diagonalización, ya que esta función se construye con la función de la diagonal de la serie de Ackermann 
## Conexiones
- [[]] 
