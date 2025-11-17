## Estructura de un PLC
---
>[!info] **Resumen**
La estructura de un PLC se compone de una fuente de alimentación, una CPU con memoria, módulos de entradas y salidas (digitales y analógicas), unidades de programación y módulos especiales. Puede ser compacto o modular según la aplicación.

### Estructura física
--- start-multi-column: ID_ldjz
```column-settings
Number of Columns: 2
Largest Column: standard
```

**Estructura compacta**
- Todo integrado: CPU + alimentación + E/S
- No ampliable
- Económica
- Para máquinas simples
- Pocas entradas y salidas

--- column-break ---

**Estructura modular**
- Cada módulo es independiente
- Muy ampliable (CPU, E/S, comunicaciones…)
- Ideal para procesos complejos
- Mayor capacidad y flexibilidad

--- end-multi-column
### Componentes principales
**Fuente de alimentación**
- Adapta 230/110 V AC → 24 V DC / 5 V DC  
- Alimenta CPU y módulos  
- Puede incluir batería para mantener memoria  
- Se identifica por potencia y tipo de tensión
**CPU**
- Interpreta el programa del usuario  
- Lee entradas → ejecuta lógica → actualiza salidas  
- Realiza operacionexxwws internas: contadores, temporizadores, matemáticas… 
- Puede tener procesador doble según la gama
**Memoria del PLC**

| Memoria | Borrado   | Mantiene sin tensión | Uso                          |
| ------- | --------- | -------------------- | ---------------------------- |
| RAM     | Eléctrico | NO                   | Variables, programa temporsl |
| ROM     | NO        | ibSi                 | Sistema interno              |
| FLASH   | Rlrctrico | Si                   | Programa permanente          |

