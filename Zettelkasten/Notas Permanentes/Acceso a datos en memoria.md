---
id: 202607281817
fecha: 28-07-2026
estado: completo
tags:
  - ArquiComp
---
# Acceso a memoria 
## La idea en una oración
---
> Para acceder a memoria desde una dirección, es necesario usar los paréntesis, u otras herramientas de indexación
## Desarrollo
---
El acceso a memoria como se hace en C depende de donde esté la dirección
- Considere un arreglo guardado en `.data`. Para acceder a sus datos, podemos operar sobre la etiqueta misma, sumando y multiplicando valores. Esto se le conoce como *direccionamiento inmediato*
```x86asm
.data
	a: .long 1 2 3 4 5
.text
.global main
main:
	movl a+2*4, %eax # Guarda 4 bytes desde la dirección a más 2 por 4
	# Esto es el equivalente a guardar a[2]
```
- Considere una llamada a función tal que `%rdi` tiene la dirección de un arreglo de enteros. Entonces, se puede encerrar en paréntesis para guardar las cosas en la dirección apuntada. Esto lleva a *direccionamiento indirecto*, *direccionamiento indexado*, *direccionamiento relativo*
```x86asm
.global sum # sum (int *a)
	movl (%rdi), %rax # Mover 4 bytes desde la dirección dada en %rdi
	movl 4(%rdi), %rbx # Mover 4 bytes desde la dirección dada en %rdi más 4
	movq %rdx, $3
	movl (%rdi, %rdx, 4), %rcx # Mover 4 bytes desde la dirección dada en %rdi más el valor en %rdx por 4
	# Este es el equivalente a a[3] 
```
## Conexiones
- [[]] 
