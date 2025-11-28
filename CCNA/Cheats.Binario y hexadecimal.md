# Cheat Sheet: Binario y Hexadecimal

> [!tip] Uso Práctico
> No estudiar teoría. Usar esta hoja solo para **Subnetting (IPv4)** y **IPv6/MAC Addresses**.

## ⚡ Números que reconocer "Al Vuelo" (Flash-Card Mental)

### Números indispensables
En una Máscara de Subred (Subnet Mask), **SOLO** pueden existir estos números. Si ves un 173 o un 200 en una máscara, es un error.

| Valor Decimal | En Binario | CIDR (en ese octeto) | Tamaño de Bloque (Saltos) |
| :---: | :---: | :---: | :---: |
| **0** | `00000000` | /0 | 256 (Toda la red) |
| **128** | `10000000` | /25 | 128 IPs |
| **192** | `11000000` | /26 | 64 IPs |
| **224** | `11100000` | /27 | 32 IPs |
| **240** | `11110000` | /28 | 16 IPs |
| **248** | `11111000` | /29 | 8 IPs |
| **252** | `11111100` | /30 | 4 IPs (2 usables) |
| **254** | `11111110` | /31 | 2 IPs (Pto-a-Pto) |
| **255** | `11111111` | /32 | 1 IP (Host único) |

> [!tip] El Truco del "Magic Number"
> Memoriza la columna **"Tamaño de Bloque"**. Es lo que usarás para calcular rangos mentalmente.
> *Ejemplo:* Si la máscara termina en **.224**, el tamaño de grupo es **32**. Los rangos van de 0, 32, 64, 96...

### 2. IPs Privadas (RFC 1918)
Si ves una IP que empieza por estos números, **NO** puede salir a Internet directamente (necesita NAT).

* **10.x.x.x** (Cualquier cosa que empiece por 10).
* **172.16.0.0 - 172.31.255.255** (Cuidado aquí, 172.32.x.x SÍ es pública).
* **192.168.x.x** (La clásica de casa).

### 3. IPs Especiales (Peligro / Diagnóstico)
Si te encuentras esto en un `show ip interface brief`, debes saber qué pasa al instante.

| Dirección / Rango | Nombre | Qué significa |
| :--- | :--- | :--- |
| **127.0.0.1** (Rango 127.x.x.x) | **Loopback** | "Yo mismo". Se usa para probar si tu tarjeta de red funciona. |
| **169.254.x.x** | **APIPA** (Link-Local) | **¡ERROR!** El DHCP ha fallado y Windows se ha inventado una IP. No tendrás internet. |
| **224.0.0.x** | **Multicast** | Tráfico de protocolos (OSPF, EIGRP). No es un usuario. |
| **255.255.255.255** | **Broadcast** | "Gritar a todos en mi red local". |

### 4. Valores Hexadecimales Clave (Cisco)
* **0x2102:** Registro de configuración normal (el router arranca y carga la configuración).
* **0x2142:** Registro para **romper contraseñas** (ignora la configuración al arranque).


## Binario (IPv4)
Memorizar las posiciones de los bits para calcular máscaras rápido.

| Bit (Posición)            |    8    |   7    |   6    |   5    |   4   |   3   |   2   |   1   |
| :------------------------ | :-----: | :----: | :----: | :----: | :---: | :---: | :---: | :---: |
| **Valor Decimal ($2^n$)** | **128** | **64** | **32** | **16** | **8** | **4** | **2** | **1** |
| **Máscara Acumulada**     |   128   |  192   |  224   |  240   |  248  |  252  |  254  |  255  |
| **CIDR (en el octeto)**   |   /25   |  /26   |  /27   |  /28   |  /29  |  /30  |  /31  |  /32  |

---

## Hexadecimal (Para IPv6 y MAC)
Vital para leer direcciones MAC y encabezados en Wireshark.

| Decimal | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | **10** | **11** | **12** | **13** | **14** | **15** |
| :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| **Hex** | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | **A** | **B** | **C** | **D** | **E** | **F** |
| **Binario**| 0000 | ... | ... | ... | ... | ... | ... | ... | 1000 | ... | 1010 | 1011 | 1100 | 1101 | 1110 | 1111 |


---
**Tags:**
#CCNA/Fundamentos
#Herramientas/Calculo
#Subnetting
#Estado/Terminado