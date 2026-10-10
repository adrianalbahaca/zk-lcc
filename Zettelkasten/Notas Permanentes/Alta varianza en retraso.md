---
id: 202610091903
fecha: 09-10-2026
estado: completo
tags:
  - Comms
---
# Manejo de un retraso variable 
## La idea en una oración
---
> En casos de retrasos en la red altamente variabls, se calcula la varianza usando diferencia y pesos extra
## Desarrollo
---
En los algoritmos dados, estos no funcionan adecuadamente para redes con retrasos variables altos. Sea $\sigma = {{1}\over{1-L}}$ la varianza del tiempo de viaje, y $L$ la carga de la red, nótese que crece en proporción con la carga
Por ello, se calcula ciertos pesos más para tratar de estimar el la varianza y el tiempo de viaje, para reemplazar a $\beta$:
$$
Diff = M - RTT_v \\
RTT_s = RTT_v + \delta \times Diff \\
Dev = Dev_v + \rho \times (|Diff| - Dev_v) \\
Timeout = RTT_s + \nu \times Dev
$$
Donde $\delta, \rho, \nu$ están entre 0 y 1.
- $\delta$: Qué tan rápido la muestra afecta el *promedio con peso*
- $\rho$: Qué tan rápido la muestra afecta la *desviación media*
- $\nu$: Qué tanto afecta el desvío al timeout

Hoy en día, los pesos suelen ser la inversa de una potencia de dos, para luego escalarlos usando un número $2^n$ con $n$ apropiado. Por ejemplo: $\delta = {{1}\over{2^3}}$, $\rho = {{1}\over{2^2}}$, $n = 3$ y $\nu = 4$  
## Conexiones
- [[]] 
