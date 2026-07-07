---
id: 202603282115
fecha: 28-03-2026
estado: completo
tags:
  - CompMatI
---
# Alg. de Ford-Fulkerson 
## La idea en una oración
---
> Con un algoritmo $f$ inicial, incluyendo el nulo, se empieza a buscar caminos $f$-aumentantes y aumentándolos con la creación antes mencionada, hasta que no haya más caminos $f$ aumentantes
## Desarrollo
---
El algoritmo consiste en buscar caminos $f$-aumentantes, y aumentar el valor del flujo poco a poco hasta que no sea posible conseguir un camino de este estilo

```
Ford-Fulkerson(G: Red, f: flujo factible) {
	Etiq = []
	U = {a}
	while (U not empty) {
		while(z not in U) {
			let v in U
			for(x in N_G(v)) {
				if (propia(xv) and f(xv) < c(xv)) {
					Etiq = [Etiq (v, min(eps(v), c(xv) - f(xv)))]	
				}
				else if (impropia(xv) and f(xv) > 0) {
					Etiq = [Etiq (v, min(eps(v), f(xv)))]
				}
				U = [U x]
			}
		}
		
		if (U empty) return
		
		P = Camino desde z hasta a con Etiq
		for (f(xv) in P) {
			if (propia(xv))
				f(xv) = f(xv) + Delta
			else if (impropia(xv))
				f(xv) = f(xv) - Delta
		}
	}
}
```

Es un algoritmo laborioso que requiere redibujar el diagrama con los flujos nuevos, pero, al hacerlo bien, podemos extraer el flujo máximo el conjunto de 
vértices para el corte mínimo por el teorema Min-Cut Max-Flow
## Conexiones
- [[Creación de flujos nuevos a partir de flujos viejos]] 
