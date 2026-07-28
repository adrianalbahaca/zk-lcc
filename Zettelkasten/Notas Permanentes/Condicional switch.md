---
id: 202607281242
fecha: 28-07-2026
estado: completo
tags:
  - ArquiComp
  - Compiladores
---
# `switch` y por qué es tan veloz
## La idea en una oración
---
> `switch` es un condicional especial que usa una tabla de direcciones para hacer los saltos hacia las condiciones dadas
## Desarrollo
---
La velocidad de switch viene por el hecho de que salta inmediatamente a la línea con la condición dada usando una *jump table* hecha previamente
```C
switch (x) {
	case 1:
		/* A */
		break;
	case 2:
		/* B */
		break:
	default:
		/* C */
		break;
}
...
```
```x86asm
.data
	tabla_saltos:
		.quad case_1
		.quad case_2
...

movq $1, %rax # Considera que se tiene que indexar el registro acorde para usar la tabla bien

cmpq $LIMITE, %rax
jg default
jmp *tabla_saltos(,%rax, 8) # 1*8 = case_2

case_1:
	# A
	jmp fin_switch

case_2:
	# B
	jmp fin_switch

default:
	# C
	jmp fin_switch

fin_switch:
...
```
## Conexiones
- [[]] 
