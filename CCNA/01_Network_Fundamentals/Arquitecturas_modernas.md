# Arquitecturas Modernas

> [!info]
> Las arquitecturas modernas de red se utilizan para aumentar escalabilidad, reducir complejidad y mejorar el rendimiento.  
> Incluyen modelos como **Spine–Leaf**, redes **SOHO** y conceptos de **Cloud vs On-Premise**.

![[Topologias_de_red#Arquitectura Spine-Leaf]]

![[Pasted image 20251127183521.png]]

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

## On-Premise vs Cloud