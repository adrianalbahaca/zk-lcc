---
id: 202607281148
fecha: 28-07-2026
estado: borrador | completo | pendiente
tags:
  - ArquiComp
---
# `if else` de C a Assembly
## La idea en una oración
---
> Los condicionales usan los saltos condicionales de Assembly para ir de una línea de código a otra 
## Desarrollo
---
Si se tiene en C el siguiente código
```C
if (a != 2) {
	b = true
}
else {
	b = false
}
```
El compilador lo traduce a Assembly de la siguiente forma
```x86asm
# Asumiendo que el valor está guardado en %eax

cmpl $2, %eax
jeq rama_true # Parte si es cierto
jmp rama_false # Parte si es falso

rama_true:
	movl $0, %ebx
	jmp cont

rama_false:
	movl $1, %ebx
	jmp cont
	
cont:
	...
```

En Assembly, hay múltiples saltos que se pueden hacer cuando se hace comparaciones. Algunos ejemplos son los siguientes:
- Igualdad: `je (==), jne (!=)`
- Desigualdad en `signed`: `jge (>=), jle (<=), jg (>), jl (<)`
- Desigualdad en `unsigned`: `jae (>=), jbe (<=), ja (>), jb (<)`
## Conexiones
- [[]] 
