---
id: 202606252222
fecha: 25-06-2026
estado: completo
tags:
  - SistOpI
---
# Deadlock vs. Livelock 
## La idea en una oración
---
> Un Deadlock cumple las condiciones de *Hold & wait*, *No expropiación*, *Espera circular* y *Exclusión Mutua*
## Desarrollo
---
Un Deadlock es un error sutil pero grave en programación concurrente donde ninguno de los procesos pueden progresar. Para esto, necesita 4 condiciones:
- **Hold & Wait:** Un proceso debe estar reteniendo al menos un recurso, y debe de estar a la espera de otro recurso que está en posesión de otro proceso
- **No Preemption:** Ninguno de los procesos puede arrebatar los recursos a necesidad
- **Espera circular:** Debe existir un ciclo de procesos donde cada uno espera un recurso del siguiente
- **Exclusión mutua:** Existe al menos un recurso que se accede en simultáneo, donde sólo un proceso a la vez puede retenerlo

En comparación, un *Livelock* ocurre cuando los procesos no se bloquean pero no hacen ningún trabajo esperado. Esto ocurre en el problema de los filósofos
## Conexiones
- [[Problema de los filósofos]] 
