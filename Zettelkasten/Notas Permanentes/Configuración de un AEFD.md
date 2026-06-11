---
id: 202605141014
fecha: 14-05-2026
estado: completo
tags:
  - LFyC
---
# Def. de configuración de un AEFD
## La idea en una oración
---
> Una configuración de un AEFD es un elemento de $S \times \Sigma^*$. De allí deriva la aceptación de palabras y de un lenguaje
## Desarrollo
---
 Para $(s, \alpha)$, siendo $s$ estado del AEFD y $\alpha$ una palabra en $\Sigma ^*$, se interpreta como "Estoy en un estado $s$ y me queda $\alpha$ por leer". Cada transición entre estados se come un símbolo de $\alpha$. 
 
 El recorrido en el autómata tiene que llegar a una configuración $(s_x, \lambda)$, y de allí se mira si el estado final pertenece a $Ac$ o no para ver si una palabra está en el lenguaje verificado por el AEFD
 
 Entonces, la *ejecución de un paso* en un AEFD $A$ se define como $\Rightarrow _A:S\times\Sigma ^* \rightarrow S\times\Sigma^*$. Su ley es $(s_1, x \alpha) \Rightarrow_A (f(s_1, \alpha), \alpha)$ 

Luego, la *ejecución de 0 o más pasos* representada como $\Rightarrow _A ^*$ como la *clausura reflexiva transitiva de* $\Rightarrow_A$. Es decir:
1. $\forall s, \alpha \, (s, \alpha) \Rightarrow _A^* (s,\alpha)$
2. $\forall s,s',s'', \alpha, \alpha ', \alpha ''. \text{Si } (s, \alpha) \Rightarrow _A^* (s',\alpha') \text{ y } (s', \alpha') \Rightarrow_A^* (s'', \alpha'') \Rightarrow (s,\alpha) \Rightarrow_A^* (s'',\alpha'')$ 
## Conexiones
- [[Lenguaje de un autómata finito]] 
