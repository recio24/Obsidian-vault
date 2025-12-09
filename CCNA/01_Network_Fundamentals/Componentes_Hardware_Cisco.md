# Componentes Hardware Cisco
---

> [!info] 
> Elementos modulares que permiten identificar y describir componentes usados comúnmente en equipos Cisco.

--- start-multi-column: ID_comp1
```column-settings
Number of Columns: 3
Largest Column: standard
```

**Chasis**
Caja o carcasa exterior del router/switch.

--- column-break ---

**Engines**
Cerebro del equipo. Procesador que ejecuta el sistema operativo.

--- column-break ---

**Tarjetas de Línea o Módulos**
Interfaces de red insertables en el chasis.

--- end-multi-column
### Módulos de Supervisión (Switches)

> [!info]
> Son el cerebro del switch. Gestionan el funcionamiento general del equipo.

**Características:**
- Utilizan ranuras distintas según modelo
- Hay varios tipos según el equipo (Nexus 7K, Catalyst 6500...)
- La instalación cambia de un equipo a otro

> [!warning] 
> Los supervisores suelen contar con puerto de consola, esto ayuda a reconocer el supervisor en nuestro equipo.


> [!info] Un equipo puede contar con uno o más. Estos son el cerebro de la máquina.

**Otro motor también cuenta con puerto de consola:**

- **NPE (Sistema de procesamiento de red)**
- **SPE (Sistema de rendimiento de servicio)**

> [!fail] Sin motor, nuestro enrutador no funcionará

---

## Tarjetas de Línea, Módulos y Adaptadores

> [!tip]
> Las **[[Cisco_Interfaces_Hardware|interfaces de red]]** están localizadas en el chasis o en tarjetas removibles. Hay varios modelos/tarjetas dependiendo del tipo de chasis.

--- start-multi-column: ID_cards1
```column-settings
Number of Columns: 2
Largest Column: standard
```

### Tarjetas de Línea
- Usadas para switches
- Abarcan todo el ancho del chasis
- **No son quitables en caliente**
- Se debe apagar para quitar o poner
- Fabricadas específicamente para cada modelo

--- column-break ---

### Módulos en Routers
- Dependiendo del router, los espacios de expansión y tamaños cambian
- Varios tipos según el proyecto
- Tamaños: pequeño, mediano, grande

**Cisco 7200**
- Espacios pequeños: Adaptadores de puerto
- Espacio grande: Controlador de entrada y salida

**Cisco 4451**
- Ranuras pequeñas: **NIMs** (Módulos de interfaz de red)
- Ranura grande: **ESM** (Módulo de servicio mejorado)

**Cisco 2611**
- Ranuras pequeñas: **[[Cisco_Interfaces_Hardware#Ubicación|WICs]]**
- Ranura grande: Módulo de red

--- end-multi-column
## Módulos de Servicio

> [!info]
> Módulo encargado de una función particular, siempre que no sea transporte de medios. Ofrecen un servicio a nuestro sistema.

**Ejemplos:**
- **FWSM:** Módulo de servicios de Firewall
- **Módulo de servicios de WLAN**
- **Módulo de servicio ASA IPS**

> [!warning] 
> No siempre deben contar con un conector, puede que solo tengan un led o varios individuales.

---

## Nomenclatura por Tamaño de Ranura

| Tamaño Ranura | Tipos de Módulos | Siglas |
| :--- | :--- | :--- |
| **Pequeñas** | WAN Interface Cards | **WICs, HWICs, VWICs** |
| **Medianas** | Adaptadores de puertos o NIM | **NIMs** |
| **Grandes** | Módulos de red, NMEs o módulos de servicios | **NMEs** |

---

**Tags:** #CCNA/Fundamentos #Hardware/Componentes #Cisco/Modular #Estado/Terminado
