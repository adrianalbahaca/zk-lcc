---
id: 202603191443
fecha: 19-03-2026
estado: completo
tags:
  - CompMatI
---
# Todo subgrafo de $K_5$ y $K_{3,3}$ es planar
## La idea en una oración
---
> Todo subgrafo de $K_5$ y de $K_{3,3}$ es planar. Es decir, $K_5$ y $K_{3,3}$ son los grafos minimales prohibidos para grafos planares
## Desarrollo
---
 Esto se puede demostrar por las desigualdades de antes:
 
 > Sea $K_5-v$. Entonces tendrá 4 aristas menos. Asumamos que el subgrafo es no plano, por lo que $|E(G')|>3|V(G')|-6$, pero con 4 vértices y 6 aristas, $|E(G)|=6 \le 3|V(G)|-6=3*4-6=6$ , lo cual es absurdo
 > Por lo tanto, tal subgrafo debe ser planar

Un razonamiento similar se puede hacer con $K_{3,3}$ pero con la desigualdad de grafos planares sin triángulos
## Conexiones
- [[Desigualdad en grafos K3-free]]
- [[Desigualdad en grafos planares]]
