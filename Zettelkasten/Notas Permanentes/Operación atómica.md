---
id: 202605112201
fecha: 11-05-2026
estado: completo
tags:
  - SistOpI
---
# Op. Atómica vs. Mutex
## La idea en una oración
---
> Una operación atómica es una acción indivisible que se ejecuta completo o no se ejecuta. Comparado a usar herramientas de Mutex, las op. atómicas reducen la sobrecarga de bloqueos
## Desarrollo
---
A pesar de que los métodos de exclusión mutua tradicionales son muy útiles, también vienen con un cierto costo de computación, ya sea al usar algoritmos o al usar las operaciones de Mutex en C

Por eso, para ciertas variables, puede ser mejor definirlas como *operaciones atómicas*, ya que así se garantiza que, al solicitar una instrucción, o se ejecuta completamente o no se ejecuta por completo. No hay intermedios

De esta manera, se evita sobrecargar el procesamiento de bloqueos, resultando en un programa más eficiente 
## Conexiones
- [[Operaciones atómicas en C]] 
