---
id: 202605211015
fecha: 21-05-2026
estado: borrador
tags:
  - LFyC
---
# Def. y uso de expresiones regulares 
## La idea en una oración
---
> Las expresiones regulares son elementos prácticos para describir un lenguaje
## Desarrollo
---
> Sea un $\Sigma$ alfabeto, una expresión regular se define de forma inductiva como:
	- $\emptyset \in ER$
	- $\lambda \in ER$
	- $a \in \Sigma \Rightarrow a \in ER$
	- $\alpha, \beta \in ER \Rightarrow (\alpha \beta) \in ER$
	- $\alpha, \beta \in ER \Rightarrow (\alpha + \beta) \in ER$
	- $\alpha \in ER \Rightarrow \alpha^* \in ER \text{ , (Representa } \lambda, \alpha, \alpha \alpha, \alpha \alpha \alpha, ...)$
	- (Opcional) $\alpha \in ER \Rightarrow \alpha^{+} \in ER \text{  (Representa } \alpha, \alpha \alpha, \alpha \alpha \alpha)$


## Conexiones
- [[Relación entre expresiones regulares y AEFND epsilon]]
- [[Lenguaje descrito por expresiones regulares]]
