# Cableado de Cisco
---
>[!info] Definición
>El cableado de red es el medio físico que permite la transmisión de datos entre dispositivos. Incluye cables de cobre, fibra óptica y diferentes estándares según la aplicación.

## ¿Cuánto cableado debemos planificar?

Para reconocer un cable de redes de Cisco necesitamos:
- **Reconocer el tipo de cable diferente** según su aplicación
- **Los cables contienen muchos tipos y factores de forma** que se deben reconocer
- **Comprar o reemplazar un cable**, conociendo el tipo, conector, sección...

---
## Diferencia entre cobre y fibra óptica

--- start-multi-column: ID_cobre_vs_fibra
```column-settings
Number of Columns: 2
Largest Column: standard
```

### Cable de Cobre
- Más barato
- Transmite electricidad
- Distancia: hasta 100m
- Sujeto a interferencias (EMI)
- Usado en LANs

--- column-break ---

### Fibra Óptica
- Más caro
- Transmite luz (filamento de vidrio)
- Distancia: hasta 100+ km
- Inmune a interferencias
- Usado en WANs y Data Centers

--- end-multi-column

---
## Cables de redes comunes

Los tipos principales de cables que encontraremos en redes Cisco son:
- **Cobre** (par trenzado)
- **Fibra óptica**
- **Coaxial**
- **Seriales**
- **Console**

### Cable de Cobre par tenzado

