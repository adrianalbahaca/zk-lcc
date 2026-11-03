---
id: 202605131758
fecha: 13-05-2026
estado: borrador
tags:
  - EDyAII
---
# Estrategias para razonar sobre programas
## La idea en una oración
---
> El razonamiento de programas involucra verificar las implementaciones para que estén definidas de forma correcta
## Desarrollo
---
Razonar sobre un programa involucra verificar la especificación y demostrar propiedades sobre la especificación dada. Para ello, tenemos varias herramientas:
- **Razonamiento ecuacional:** Se despeja las ecuaciones usando las definiciones directas dadas. Acá, en caso de sacar el código de Haskell, la igualdad `=` es matemática, no solo en sentido de asignación
- **Patrones disjuntos:** Una forma de facilitar el razonamiento es usar estos patrones, para dar límites útiles en las fórmulas. Por ejemplo:
```Haskell
isCero :: Int -> Bool
isCero 0 = True
isCero n = False
-- Se añade una guarda para dar su restricción adecuada al último caso
isCeroGuarda :: Int -> Bool
isCeroGuarda 0 = True
isCeroGuarda n | n != 0 = False
```
- **Extensionalidad:** Si queremos verificar que, para dos funciones $f$ y $g$, $f = g$, se hará a partir de los argumentos de su dominio. Entonces $\forall x \in A, f(x) = g(x)$
- **Inducción sobre los naturales:** Podemos usar los naturales sobre una estructura $t$ de tal manera que el predicado a demostrar sea a base de un dato numeral de la estructura. En otras palabras, si se tiene el predicado $P(t)$, el nuevo predicado queda como:
  $Q(n) = \forall a \in A : f(a) = n \Rightarrow P(a)$
- **Inducción estructural:** La mayoría del tiempo, si la estructura está definida de forma recursiva, se puede aplicar un estilo de inducción sobre la misma estructura, tomando sus casos como el caso base y la $HI$ misma sobre los constructores recursivos
## Conexiones
- [[Principio de extensionalidad]] 
- [[Análisis por casos]]
- [[Inducción]]
- [[Inducción de naturales a programas]]
- [[Inducción estructural]]