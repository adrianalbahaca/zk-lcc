---
id: 202605231941
fecha: 23-05-2026
estado: borrador
tags:
  - Lógica
---
# Def. y uso del Teorema de Sustitución 
## La idea en una oración
---
> El teorema de sustitución permite crear resultados generales a partir de casos particulares
## Desarrollo
---
Formalmente, lo define de esta forma:
> Sean $\phi_1, \phi_2, \lambda \in PROP, p_i \in AT$ . Si $\vDash \phi_1 \iff \phi_2$, entonces $\vDash \phi_1[\lambda/p_i] \iff \phi_2[\lambda/p_i]$ 

*Ej:* Sabiendo que $\vDash p \rightarrow p$ es tautología, entonces, usando $p \wedge q$ y este teorema, podemos concluir que $\vDash (p \wedge q) \rightarrow (p \wedge q)$ 
## Conexiones
- [[]] 
