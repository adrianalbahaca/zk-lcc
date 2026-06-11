---
id: 202606110842
fecha: 11-06-2026
estado: borrador
tags:
  - LFyC
---
# Lema del bombeo para LIC
## La idea en una oración
---
> Sea $L$ un lenguaje ind. del contexto infinito, en $L$ debe de haber al menos una palabra $\alpha$ de la formula $\alpha = svuwt$ donde $vw \neq \lambda$ tal que $\forall n, s(v^n)u(w^n)t \in L$  
## Desarrollo
---
El objetivo de su demo. es ver que existe una propiedad que los LIC cumplen, para después mostrar un lenguaje que no lo cumple y ver que no es LIC

>Si se considera $L \in LIC$, entonces tiene una gramática ind. del contexto tal que $L = L(G)$
>Si vemos $G=N, T, P, \sigma)$ y sea $n=|N|,k=|T|,m\in \mathbb{N}$, tal que $m$ es la longitud mínima del lado derecho de las producciones de $G$
>Toma una palabra $\alpha$ de $L$ tal que $|\alpha| > m^n$. La palabra de tal tamaño existe porque el lenguaje es infinito
>Considera el árbol $t$ de $\alpha$. Su profundidad es, al menos, $n$, o en otras palabras $Prof(t) \ge n$ . Eso indica que hay un camino de no terminales hasta una hoja, aparecerá más de $k$ símbolos, pero sólo hay $n$ no terminales. Por *principio de palomar*, **debe de haber un no terminal que se repita**
>En el subárbol donde ocurre esto, se denomina los extremos: $s$ es la trama del subárbol izquierdo de $\sigma$, $v$ es la trama del subárbol izquierdo de la primera representación del $N$ no terminal, $u$ es el punto medio de la segunda representación de $N$, $w$ es la trama del subárbol derecho de la primera representación de $N$ y $t$ es la trama del subárbol derecho de $\sigma$ 
>La palabra $\alpha$ queda como $svuwt = \beta_1 \gamma_1 N \gamma_2 \beta_2$
>

Quiere decir que el subárbol $N$ se puede copiar cuantas veces se quiera, siendo capaz de generar $s(v^n)u(w^n)t, n \in \mathbb{N}$ 

Piensa que, desde $\sigma$, formas un árbol con hijos sus terminales y no terminales. Los no terminales se extienden como árboles con los mismos tipos de hijos, y así sucesivamente
## Conexiones
- [[Principio de Palomar]] 
- [[Límite del Lenguaje Independiente del Contexto]]
