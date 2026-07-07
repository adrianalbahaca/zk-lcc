---
id: 202603211857
fecha: 21-03-2026
estado: borrador
tags:
  - SistOpI
---
# Def. de Signal y usos
## La idea en una oración
---
> Un *Signal* es un entero que se suele enviar entre procesos. Los procesos pueden actuar acorde a las señales enviadas o recibidas
## Desarrollo
---
Uno de los mecanismos que Linux usa son los *Signals*, señales con significados especiales que un proceso puede recibir para, después, manejarlo acorde. Antes, cuando no había pantallas, las señales usando la tecla `Ctrl` permitía enviar señales al dispositivo para pausar, interrumpir y/o derramar el core, dependiendo de su comportamiento predeterminado
Piénsalo como una notificación asíncrona que el proceso debe de gestionar
## Conexiones
- [[Envío de signals]]
- [[Recepción y manejo de signals]]
