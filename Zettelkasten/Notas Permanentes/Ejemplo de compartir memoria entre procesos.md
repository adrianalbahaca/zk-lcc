---
id: 202605031806
fecha: 03-05-2026
estado: completo
tags:
  - SistOpI
---
# `mmap`: Designar memoria entre procesos
## La idea en una oración
---
> `mmap` es una función que permite alocar memoria virtual para los procesos entre sí
## Desarrollo
---
Para que dos procesos compartan memoria en vez de enviarse cosas, se puede alocar un espacio de memoria virtual entre los procesos de un cierto tamaño usando `mmap`, el cual se le tiene que dar un tamaño, sitio de principio, banderas y características, y offset

```C
#include <sys/mman.h>
#include <unistd.h>
#include <stdio.h>

// Ej. de dos procesos compartiendo memoria para un número
int main() {
    // Crear memoria compartida entre padre e hijo
    int *shared = mmap(NULL, sizeof(int),
                       PROT_READ | PROT_WRITE,
                       MAP_SHARED | MAP_ANONYMOUS,
                       -1, 0);

    *shared = 0;

    if (fork() == 0) {
        // Hijo: modifica la memoria compartida
        *shared = 42;
        _exit(0);
    }

    wait(NULL);
    // Padre: ve el cambio del hijo
    printf("Valor: %d\n", *shared); // imprime 42

    munmap(shared, sizeof(int));
    return 0;
}
```
## Conexiones
- [[]] 
