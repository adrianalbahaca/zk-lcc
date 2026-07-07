---
id: 202605122128
fecha: 12-05-2026
estado: borrador
tags:
  - PyE
---
# Def. y caract. de la FDA
## La idea en una oración
---
> La función de distribución acumulada es el cálculo de la integral de la f.d.p desde el $-\infty$ hasta un valor $a$ en la función
## Desarrollo
---
Considerando la probabilidad pedida como $P(X \le a)$, que puede ser esencial para tener las probabilidades de que una variable de menor o igual a $a$, se calcula la integral $\int_{-\infty}^{a} f(x)\,dx$. Esto se le conoce como la *función de distribución acumulada*

En el caso de variables discretas, se representa como $\Sigma _{u \le x} f(x)$, la suma de las probabilidades anteriores hasta $x$ inclusive 

Es esencial para determinar el comportamiento completo de los datos y, en variables aleatorias continuas, es absolutamente continua, lo que permite calcular la probabilidad de un rango como sigue:
$$P[a \le x \le b] = \int_{a}^{b}f(x)\,dx= \int_{-\infty}^{b}f(x)\,dx - \int_{-\infty}^{a}f(x)\,dx = F(b) - F(a)$$
También, tienen ciertas propiedades:
- $0 \le F(x) \le 1$ 
- $\lim_{x\rightarrow \infty} F(x) = 1$
- $\lim_{x\rightarrow -\infty} F(x) = 0$ 
- $a \le b \Rightarrow F(a) \le F(b)$ , Es monótona no decreciente
- $lim_{x\rightarrow a^+}F(x) = F(a^+)$  , Es continua por derecha
## Conexiones
- [[Función de densidad de probabilidad]] 
