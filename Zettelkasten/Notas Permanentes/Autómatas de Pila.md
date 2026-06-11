---
id: 202606050815
fecha: 05-06-2026
estado: borrador
tags:
  - LFyC
---
# Def. del autómata de pila
## La idea en una oración
---
> Un autómata de pila es una tupla $(S, \Sigma, \Delta, T, \sigma, Ac)$ tal que $S$ es un conjunto finito de estados, $\Sigma$ es el conjunto finito de símbolos de entrada, $\Delta$ es el conjunto finito de símbolos de la  pila, $T \subseteq S \times (\Sigma \cup \{ \lambda \}) \times (\Delta \cup \{ \lambda \}) \times (\Delta \cup \{ \lambda \}) \times S$ es una relación de transición, $\sigma \in S$ es el estado inicial, $Ac \subseteq S$ es un conjunto de estados de aceptación
## Desarrollo
---
El autómata de pila permite tener algún estilo de "memoria" que los autómatas AEF no tienen. Se considera una generalización de los AEFND, haciéndolos *no deterministas*

Se puede imaginar como si la máquina recibe una cinta, con un indicador de estado y una pila interna. Mientras lee cada carácter, puede cambiar el estado o no, y almacenar el carácter en la pila (`push`), sacar un elemento (`pop`), o no hacer nada

Los símbolos almacenados en la pila no son necesariamente los del alfabeto de entrada. Hay unos símbolos más, como marcadores internos (Ejemplo: $\#$ como indicador de la base de la pila, $S$ para determinar secciones)

Las transiciones del autómata son: $\sigma$ como *estado actual*, $\chi$ como *símbolo del alfabeto que se lee en la entrada*, $\alpha$ como *símbolo a extraer de la pila*, $\beta$ como *símbolo a insertar en la pila*, $\tau$ como *estado al cual se va*. $\lambda$ en alguno de estos espacios implica que no se hace tal acción.

> Por ejemplo, la transición de $a$ a $b$ con el movimiento $\lambda, \lambda, \#$ no saca nada y recibe un carácter nulo, pero inserta el numeral. Este suele ser comienzo de este autómata

*El conjunto de todos los autómatas de pila es infinito numerable*, ya que se puede representar como $AP = \cup_{n\in \mathbb{N}} AP_n$ donde $n$ es la cantidad de estados del autómata. Esto ya nos indica que hay lenguajes que no pueden ser aceptados por un autómata de pila
## Conexiones
- [[Gramática independiente del contexto]] 
- [[Pila]]
- [[AEFND a autómata de pila]]
- [[Configuración de un autómata de pila]]
- [[Lema del bombeo en lenguajes independientes de contexto]]
