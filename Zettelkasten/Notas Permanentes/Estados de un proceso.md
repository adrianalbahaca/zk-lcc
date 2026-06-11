---
id: 202603192111
fecha: 19-03-2026
estado: borrador
tags:
  - SistOpI
---
# Múltiples estados para el proceso
## La idea en una oración
---
> Un proceso puede estar *nuevo, listo, en ejecución, bloqueado, terminado o Zombie* 
## Desarrollo
---
Un proceso puede estar en alguno de los 6 estados
1. **Nuevo:** Se ha hecho la solicitud al SO para que asigne recursos al estado
2. **Listo:** Una vez los recursos están listos, se espera al procesador para que se ejecute el proceso
3. **En ejecución:** El proceso estaría ejecutándose en ese momento
4. **Bloqueado:** El proceso se detuvo y espera a un evento para continuar
5. **Terminado:** El proceso finaliza sus instrucciones y espera que el SO lo elimine
6. **Zombie:** El proceso termina pero el SO tiene que hacer algunas tareas extra antes de eliminarlo, como liberar memoria, cerrar conexiones, y cosas así
## Conexiones
- [[]] 
