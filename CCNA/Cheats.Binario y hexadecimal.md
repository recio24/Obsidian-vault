# Cheat Sheet: Binario y Hexadecimal

> [!tip] Uso Práctico
> No estudiar teoría. Usar esta hoja solo para **Subnetting (IPv4)**, **IPv6** y entender cómo filtra tráfico un router.

## Números que reconocer "Al Vuelo" (Flash-Card Mental)

### Números básicos en subredes
En una Máscara de Subred (Subnet Mask), **SOLO** pueden existir estos números.

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
> Memoriza la columna **"Tamaño de Bloque"**.
> *Ejemplo:* Si la máscara es **.240**, el tamaño de bloque es **16**. Los rangos van de 0, 16, 32, 48...

### La Lógica del Router (Operación AND)
Así es como un router sabe si una IP pertenece a una red.
* **1 + 1 = 1** (Se mantiene el bit)
* **1 + 0 = 0** (Se borra el bit)
* **0 + 0 = 0** (Se borra el bit)

> **Regla de oro:** La máscara actúa como un colador. Donde hay un **1**, la IP pasa. Donde hay un **0**, la IP se convierte en 0 (Red).

---

## Tablas de Referencia Rápida

### IPs Especiales (Peligro / Diagnóstico)

| Dirección / Rango | Nombre | Qué significa |
| :--- | :--- | :--- |
| **127.0.0.1** | **Loopback** | "Yo mismo". Para probar la tarjeta de red. |
| **169.254.x.x** | **APIPA** | **¡ERROR!** Sin DHCP. Windows se autoconfigura. No hay internet. |
| **10.x.x.x** | **Privada A** | Redes grandes (Enterprise). |
| **172.16.x - 172.31.x**| **Privada B** | Redes medianas (AWS/Azure usan mucho esto). |
| **192.168.x.x** | **Privada C** | Redes domésticas (SOHO). |
| **224.0.0.x** | **Multicast** | Tráfico de protocolos (OSPF, EIGRP). |

### Valores Hexadecimales Clave (Cisco)
* **0x2102:** Registro normal (arranque estándar).
* **0x2142:** Registro de recuperación (ignora la startup-config para resetear pass).

---

## Tablas de Conversión (Completas)
### Binario (Posiciones para IPv4)
El método "8421" extendido.

| Bit (Posición) | 8 | 7 | 6 | 5 | 4 | 3 | 2 | 1 |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Valor Decimal** | **128** | **64** | **32** | **16** | **8** | **4** | **2** | **1** |
| **Máscara Acumulada** | 128 | 192 | 224 | 240 | 248 | 252 | 254 | 255 |

### Hexadecimal (Para IPv6, MAC y Hacking)

| Posición (desde derecha) | 4ª (4096) | 3ª (256) | 2ª (16) | 1ª (1) | 
| :--- | :---: | :---: | :---: | :---: | 
| **Potencia ($16^n$)** | $16^3$ | $16^2$ | $16^1$ | $16^0$ | | **Valor Decimal** | **4096** | **256** | **16** | **1** |

| Decimal |  Hex  | Binario (8421) |
| :-----: | :---: | :------------: |
|    0    | **0** |      0000      |
|    1    | **1** |      0001      |
|    2    | **2** |      0010      |
|    3    | **3** |      0011      |
|    4    | **4** |      0100      |
|    5    | **5** |      0101      |
|    6    | **6** |      0110      |
|    7    | **7** |      0111      |
|    8    | **8** |      1000      |
|    9    | **9** |      1001      |
|   10    | **A** |      1010      |
|   11    | **B** |      1011      |
|   12    | **C** |      1100      |
|   13    | **D** |      1101      |
|   14    | **E** |      1110      |
|   15    | **F** |      1111      |

> [!example] Ejemplo de lectura MAC
> `00:0C:29...` -> `0` (0000) `C` (1100).

---
**Tags:**
#CCNA/Fundamentos
#Herramientas/Calculo
#Subnetting
#Estado/Terminado