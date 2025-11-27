# Topologias de red
---
> [!info] 
> Una topología de red describe cómo están organizados y conectados los dispositivos en una red. Incluye topología física, topología lógica y los modelos de diseño LAN como el jerárquico de 2 y 3 capas.
## ¿Que es una topología?
La **topología** es la forma en la que se diseñan y conectan las redes. Se divide en:
- **Topología física**: Como están conectados los dispositivos fisicamente (cables, fibra, switches).
- **Topología lógica**: Como fluye el tráfico realmente (VLANs, STP, rutas, broascast domains).
## Modelos de diseño LAN
Un modelo de diseño LAN es una forma estructurada de organizar la red interna de una empresa. Cisco propone modelos con capas para separar funciones, mejorar rendimiento y facilitar el crecimiento de la red. Los beneficios son:
- Escalabilidad
- Redundancia 
- Estabilidad
- Fácil solución de problemas
- Aislamiento de fallos
- Estandarización
### Modelo de 3 capas (Jerarquico)

--- start-multi-column: ID_x03n
```column-settings
Number of Columns: 3
Largest Column: standard
```

**Core**
- Alta velocidad y baja latencia
- Grandes volúmenes de trabajo
- Totalmente redundante
- Sin políticas pesadas (No [[Network_conceptos#^4dadad|ACLs]] complejas)

--- column-break ---



--- column-break ---



--- end-multi-column

