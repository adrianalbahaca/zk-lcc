---
id: 202605131504
fecha: 13-05-2026
estado: borrador
tags:
  - PyE
---
# Def. de dist. normal 
## La idea en una oración
---
> La distribución normal es una dist. observada en la naturaleza. Se asocia a la binomial cuando $n$ tiende a infinito
## Desarrollo
---
Esta probabilidad nace de ver qué es lo que pasa cuando se tiene la dist. binomial $Bi(n,p)$ cuando $n$ crece. Fue creada ya que fue observada mucho en la naturaleza, y que, a pesar de que no se puede calcular con integrales de forma directa, se puede aproximar con valores en una tabla

Se representa como $X \sim N(\mu, \sigma ^2)$ y la f.d.p está determinada como:
$$
f(x) = {{1} \over {\sqrt{2 \pi} \sigma}} e^{{-{1\over2}}({{x-\mu}\over{\sigma}})^2}
$$
Donde se tiene que satisfacer $-\infty < \mu < \infty$ y $\sigma > 0$
- Es simétrica alrededor de la esperanza $\mu$ 
- Tiene forma de campana con punto de inflexión $\mu +- \sigma$
- Mientras más cerca de $\mu$, más grande la densidad. Se ve por el pico de la población

En el caso de que $Z \sim N(0,1)$, es *normal estandarizada*, y es la que está tabulada acorde, luego, para $Z \sim N(\mu,\sigma)$, lo pasamos a $X \sim N(0,1)$ como sigue: 
$$
X = {{Z-\mu}\over{\sqrt{\sigma ^2}}}
$$

Importante: Percentiles acá
## Conexiones
- [[Distribución Binomial]] 
- [[Regla 68-95-99.7]]
- [[De dist. normal a normal estandarizada]]
