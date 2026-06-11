---
id: 202605211023
fecha: 21-05-2026
estado: borrador
tags:
  - LFyC
---
# Lenguaje de las $ER$ 
## La idea en una oración
---
> Se define formalmente el lenguaje descrito por una expresión regular para notar que es regular
## Desarrollo
---
> El lenguaje descrito por una expresión regular se define como $L: ER \rightarrow P(\Sigma^*)$ y tiene las siguientes características
> 	- $L( \emptyset ) = \emptyset$
> 	- $L( \lambda ) = \{ \lambda \}$
> 	- $L(x) = \{ x \}$
> 	- $L(\alpha \beta) = L(\alpha) L(\beta)$
> 	- $L(\alpha + \beta) = L(\alpha) \cup L(\beta)$ 
> 	- $L(\alpha^*) = (L(\alpha))^*$ 

Con esta definición recursiva, se puede demostrar que los lenguajes representados por un AEFD se pueden representar como una expresión regular. Es ladilla la demo. pero súper útil
## Conexiones
- [[Relación entre AEFD y expresiones regulares]] 
