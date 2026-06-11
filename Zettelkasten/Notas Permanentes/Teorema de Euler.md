---
id: 202603171505
fecha: 17-03-2026
estado: completo
tags:
  - CompMatI
---
# Demo. del Teorema de Euler
## La idea en una oración
---
> Si un grafo $G$ es planar y conexo con $n$ vértices, $e$ aristas y $c$ caras, entonces, $n-e+c=2$ 
## Desarrollo
---
Este teorema se demuestra usando *inducción* sobre el conjunto de grafos conexos y planos con $e$ aristas

> *Caso base:* Sea el grafo $G$ tal que no tiene aristas. Como $G$ es conexo, entonces sólo puede contener 1 vértice y 1 cara, por lo que $v-e+c=1-0+1=2$, por lo que cumple
> *Caso inductivo:* Asuma que el teorema cumple para grafos $H$ conexos y planares con $e=k$. Sea $G$ grafo conexo planar con $e=k+1$
> 	- Si $G-a$ es conexo, entonces una de sus caras se debió de haber fusionado, y por el $HI$, se tiene que $v-e+(c-1)=2$. Entonces, al agregarle la arista de vuelta, queda que $v-(e+1)+(c-1) = v-e+c = 2$
> 	- Si $G-a$ es disconexo, $a$ es una arista de corte y $G$ se divide en componentes conexas. Al juntarlos de vuelta, se tiene que también cumple el teorema
> Como cumple para el caso base y el paso inductivo en el conjunto inductivo de grafos planares conexos, se tiene que el teorema aplica para todo grafo conexo planar $\blacksquare$  

Gracias a este teorema, es posible conseguir cotas usando datos como la cant. de vértices, de aristas o de caras
Hay una segunda versión con inducción sobre la cantidad de vértices
## Conexiones
- [[Principio de Inducción Primitiva]] 
- [[Desigualdad en grafos planares]]
- [[Desigualdad en grafos K3-free]]
