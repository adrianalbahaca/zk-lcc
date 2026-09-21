---
id: 202609031557
fecha: 03-09-2026
estado: borrador
tags:
  - Comms
---
# Serie de Fourier y sus implicancias 
## La idea en una oración
---
> La serie de Fourier permite construir cualquier función de comportamiento razonable con una suma finita o infinita de senos y cosenos
## Desarrollo
---
La serie de Fourier permite construir funciones periódicas con una suma finita o infinita de senos y cosenos como sigue:

$$f(t) = {\displaystyle {\frac {a_{0}}{2}}+\sum _{n=1}^{\infty }\left[a_{n}\cos {\frac {2n\pi }{T}}t+b_{n}\operatorname {sen} {\frac {2n\pi }{T}}t\right]}$$
Tenemos que $a_n, b_n$ son las *amplitudes del n-ésimo armónico*, y donde $f = {{1}\over{T}}$ es la *frecuencia fundamental*

$${\displaystyle a_{0}={\frac {2}{T}}\int _{-T/2}^{T/2}f(t)dt,\qquad a_{n}={\frac {2}{T}}\int _{-T/2}^{T/2}f(t)\cos \left({\frac {2n\pi }{T}}t\right)dt,\qquad b_{n}={\frac {2}{T}}\int _{-T/2}^{T/2}f(t)\operatorname {sen} \left({\frac {2n\pi }{T}}t\right)dt.}$$

## Conexiones
- [[]] 
