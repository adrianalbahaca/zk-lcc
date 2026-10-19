---
id: 202610191226
fecha: 19-10-2026
estado: completo
tags:
  - EDyAII
---
# Costes de Divide & Conquer
## La idea en una oración
---
> El algoritmo de Divide & Conquer separa los costos de dividir el problema, resolver cada problema y combinar todo
## Desarrollo
---
**Divide & Conquer** es una de las estrategias más comúnes para resolver un problema. Sus costos se puede dividir como siguen

$$
W(n) = W_{dividir}(n) + \Sigma_{i=1}^k W(n_i) + W_{combinar}(n) \\
S(n) = S_{dividir}(n) + Max_{i=1}^k S(n_i) + S_{combinar}(n)
$$

Un ejemplo de cómo se divide los costes es en el algoritmo de *Merge Sort* de una lista, el cual divide el problema en partes y los une para obtener la lista ordenada. Si vemos el algoritmo, obtenemos para el trabajo que:

$$
W_{combinar}(n) = W_{merge}(n-1) + c_1 \\
W_{dividir}(n) = W_{dividir}(n-2) + c_2 \\
W_{MergeSort}(n) = W_{dividir}(n) + 2W_{MergeSort}(n/2) + W_{combinar}(n) + c_3\\
W_{combinar}(n) \in O(n) , W_{dividir}(n) \in O(n), W_{MergeSort}(n) \in O(n \log n)
$$

Luego, queda que la profundidad es:

$$
S_{combinar}(n) = S_{combinar}(n-1) + c_4 \\
S_{dividir}(n) = S_{dividir}(n-2) + c_5 \\
S_{MergeSort}(n) = S_{dividir}(n) + S_{MergeSort}(n/2) + S_{combinar}(n) + c_6 \\
S_{combinar}(n), S_{dividir}(n), S_{MergeSort}(n) \in O(n)
$$

Nótese que, usando listas, este algoritmo no es muy paralelizable
## Conexiones
- [[Merge Sort]]
- [[Divide and Conquer Genérico como Algoritmo]]
