---
id: 202610092101
fecha: 09-10-2026
estado: completo
tags:
  - EDyAII
---
# Modelo de Costo y paralelismo
## La idea en una oración
---
> Se enfocará en el Trabajo y Profundidad, los dos modelos de costo de la cátedra. Nuestro objetivo es aumentar el paralelismo
## Desarrollo
---
Para analizar un programa, nos enfocaremos en dos modelos de costo: El trabajo ($W$), y la profundidad ($S$)

Ahora, considere la definición de paralelismo $P = {{W}\over{S}}$. Este mide cuantos procesadores se pueden usar en un programa

Asumiendo un Scheduler voraz y baja latencia de comunicación entre componentes, se cumple el *Principio de Brent*, donde:

$$
T \le {{W}\over{p}} + S = {{W}\over{p}} + {{W}\over{S}} = {{W}\over{p}} (1 + {{p} \over {P}})
$$

Entonces, si $P \rightarrow \infty$, tenemos que ${{p}\over{P}} \rightarrow 0$, dando una cota de tiempo óptima

Nuestro objetivo es claro: **Buscamos que nuestros algoritmos sean lo más paralelizables posibles** 
## Conexiones
- [[Modelos de costo]]
- [[Costo de Divide & Conquer]]
- [[Paralelismo]]