Los cables de cobre tienen varias características importantes:
- **Más barato** que el cable de fibra
- **Se usa para transmitir cargas eléctricas** mediante hilos de cobre (como un carril)
- **Múltiples hilos trenzados**: Los pares están trenzados entre sí para evitar interferencias electromagnéticas (EMI)
- Se utiliza en redes [[Network_conceptos#^a80a01|LAN]] para distancias de hasta 100 metros

>[!tip] Vista del receptor
>Viendo el receptáculo o puerto al que debe ir el cable, NO dará una pista sobre qué tipo de cable debe usarse. 
>**RJ45** por ejemplo acepta cable de cobre.
>**SFP** por ejemplo acepta fibra óptica.

![[SFP con RJ45.png]]

--- start-multi-column: ID_caracteristicas_cobre
```column-settings
Number of Columns: 2
Largest Column: standard
```

**Ventajas**
- Más barato que la fibra
- Fácil instalación
- Compatible con [[PoE (Power of ethernet)|PoE]]
- Amplia disponibilidad

--- column-break ---

**Limitaciones**
- Distancia máxima: 100 metros
- Susceptible a EMI
- Menor ancho de banda vs fibra
- Requiere blindaje en entornos ruidosos

--- end-multi-column

**Principales usos:**
- **Coaxiales**: Redes antiguas y televisión
- **Ethernet**: Conexiones [[Network_conceptos#^a80a01|LAN]]
- **Cables seriales**: Conexiones [[Network_conceptos#WAN|WAN]] (múltiples pines)
### Ethernet

Los cables ethernet **originales eran coaxiales**. Con el tiempo existió evolución  ha los que conocemos ahora. Los cables de ethernet son normalmente de **pares trenzados**. Un par de hilos forman un loop completo. Los pares están retorcidos entre sí para cancelar el EMI (Interferencias electromagnéticas). Un gigabit ethernet necesita **4-8 pares de cables**.

>[!info] Transmisión de datos
>Cada par de cables trabaja en conjunto para transmitir y recibir datos. En un cable ethernet estándar:
>- **Par 1 (Wire 1, Par 1)**: Transmisor ↔ Receptor
>- **Par 2 (Wire 2, Par 1)**: Transmisor ↔ Receptor

![[Cable de pares trenzados.png]]
### Clasificación de cables ethernet

Los cables de pares trenzados pueden venir en dos variantes:

--- start-multi-column: ID_cable_tipos
```column-settings
Number of Columns: 2
Largest Column: standard
```

**Cable Directo (Straight-Through)**
- El orden de los colores sigue igual en ambos extremos
- Sirve para conectar **dispositivos en distinta capa**
- Ejemplos de uso:
	- PC → Switch
	- Switch → Router
	- PC → Router

--- column-break ---

**Cable Cruzado (Crossover)**
- Se cruza el cable 1 ↔ 3, y el cable 2 ↔ 6
- Se usa al conectar **dispositivos de la misma capa**
- Ejemplos de uso:
	- Router → Router
	- Switch → Switch
	- PC → PC

--- end-multi-column

![[Cable ethernet normal vs cruzado.png]]

>[!tip] MDI-X (Auto-detect)
>Existen dispositivos con interfaces automáticas **MDI-X**, esto detecta el tipo de cable y lo tiene en cuenta automáticamente. Por ejemplo, dos switches modernos conectados con cable directo funcionarán sin problemas.


Además, también se dividen los cables por categorías. Cuanto mayor categoría, más pares de hilos por centímetro y más protección de la vaina. Las categorías son diseños para distinguir unos de otros. A mayor categoría, mayor capacidad de velocidad en el cable.
![[Cats.png]]

>[!warning] Ojo con la distancia
>Aunque Cat 6 soporta 10 Gbps, solo lo hace hasta **55 metros**. Para los 100 metros completos a 10 Gbps necesitas **Cat 6a** o superior.


Por otro lado, podemos encontrar cables **sin blindar (UTP)** o **blindados (STP)**.

--- start-multi-column: ID_utp_stp
```column-settings
Number of Columns: 2
Largest Column: standard
```

**UTP (Unshielded Twisted Pair)**
- Sin blindaje
- Más económico
- Suficiente para la mayoría de entornos
- Usado en oficinas estándar

--- column-break ---

**STP (Shielded Twisted Pair)**
- Con capa blindada (general o por par)
- Mejora resistencia a EMI
- Recomendado en:
	- Fábricas
	- Junto a líneas eléctricas
	- Entornos con mucha interferencia

--- end-multi-column

---
## Cable Coaxial

Formado por un único hilo de cobre, parecido al cable de televisión. Es mejor previniendo interferencias electromagnéticas al contar con un aislamiento muy grueso.

**Estructura del cable coaxial:**
1. **Hilo de cobre** (centro) - Conductor principal
2. **Aislante** (Aislamiento) - Dieléctrico
3. **Malla de cobre** - Blindaje
4. **Cubierta exterior** - Protección

![[capas coaxial.png]]

Siendo mucho más grueso que el cable de pares trenzados. También tiene la posibilidad de transmitir señal mucho más lejos que el par trenzado. Utiliza conectores **BNC** (se puede conectar en conexiones de modem).

>[!info] Uso histórico
>Los cables coaxiales fueron muy utilizados en redes antiguas (10BASE2, 10BASE5) y aún se usan para:
>- Televisión por cable
>- Internet por cable (DOCSIS)
>- Conexiones de módem antiguas

---
## Cables de consola y puertos auxiliares

Estos puertos normalmente trabajan usando conectores con **RJ45**.

Estos conectores necesitan adicionar cables entrelazados los cuales se conectan en la inversa del otro extremo, mandándolo a espejo. Normalmente será un cable **azul claro** (flat/rollover), en un extremo será un **RJ45** y en el otro un **DB9**, que se puede conectar por un adaptador **USB o Serie**.

>[!tip] Cable Rollover
>El cable de consola es un tipo especial llamado "rollover" o "rolled cable". El pin 1 se conecta al pin 8, el pin 2 al pin 7, y así sucesivamente. Es fácil de reconocer por su **color azul claro**.
![[Cable konsola.png]]

**Uso principal:**
- Configuración inicial de routers y switches
- Recuperación de contraseñas
- Acceso a modo de emergencia
- Gestión local del dispositivo

---
## Cables Seriales

Los cables seriales son de **cobre** y existen muchos factores de forma diferentes. Para saber qué cable serie necesitamos debemos:
- Saber si el router va a ir conectado a un terminal **DTE** (Data Terminal Equipment) o **DCE** (Data Communication Equipment)
- Necesita conector **hembra o macho**
- Qué **estándar de señalización** necesitamos

--- start-multi-column: ID_dte_dce
```column-settings
Number of Columns: 2
Largest Column: standard
```

### DTE (Data Terminal Equipment)
**Instrumento que convierte información** de usuarios en señales de transmisión o reconvierte señales recibidas en información de usuarios.

**Ejemplos:**
- Ordenadores
- Routers
- DSU/CSU's

--- column-break ---

### DCE (Data Circuit-Terminating Equipment)
Equipo como un **módem** que proporciona **reloj** al equipo DTE. Este conecta el DTE al circuito de transmisión.

**Función principal:**
- Proporciona la señal de reloj
- Conecta a la red [[Network_conceptos#WAN|WAN]]
- Marca el tiempo de transmisión

--- end-multi-column

>[!info] Diferenciación de conectores
>Los cables seriales están marcados en su extremo para DTE y DCE. Los conectores se diferencian:
>- **Macho:** se ven los pines
>- **Hembra:** se ven los huecos para los pines

<!-- IMAGEN RECOMENDADA: Conectores seriales macho vs hembra -->

### Estándares de señalización

Los estándares de señalización definen cómo se organizan los pines y las señales en el cable:

**Algunos estándares son:**
- **EIA/TIA-232 DTE** (RS-232)
- **V.35 DTE**
- **HSSI** (High-Speed Serial Interface)

<!-- IMAGEN RECOMENDADA: Conectores seriales DB-60, Smart Serial, V.35 -->

---
## Cables de Fibra Óptica

Utiliza **filamento de vidrio** para transmitir datos mediante luz.

--- start-multi-column: ID_ventajas_fibra
```column-settings
Number of Columns: 2
Largest Column: standard
```

**Ventajas**
- **Más fino** que los cables de ethernet
- **Más flexible** que los cables de ethernet
- Inmune a interferencias electromagnéticas
- Mayor ancho de banda
- Distancias mucho más largas
- Más seguro (difícil de interceptar)

--- column-break ---

**Desventajas**
- Más costoso que el cobre
- Instalación más delicada
- Requiere equipamiento especializado
- No puede transportar energía ([[PoE (Power of ethernet)|PoE]])

--- end-multi-column

Hay dos clasificaciones principales de fibra óptica:

### MMF vs SMF - Comparación

--- start-multi-column: ID_mmf_smf
```column-settings
Number of Columns: 2
Largest Column: standard
```

### MMF (Multi-Mode Fiber)
Núcleo de **largo diámetro**, permitiendo **múltiples modos** o rayos de luz para propagarse. Diseñado para emisores de luz más baratos.

**Características:**
- Usa **LED** (850nm o 1300nm)
- Distancia: **20-500m** (hasta ~2 km)
- Más económico
- Color típico: **Naranja**
- Usado en:
	- Campus
	- Edificios
	- Distancias cortas

--- column-break ---

### SMF (Single-Mode Fiber)
Núcleo **muy estrecho** que permite un **solo modo** de propagación de luz. Requiere **LÁSER** (más caro).

**Características:**
- Usa **LÁSER** (1310nm o 1550nm)
- Distancia: **2 millas a 100+ km**
- Más costoso
- Color típico: **Amarillo**
- Usado en:
	- [[Network_conceptos#WAN|WAN]]
	- Conexiones entre ciudades
	- Largas distancias

--- end-multi-column

<!-- IMAGEN RECOMENDADA: Diagrama comparativo del núcleo MMF vs SMF mostrando la diferencia de diámetro y propagación de luz -->

>[!tip] Identificación de cables de fibra
>Para diferenciarlos se puede hacer por el **código en el módulo** del cable. También hay una **tabla de colores** para diferenciar los distintos cables de fibra:
>- Los cables **multimodales** suelen ser **naranjas**
>- Los cables **single-mode** suelen ser **amarillos**

<!-- IMAGEN RECOMENDADA: Cables de fibra naranja (MMF) y amarillo (SMF) -->

### Tabla comparativa completa

| Característica | MMF (Multi-Mode) | SMF (Single-Mode) |
| :--- | :--- | :--- |
| **Diámetro del núcleo** | 50-62.5 μm | 8-10 μm |
| **Fuente de luz** | LED | LÁSER |
| **Distancia máxima** | ~2 km | ~100 km |
| **Costo** | Más barato | Más caro |
| **Color del cable** | Naranja | Amarillo |
| **Ancho de banda** | Menor | Mayor |
| **Uso típico** | LAN, Campus | WAN, Larga distancia |
| **Dispersión modal** | Sí (limita distancia) | No |

---
## Conectores de Fibra Óptica

Los conectores de fibra óptica varían según el tipo de instalación y factor de forma:

--- start-multi-column: ID_conectores_fibra
```column-settings
Number of Columns: 2
Largest Column: standard
```

### Conectores comunes

**LC (Lucent Connector)**
- Conector pequeño y compacto
- Muy usado en módulos SFP
- Factor de forma reducido
- El más popular actualmente

**SC (Subscriber Connector)**
- Conector cuadrado push-pull
- Fácil de conectar/desconectar
- Usado en instalaciones antiguas

--- column-break ---

**ST (Straight Tip)**
- Conector tipo bayoneta
- Más antiguo
- Requiere girar para conectar
- Menos común hoy día

**MPO/MTP**
- Conector multi-fibra
- Alta densidad
- Usado en data centers
- Puede tener 12, 24 o más fibras

--- end-multi-column

<!-- IMAGEN RECOMENDADA: Comparación visual de conectores LC, SC, ST y MPO -->

>[!warning] Limpieza de conectores
>Los conectores de fibra óptica deben mantenerse **extremadamente limpios**. Una mota de polvo microscópica puede bloquear completamente la señal de luz. Siempre usa:
>- Tapas protectoras cuando no estén en uso
>- Limpiadores especiales de fibra
>- Inspección con microscopio antes de conectar

---
## Resumen de tipos de cable

| Tipo de Cable | Medio | Distancia Máxima | Velocidad Típica | Uso Principal | Conector Común |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **UTP Cat 5e** | Cobre | 100m | 1 Gbps | LAN doméstica/[[Arquitecturas_modernas#Arquitectura SOHO (Small Office / Home Office)|SOHO]] | RJ45 |
| **UTP Cat 6/6a** | Cobre | 100m | 1-10 Gbps | LAN empresarial | RJ45 |
| **STP** | Cobre | 100m | 1-10 Gbps | Entornos con EMI | RJ45 |
| **Coaxial** | Cobre | Variable | Variable | Cable TV, antiguo | BNC |
| **Serial** | Cobre | Variable | Variable | Conexiones [[Network_conceptos#WAN|WAN]] | DB-60, Smart Serial |
| **Console** | Cobre | Corta | N/A | Gestión de equipos | RJ45 a DB9/USB |
| **MMF** | Fibra | ~2 km | 1-100 Gbps | Campus, edificios | LC, SC, ST |
| **SMF** | Fibra | ~100 km | 1-100 Gbps | WAN, larga distancia | LC, SC |

---
## Relación con Interfaces Cisco

Este documento complementa la información de [[Cisco_Interfaces_Hardware]]:

**Interfaces de cobre:**
- Los puertos [[Cisco_Interfaces_Hardware#Interfaces Ethernet (LAN)|RJ45]] aceptan cables de cobre (Cat 5e, Cat 6, Cat 6a)
- Los cables de cobre UTP pueden transportar energía mediante [[PoE (Power of ethernet)|PoE]]

**Interfaces de fibra:**
- Los puertos [[Cisco_Interfaces_Hardware#Interfaces Ethernet (LAN)|SFP/SFP+]] aceptan módulos de fibra óptica (MMF o SMF)
- Los módulos SFP se insertan en el puerto y luego se conecta el cable de fibra

**Interfaces seriales:**
- Las [[Cisco_Interfaces_Hardware#Interfaces Seriales (WAN)|interfaces seriales]] utilizan cables específicos con conectores DB-60 o Smart Serial
- Requieren identificar si el dispositivo es DTE o DCE

**Interfaces de gestión:**
- Los puertos console usan cables especiales rollover RJ45 a DB9/USB
- Necesarios para configuración inicial y recuperación

---
## Topología Física y Cableado

El tipo de cableado utilizado afecta directamente a la [[Topologias_de_red#¿Que es una topología?|topología física]] de la red:

**En arquitecturas [[Topologias_de_red#Modelo de 3 capas (Jerarquico)|jerárquicas de 3 capas]]:**
- **Capa de Acceso**: Cables de cobre Cat 6/6a hacia dispositivos finales
- **Capa de Distribución**: Mezcla de cobre y fibra MMF
- **Capa de Core**: Fibra SMF para máximo rendimiento

**En arquitecturas [[Topologias_de_red#Arquitectura Spine-Leaf|Spine-Leaf]]:**
- Enlaces entre Spine y Leaf: Fibra óptica (MMF o SMF según distancia)
- Servidores a Leaf: Cables de cobre Cat 6a o fibra según requerimientos

---
**Tags:** #CCNA/Fundamentos #Hardware/Cableado #Capa_Fisica #Ethernet #Fibra_Optica #Estado/Terminado