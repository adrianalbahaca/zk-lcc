---
id: 202603242142
fecha: 24-03-2026
estado: completo
tags:
  - CompMatI
---
# Def. de Flujo y utilidad 
## La idea en una oración
---
> Sea $G$ una red adecuada. Un flujo $f:E(G) \rightarrow \mathbb{R}_0^+$ es una función tal que para toda arista $e$ de la red, $0 \le f(e) \le c(e)$ y para todo vértice $v$ de $G$, se cumple que $f^+(v) = f^- (v)$
## Desarrollo
---
Sea una red de bombeo de una ciudad, tal que tenemos subestaciones con una cierta capacidad. Queremos ver cuánta agua podemos bombear por toda la red, incluso hasta el nivel máximo de agua bombeable. O también, puede que queramos un matching máximo en un grafo bipartito.
Acá llega a la mano el concepto de *flujo*, una función desde las aristas a los reales positivos con el cero tal que todo flujo está entre el cero y la capacidad de la arista, y que cumple la propiedad de *conservación de flujo*
## Conexiones
- [[Caminos f-aumentantes]]
- [[Algoritmo de Ford-Fulkerson]]
- [[Corte en un flujo]]
