---
id: 202609211745
fecha: 21-09-2026
estado: borrador
tags:
  - Comms
---
# Multiplexación por división de código 
## La idea en una oración
---
> Usando vectores de chips internos entre el transmisor y el receptor, se envía una señal que el receptor calcula con su vector interno para obtener su bit
## Desarrollo
---
Esta multiplexación permite usar todo el ancho de banda por usuario. Se le da a cada uno una *secuencia de chips*, un vector, donde entre cada usuario su vector es ortogonal (Esto se puede calcular con los *códigos de Walsh*). Luego, el transmisor transmite la señal, haciendo que la suma de los transmisores de forma lineal den un voltaje que, al calcular, den el resultado final, usando el producto interno de los chips transmitidos para obtener el resultado
Acá entra el producto entre vectores al enviar las señales
## Conexiones
- [[]] 
