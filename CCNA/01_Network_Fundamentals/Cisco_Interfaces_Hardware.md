# Cisco Interfaces 
---
>[!info] Que es una interfaz
>Es un conector que proporciona energía o señal a un dispositivo.
>**Ejemplos cotidianos:** HDMI (Video), Jack (Audio).
>**En Networking:** Nos centramos en interfaces de **datos**, aunque algunas pueden dar energía (PoE).
## Criterios de clasificación
Las interfaces variarán en tamaño y forma según:
1. **LAN vs WAN**: En LAN los conectores suelen ser más pequeños al conexiones más cortas.
2. **Pines**: Distinta cantidad según necesidad.
3. **Medio de transmisión**: Luz (Fibra), Electricidad (Cobre), RF (Wireless).
## Ubicación
Los puertos en cisco los podemos encontrar:
- **Integrados**: En el chasis, no son extraíbles.
- **Modulares**: Tarjetas que se pueden inesrtar/cambiar.
	- **NMs**: Network modules.
	 ![[Pasted image 20251201110441.png]]
- **HWICs**: Wan Interface Cards (High speed).
  ![[Pasted image 20251201110638.png]]
- **PAs**: Adaptadores de puerto
 ![[Pasted image 20251201110734.png]]
 - **VWICs**: Voice/WAN Interface Cards.
	![[Pasted image 20251201110846.png]]
>[!Example] Identificación visual
Podemos identificar una interfaz por su tamaño, forma, conectores y el número de Part.
**PA-4T**: *Port adapter de 4 puertos*
**Ethernet 1/0**: *Slot/Puerto*

---
## Interfaces comunes
### Interfaces ethernet (LAN)
- **RJ45**: Típico para interfaces ethernet de cobre.
		![[Pasted image 20251201111350.png]]
- **Transceptores**:
	- **GBIC** Gigabit Interface Converter: Interfaz Gigabit, creada inicialmente para fibra. Es grande.
		- ![[Pasted image 20251201111852.png]]
	- **SFP** Small Form-Factor Pluggable: Interfaz convertidor de Gigabit. Es más pequeño que el GBIC.
		- ![[Pasted image 20251201112140.png]]

### Interfaces de stacking (Apilamiento)
Sirven para unir varios switches y administrarlos como un único equipo lógico. 
- **StackWise Catalyst3750**: Conecta ek plan o posterior entre sí.
- **FlexStack Catalysr 2960**: Usa un módulo de pila flexible en la parte traera.

### RPS
Fuente de alimentación redundante.

---

## Interfaces seriales (WAN)
> [!fail] El problema de Ethernet en WAN > Ethernet tiene una distancia máxima de **100 metros**. Para conectar redes lejanas, se inventaron las interfaces seriales.

### Ethernet vs TDM
