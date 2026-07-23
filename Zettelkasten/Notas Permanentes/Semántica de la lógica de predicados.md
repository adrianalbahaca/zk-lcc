---
id: 202607141634
fecha: 14-07-2026
estado: completo
tags:
  - Lógica
---
# Consecuencia semántica en Lógica de predicados
## La idea en una oración
---
> Debido a la variedad de modelos y entornos, demostrar una consecuencia semántica requiere usar un modelo arbitrario y concluir que vale la consecuencia
## Desarrollo
---
En lógica proposicional, nos basábamos en una valuación para verificar que una proposición fuera cierta o no, pero en lógica de predicados, no se puede asumir simplemente que los predicados son ciertos y sacar conclusiones de allí

Las variables dentro de cada fórmula son solo placeholders para ser reemplazados por términos con significado y valores concretos. Por ello, viene el concepto de un *Modelo* como universo de elementos a trabajar con ciertos significados, y un *entorno*, como función que reemplaza tales variables con elementos del modelo

Por ello, dado una signatura $(\mathcal{F}, \mathcal{P})$, un modelo y entorno $\mathcal{M}, s$ correspondientes a la signatura, y $\phi \in FORM$, la semántica se hereda de forma inductiva desde las variables, usando el entorno para asignarle valores del universo, y después usar los elementos de las fórmulas para evaluar veracidades
## Conexiones
- [[Modelo y entorno en lógica]]
- [[Sentencias]]
