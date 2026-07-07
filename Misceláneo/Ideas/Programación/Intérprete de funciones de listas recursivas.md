# Idea principal
---
Este fue un trabajo práctico de la universidad, que no aprobé por errores de memoria. Con el conocimiento que tengo ahora, que es más avanzado en varios archivos, quiero reescribirlo de forma que sea más óptimo, con una heurística nueva para definir el search
# Lenguaje a usar
---
```
<comando> ::= <declaracion>

<declaracion> ::= <dlist> | <dfunction> | <apply> | <search>

<dlist> ::= dlist <def> = <lista> <terminal> <terminal>
<dfunction> ::= dfunction <def> = <funcs> <rec> <funcs> <terminal>
<apply> ::= apply <func> <lista>/<def> <terminal>
<search> ::= search <lista>/<def> <lista>/<def> <terminal>

<lista> ::= [ <nums> ]
<nums> ::= <num>, <nums> | <num>

<funcs> ::= <func> <funcs> | NULL
<rec> ::= < <funcs> > | NULL
<func> ::= <def> | <prim>

<def> ::= # Definir acorde a como se define en C
<num> ::= # Numeros naturales!
<terminal> ::= ;
```
---
## Lexer: Procesamiento del comando
## Parser: AST, lenguaje formales ind. del contexto y creación adecuada
## Execute: Implementación de comandos sin error de memoria jaja
---
- Posible uso de Arenas?... **!** 