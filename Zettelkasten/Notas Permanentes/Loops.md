---
id: 202607281222
fecha: 28-07-2026
estado: completo
tags:
  - ArquiComp
---
# Loops `while` y `for` 
## La idea en una oración
---
> Los loops usan un arreglo contador, saltos de línea y saltos condicionales para repetir una instrucción
## Desarrollo
---
Considere el código en C siguiente:
```C
while (x > 0) {
	/* Cuerpo */
	x--;
}
...
```
En Assembly x86-64, su código similar se ve así
```x86asm
while_loop:
	cmpl $0, %ecx
	jle fin_while_loop
	
	# Cuerpo
	decl %ecx
	jmp while_loop

fin_while_loop:
	...
```

Los loops `while` se basan en 3 conceptos: La comparación de una condición que *debe dejar de cumplirse* antes de salir, el salto indefinido al principio del loop y un registro que mantiene a cuentas esto

Por este motivo, `for` termina siendo una variante de lo anterior
```C
for (int i = 0; i < 10; i++) {
/* Cuerpo */
}
...
```
```x86asm
movl $0, %ecx
for_loop:
	cmpl $10, %ecx
	jge fin_for_loop
	
	# Cuerpo
	
	incl %ecx
	jmp for_loop

fin_for_loop:
	...
```

Y el `do-while` es otra invariante, sin el chequeo en el principio:
```C
do {
/* Cuerpo */
x--;
} while (x > 0);
...
```
```x86asm
do_while_loop:
	# Cuerpo
	
	decl %ecx
	cmpl $0 %ecx
	jge fin_do_while_loop
	jmp do_while_loop

fin_do_while_loop:
	...
```
## Conexiones
- [[]] 
