---
id: 202605140831
fecha: 14-05-2026
estado: completo
tags:
  - LFyC
---
# Ejemplo del Lenguaje de Romeo 
## La idea en una oración
---
> El lenguaje de Romeo es el primer lenguaje a estudiar, que muestra cómo se produce las frases, a través de una gramática
## Desarrollo
---
Una `<frase>` de Romeo (No es que la dice, sino es que se reemplaza por lo que se puede decir) tendrá un `<sujeto>` y `<predicado>`. En el caso de Romeo, `<sujeto>` se reemplaza por `Julieta`, y `<predicado>` tendrá `eres <cuantificador> hermosa`, donde dice en el `<cuantificador>` lo fuerte que siente su amor, que puede ser `muy` una o varias veces, dependiendo de cuánto tiempo anduvo sin verla

Este es el primer ejemplo de una *gramática* para el lenguaje de Romeo

Luego, Julieta tiene que verificar que quien le esté hablando sea en realidad Romeo y no alguien más, viendo si lo que está diciendo es algo que Romeo diría o no. Ella espera cada palabra siguiente que diga Romeo. Si llega a escuchar otra cosa, se va a decepcionar. Si Romeo dice la `<frase>` correctamente, ella se va a alegrar. Ella se vuelve en una *máquina de estado*, donde el camino representa cómo se arma la frase. Si se llega al *estado de aceptación*, se sigue derecho a calcular, y sino, se avisa que hay un error sintáctico

Ambos están relacionados con una relación del $\iff$ 
## Conexiones
- [[]] 
