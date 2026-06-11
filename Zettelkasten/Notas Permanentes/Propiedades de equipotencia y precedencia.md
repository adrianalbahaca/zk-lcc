---
id: 202603071509
fecha: 07-03-2026
estado: completo
tags:
  - LFyC
---
# Propiedades de equipotencia y precedencia
## La idea en una oración
---
> La relación de equipotencia $\sim$ es de equivalencia, mientras que la relación $\preceq$ es de grado
## Desarrollo
---
 Se puede demostrar que la relación de equipotencia es una relación de equivalencia
 1. **Es reflexiva:** Sea un conjunto $A$, con la función identidad $f: A \rightarrow A$, tal que $f(a) = a$, naturalmente es biyectiva, por lo que $A \sim A$
 2. **Es simétrica:** Sean dos conjuntos $A, \ B$, tal que $A \sim B$, entonces, tenemos la función $g: B \rightarrow A$ con ley $g(b) = f^{-1}(b)$, ya que $g$ tiene inversa, es biyectiva, y entonces $B \sim A$
 3. **Es transitiva:** Sean 3 conjuntos $A, \ B, \ C$, tal que $A \sim B$ y $B \sim C$, entonces, con funciones $f: A \rightarrow B$ y $g: B \rightarrow C$ biyectivas, la función $h: A \rightarrow C$ con la ley $h(a) = f(g(a))$, es una función biyectiva, por lo que $A \sim C$

También, se puede demostrar que la relación de precedencia es una relación de grado
1. **Es reflexiva:** Similar a la demostración de reflexividad anterior. Con la función identidad, como es biyectiva, es inyectiva y su inversa también, por lo que $A \preceq A$
2. **Es antisimétrica:** Con dos conjuntos $A, \ B$ tal que $A \preceq B$, sólo tenemos que la función a la que se asocia es inyectiva, pero no sobreyectiva, por lo que no es posible crear otra función sobreyectiva, por lo que $B \npreceq A$
3. **Es transitiva:** Es similar a la demo. anterior. Usando las funciones inyectivas, y creando otra función inyectiva, se demuestra que es transitiva
## Conexiones
- [[Cardinalidad]] 
- [[El conjunto de partes precede al conjunto]]
- [[Los naturales no son equipotentes a los reales]]
## Fuente / origen de la idea
---
- [[]]