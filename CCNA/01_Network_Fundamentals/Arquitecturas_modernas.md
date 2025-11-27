# Arquitecturas Modernas

> [!info]
> Las arquitecturas modernas de red se utilizan para aumentar escalabilidad, reducir complejidad y mejorar el rendimiento.  
> Incluyen modelos como **Spine–Leaf**, redes **SOHO** y conceptos de **Cloud vs On-Premise**.

![[Topologias_de_red#Arquitectura Spine-Leaf]]

![[Pasted image 20251127183521.png]]

---
## **Arquitectura SOHO (Small Office / Home Office)**

> [!info]
Modelo de red muy simple para pequeñas oficinas o casas. Suele tener un solo router “todo en uno”.
--- start-multi-column: ID_xl1u
```column-settings
Number of Columns: 2
Largest Column: standard
```

**Características**
- 1 router que hace de Firewall + Switch + Access Point
- [[Network_conceptos#^a80a01|LAN]] y WAN muy básicas
- Poco tráfico y pocos dispositivos
- Usa Internet tipo FTTH, Cable o 4G/5G

--- column-break ---

 **Limitaciones**
- No es escalable
- Poca seguridad avanzada
- No es apto para empresas medianas
- No permite segmentación avanzada

--- end-multi-column
![[Pasted image 20251127185049.png]]
---
## On-Premise

> [!info]
Todos los dispositivos están **físicamente dentro** del edificio o campus.

**Características**
- Control total sobre la red
- Servidores y switches locales
- Mayor responsabilidad de mantenimiento
- Mayor coste inicial
- Ideal para empresas con requisitos de privacidad

## Cloud Networking

> [!info]
Parte o toda la red se gestiona desde la nube utilizando paneles centralizados.

**Características**
- Controladores como **Cisco DNA Center**, **Meraki Dashboard**, etc.
- Configuración y monitorización desde Internet
- Equipamiento local más simple
- Escalabilidad rápida
- Reducción de costes de mantenimiento
**Ventajas**
- Menos hardware local
- Automatización
- Gestión centralizada
- Ideal para empresas con varias sedes
## On-Premise vs Cloud
--- start-multi-column: ID_xkc3
```column-settings
Number of Columns: 2
Largest Column: standard
```

**On-Premise**
- Control total    
- Mayor seguridad local
- Mayor coste inicial
- Requiere personal de red

--- column-break ---

**Cloud**
- Automatización
- Gestión desde la nube
- Reducción de hardware
- Fácil de escalar

--- end-multi-column

---
## ¿Dónde usar cada arquitectura?

- **Centros de datos modernos** → Spine–Leaf
- **PYMES o campus pequeños** → Modelo de 2 capas
- **Empresas medianas/grandes** → On-Premise tradicional o híbrido
- **Sedes pequeñas / casas** → SOHO
- **Empresas distribuidas por muchas sedes** → Cloud Networking + SD-WAN
---
