---
id: 202605231836
fecha: 23-05-2026
estado: completo
tags:
  - Lógica
---
# Def. de Sustitución 
## La idea en una oración
---
> La sustitución añade un condicional a una proposición, reemplazándola al detectar una proposición lógica en su largo
## Desarrollo
---
Se define de forma inductiva como sigue:
- $\bot [\phi / p_i] = \bot$
- $p_j [\phi/p_i] = \begin{cases} \phi \text{ si } i = j \\ p_j \text{ sino} \end{cases}$ 
- $(\phi \square \mu)[\lambda / p_i] = (\phi [\lambda / p_i]) \square (\mu [\lambda /p_i])$ 
- $(\neg \phi)[\lambda/p_i] = \neg (\phi [\lambda/p_i])$ 

La sustitución es una herramienta a usar cuando queremos dar resultado generales de resultados concretos. Esto se debe al *Teorema de Sustitución*
## Conexiones
- [[Teorema de Sustitución en Lógica Proposicional]]
- [[Consecuencia semántica]]
