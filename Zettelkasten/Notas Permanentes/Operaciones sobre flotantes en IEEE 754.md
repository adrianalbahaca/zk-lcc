---
id: 202608051823
fecha: 05-08-2026
estado: completo
tags:
  - ArquiComp
---
# Suma, resta, mult. y div. en flotantes IEEE 754
## La idea en una oración
---
> Para operar, se extrae el valor normalizado de la mantisa, se opera sobre las mantisas, se actualiza el exponente sesgado y se guarda el número otra vez
## Desarrollo
---
El proceso de operar sobre flotantes se simplifica a lo siguiente
1. Extraer los números flotantes a operar, representandolos en su forma normalizada, con su base y signo. Recuerda considerar el signo y el exponente
2. Luego, si es necesario, igualar exponentes. Si ocurre que la resta entre exponentes supera a los bits de la mantisa, entonces el resultado es el mayor argumento
3. Sino, se opera sobre los elementos con exponentes iguales
4. Finalmente, se mueve el exponente hasta que el resultado tenga la forma $1.f$ y se convierte de vuelta a flotante
## Conexiones
- [[]] 
