---
id: 202609211337
fecha: 21-09-2026
estado: borrador
tags:
  - Comms
---
# Transmisión pasa-banda 
## La idea en una oración
---
> Empezando desde una señal en una banda de frecuencias, se altera la señal en un cierto rango para mandar información
## Desarrollo
---
Tomando una señal en banda base, se puede correr hasta una *banda de paso* para que varíe entre $S$ y $S+B$ Hz sin cambiar la información a transmitir. Luego, el receptor las pasa de vuelta a banda base para detectar los símbolos
- **ASK (Modulación por amplitud de frecuencia)**: Sigue las ideas de NRZ y NRZI pero usa dos amplitudes distintas con niveles distintos para diferenciar entre el bit 0 y bit 1
- **FSK (Modulación por desplazamiento de frecuencia)**: Sigue la idea de ASK pero usa dos frecuencias distintas para distinguir entre bits
- **PSK (Modulación por desplazamiento de fase)**: Por último, se puede rotar la fase de la frecuencia por cada símbolo
Estos esquemas pueden ser combinados y usados con más niveles para transmitir mas bits por símbolo. Un ejemplo de esto es el *QAM-16*
## Conexiones
- [[Multiplexación por división en frecuencia]] 
