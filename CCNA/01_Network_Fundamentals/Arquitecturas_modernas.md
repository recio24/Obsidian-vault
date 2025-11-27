# Arquitecturas Modernas

> [!info]
> Las arquitecturas modernas de red se utilizan para aumentar escalabilidad, reducir complejidad y mejorar el rendimiento.  
> Incluyen modelos como **Spine–Leaf**, redes **SOHO** y conceptos de **Cloud vs On-Premise**.

## Arquitectura Spine–Leaf

> [!info]
> Usada principalmente en **centros de datos**.  
> Permite caminos de igual coste, baja latencia y una escalabilidad horizontal muy alta.

--- start-multi-column: ID_m61q
```column-settings
Number of Columns: 2
Largest Column: standard
```

**Cómo funciona**

- Los **Leaf** se conectan a _todos_ los **Spine**
- Los **Leaf NO se conectan entre sí**
- Los **Spine NO se conectan entre sí**
- Cada servidor se conecta a un Leaf
- Añadir un Leaf añade capacidad automáticamente

--- column-break ---



--- end-multi-column

