# Generación de Rutas Seguras en Entornos Dinámicos

## Problema

En los sistemas de transporte modernos y los entornos urbanos, garantizar la seguridad y eficiencia de las rutas de movilidad representa uno de los mayores desafíos. Esta tarea se complica aún más en entornos dinámicos, donde factores como el tráfico, las condiciones meteorológicas y eventos inesperados pueden cambiar rápidamente. Este proyecto aborda el problema de generar rutas seguras en estos escenarios, con un enfoque especial en la adaptabilidad a condiciones que varían en tiempo real.

## Formalización

El sistema de rutas se modela como un **grafo dinámico** $G = (V, E)$, donde:

- **V** : Nodos que representan puntos de interés, como intersecciones o ubicaciones específicas.
- **E** : Aristas que conectan los nodos, cada una con un peso dinámico $w(u,v)$, que indica el nivel de riesgo asociado a esa conexión.

El peso $w(u,v)$ incorpora tanto factores estáticos (distancia, historial de accidentes) como condiciones dinámicas (tráfico en tiempo real, clima, accidentes o bloqueos). 

El objetivo principal es encontrar la **ruta más segura** desde un nodo de origen **s** hasta un nodo de destino **t**, minimizando el riesgo acumulado en el trayecto. Además, se busca que el sistema pueda adaptarse rápidamente a cambios en el entorno mediante la **replanificación de rutas en tiempo real**.

El proyecto también considera restricciones adicionales relevantes en escenarios reales, como limitar la duración de las rutas o evitar zonas de alto riesgo.

