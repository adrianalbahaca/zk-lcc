---
id: 202605140913
fecha: 14-05-2026
estado: completo
tags:
  - LFyC
---
# Partes de un lenguaje
## La idea en una oración
---
> Cada lenguaje se representa por un alfabeto, y es un subconjunto de palabras sobre el conjunto completo de palabras posibles sobre el alfabeto
## Desarrollo
---
Un *alfabeto* se representa con un conjunto de símbolos **finito** que están en un lenguaje. Se usará el símbolo $\Sigma$ para representarlo y serán con una cantidad de elementos pequeña, como por ejemplo $\Sigma = \{ a,b,c \}$. 

Luego, una *palabra* sobre un alfabeto es una secuencia **finita** de símbolos del alfabeto. Cuando la secuencia es infinita, va más a la *verificación de modelos*. La palabra vacía $\lambda$ tiene 0 símbolos

La potencia $\Sigma ^n$ del alfabeto $\Sigma$ se puede definir inductivamente, *pero no es un alfabeto. Es un conjunto de palabras*. Es como la diferencia entre `[a]` y `a`

El conjunto de todas las posibles palabras $\Sigma ^*$ es un conjunto infinito numerable, ya que se define como la unión infinita de conjuntos numerables $\Sigma ^n$ ($\Sigma ^* = \cup_{n \in \mathbb{N}_0} \Sigma^n$)

Finalmente, un *Lenguaje* sobre un alfabeto $\Sigma$, es un subconjunto de $\Sigma ^*$. Por esta definición, $\Sigma ^*$ mismo y $\{ \lambda \}$ son lenguajes también (ver práctica 1). Ej: Siendo $\Sigma = \{ 0,1 \}$, tenemos el lenguaje $A = \{ w \in \Sigma ^* : |w| = 3 \}$ que tiene 8 elementos

Con esto, se puede determinar el problema de *¿Esta palabra pertenece a este lenguaje?*. Mientras que, para $\Sigma ^*$ es bastante fácil determinarlo, para otros lenguajes, como el que tiene longitud número primo, es más complejo
## Conexiones
- [[Verificación de modelos]] 
- [[Autómatas de estado finito]]
