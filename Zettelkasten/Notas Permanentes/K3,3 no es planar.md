---
id: 202603171530
fecha: 17-03-2026
estado: completo
tags:
  - CompMatI
---
# El grafo $K_{3,3}$ no es planar
## La idea en una oración
---
> El grafo $K_{3,3}$ no es planar, y se demuestra con una desigualdad que sale del Teorema de Euler. Es uno de los grafos no planares minimales
## Desarrollo
---
Otro de los *grafos no planares minimales* es $K_{3,3}$ y su demostración está atado fuertemente con una desigualdad de grafos $K_{3-free}$

> Sea el grafo $K_{3,3}$, que no contiene ciclos impares y es conexo y bipartito.
> Asuma que $K_{3,3}$ es planar
> Por la desigualdad de grafos $K_{3-free}$ se tiene que $|E(K_{3,3})| \le 2|V(K_{3,3})|-4$ pero $|E(K_{3,3})| = 9 > 2|V(K_{3,3})|-4 = 8$, por lo que entonces llega a un absurdo
> Por esto, se concluye que $K_{3,3}$ no es planar

 Acá se demuestra el poder de las desigualdades demostradas desde el teorema de Euler
## Conexiones
- [[Desigualdad en grafos K3-free]]
