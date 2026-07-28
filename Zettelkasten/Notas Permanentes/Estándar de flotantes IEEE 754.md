---
id: 202607251736
fecha: 25-07-2026
estado: pendiente
tags:
  - ArquiComp
---
# Estándar IEEE 754 para números flotantes
## La idea en una oración
---
> El estándar IEEE 754 es el más usado para representar números flotantes. Anota el número en notación científica normalizada y guarda su bit de signo, su exponente y su mantisa 
## Desarrollo
---
Para evitar tener múltiples formas de representar un número flotante, se creó el Estándar IEEE 754, el cual representa el número en binario así:
$$
fl(x) = (-1)^s \times (1.m) \times 2^e
$$
Donde $s$ es el bit de signo, $m$ es la mantisa a guardar y $e$ es el exponente sesgado, el cual se calcula como sigue
$$
e = E - sesgo
$$
Ahora, hay 3 precisiones. En todas, el primer bit se reserva como el bit de signo
- Simple: 8 bits para el exponente, 23 bits para la mantisa
- Doble: 11 bits para el exponente, 52 bits para la mantisa
- Cuádruple: (Completar)
## Conexiones
- [[Patrones especiales de IEEE 754]] 
