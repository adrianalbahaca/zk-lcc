---
id: 202607281138
fecha: 28-07-2026
estado: completo
tags:
  - ArquiComp
---
# Infinito, NaN y cero en IEEE 754 
## La idea en una oración
---
> Debido a la representación de flotantes, los casos como el cero, infinito y `NaN` tienen partes distintas
## Desarrollo
---
En el estándar IEEE 754, se permite representar unos valores especiales usando la mantisa, exponente y signo
- `INF`: La mantisa es todo cero y el exponente es todo uno
- `NaN`: La mantisa contiene algún bit uno y el exponente es todo uno
- `0`: La mantisa, exponente y bit de signo es todo cero

Estos casos nos permiten calcular matemáticamente bien las indeterminaciones como $0 \times \infty$ o $\infty + (- \infty)$ 
## Conexiones
- [[]] 
