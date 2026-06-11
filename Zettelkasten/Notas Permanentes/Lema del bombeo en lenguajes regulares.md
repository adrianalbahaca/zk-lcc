---
id: 202605210916
fecha: 21-05-2026
estado: borrador
tags:
  - LFyC
---
# Var. del lema del bombeo en lenguajes regulares y su uso 
## La idea en una oración
---
> Sea $L$ un lenguaje regular con cadenas infinitas de la forma $x^n g^n$, entonces $L$ tiene infinitas cadenas de la forma $x^k g^j$ con la forma $k \le j$ 
## Desarrollo
---
El lema no dice de cosas que no son regulares. Más bien, lo que dice es una propiedad de lenguajes regulares. Con esto, si un lenguaje no cumple tal propiedad, no es regular. Similar a cómo demostramos que existen funciones que no pueden ser $FRP$

> Sea $L$ un lenguaje regular, entonces existe un autómata AEFD $A$ tal que $L(A)=L$, y sea $n$ la cantidad de estados de dicho autómata. Note que existe $k \ge n : x^k y^k \in L$ 
> Viendo la secuencia de estados que reconoce $x^k y^k$, $S_0 \rightarrow^x S_1 \rightarrow^x .. \rightarrow^x S_k \rightarrow^y S_{k+1} \rightarrow^y ... \rightarrow^y S_{2k}$, *hay entre $S_0$ y $S_k$ algún estado que aparece al menos 2 veces* . En otras palabras, hay un ciclo en el autómata **(Variante del teorema de palomar)**
> Ahora, sea $j$ la cantidad de transiciones entre estados repetidos, podemos ver que existe un camino en el mismo tal que $x^{k+j}y^j$ es aceptado. Esto se puede repetir $r$ veces $\blacksquare$

En resúmen: Lo que nos dice es que **Los autómatas finitos no tienen memoria**. Como corolario, se tiene que el lenguaje $L(G) = \{ 0^n 1^n : n \in \mathbb{N} \}$ no es regular, ya que, de serlo, debería de aceptar la cadena $0^n 1^m$ tal que $n \not= m$, pero no es así

Es algo súper pequeño pero casi esencial para demostrar que hay lenguajes no regulares

*Esto es sólo válido para lenguajes con más de dos caracteres en su alfabeto*
## Conexiones
- [[Límites de las FRP]] 
- [[Teorema del palomar]]
