---
id: 202609211152
fecha: 21-09-2026
estado: borrador
tags:
  - Comms
---
# Non-Return-to-Zero 
## La idea en una oración
---
> Un voltaje positivo es 1 y un voltaje negativo es 0. Es simple, pero su ancho de banda es algo alto y manda poca info
## Desarrollo
---
El NRZ consiste en usar un voltaje positivo para el bit 1 y un voltaje negativo para el bit 0. Este sistema es bastante simple, pero debido a que la señal se distorsiona, puede verse complicado diferenciar entre los dos
Suele combinarse con *niveles de señalización*, donde cada nivel es un *símbolo* y representa una cierta cantidad de bits. Tiene una tasa de bits por segundo más alta pero, en la distorsión, los niveles pueden ser confundidos
Por ejemplo, en el WiFi, usando NZR con niveles, se puede aumentar la cantidad de niveles cuando el receptor esté cerca, y reducirla cuando esté lejos. De esta forma, se adapta la cantidad de información a transmitir sin aumentar la potencia del transmisor o receptor
## Conexiones
- [[]] 
