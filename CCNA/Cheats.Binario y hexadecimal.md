# Cheat Sheet: Binario y Hexadecimal

> [!tip] Uso Práctico
> No estudiar teoría. Usar esta hoja solo para **Subnetting (IPv4)** y **IPv6/MAC Addresses**.

## 1. La Tabla Mágica del Subnetting (IPv4)
Memorizar las posiciones de los bits para calcular máscaras rápido.

| Bit (Posición) | 8 | 7 | 6 | 5 | 4 | 3 | 2 | 1 |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Valor Decimal ($2^n$)** | **128** | **64** | **32** | **16** | **8** | **4** | **2** | **1** |
| **Máscara Acumulada** | 128 | 192 | 224 | 240 | 248 | 252 | 254 | 255 |
| **CIDR (en el octeto)** | /25 | /26 | /27 | /28 | /29 | /30 | /31 | /32 |

---

## 2. Hexadecimal (Para IPv6 y MAC)
Vital para leer direcciones MAC y encabezados en Wireshark.

| Decimal | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | **10** | **11** | **12** | **13** | **14** | **15** |
| :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| **Hex** | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | **A** | **B** | **C** | **D** | **E** | **F** |
| **Binario**| 0000 | ... | ... | ... | ... | ... | ... | ... | 1000 | ... | 1010 | 1011 | 1100 | 1101 | 1110 | 1111 |

> [!example] Truco de Conversión Rápida
> Para pasar de Binario a Hex, divide el byte (8 bits) en dos grupos de 4 bits (nibbles).
> * `11000010` $\rightarrow$ `1100` (12 = **C**) y `0010` (2 = **2**) $\rightarrow$ **0xC2**

---
**Tags:**
#CCNA/Fundamentos
#Herramientas/Calculo
#Subnetting
#Estado/Terminado