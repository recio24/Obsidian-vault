# Power over Ethernet (PoE)
---
>[!info] Definición
>PoE es una tecnología que permite enviar energía y datos simultáneamente a través del mismo cable de red (par trenzado). Esto elimina la necesidad de fuentes de alimentación externas para cada dispositivo.

**Beneficios**
- Ahorro de costes: Menos cableado, menos transformadores...
- Flexibilidad: Puedes instalar dispositivos en lugares sin enchufes cercanos, simplemente llevando un cable de red hasta el equipo.
- Control centralizado: Se tiene control total de los equipos, sumando la capacidad de apagar un dispositivo desde el switch.
- Seguridad: Utiliza voltajes bajos y mecanismos de protección para suministrar la energía necesaria para cada dispositivo.

**Dispositivos que lo conforman**
- **PSE (Power Sourcing Equipment** 
	- Es el equipo que suministra energía.
	- Ejemplos: Switch, Inyector de energía...
- **PD (Powered Device)**
	- Es el equipo que recibe la energía.
	- Ejemplo: Teléfonos IP, cámaras IP, puntos de acceso. 

---
## Estándares IEEE PoE

| Estándar IEEE | Nombre Común | Tipo   | Potencia PSE (Salida Switch) | Potencia PD (Llegada Disp.) | Uso Típico                  |
| :------------ | :----------- | :----- | :--------------------------- | :-------------------------- | :-------------------------- |
| **802.3af**   | PoE          | Tipo 1 | **15.4 W**                   | ~12.95 W                    | Teléfonos IP, Cámaras fijas |
| **802.3at**   | PoE+         | Tipo 2 | **30 W**                     | ~25.5 W                     | APs WiFi 6, Cámaras PTZ     |
| **802.3bt**   | UPoE / 4PPoE | Tipo 3 | **60 W**                     | ~51 W                       | Iluminación, Portátiles     |
| **802.3bt**   | 4PPoE        | Tipo 4 | **90 W**                     | ~71 W                       | Pantallas grandes           |
>[!warning] Ojo con la perdida
>La potencia que llega al dispositivo (PD) siempre es menor que la que sale del switch (PSE) debido a la resistencia del cable de cobre y perdidas en calor, etc.

---
## Funcionamiento
El switch no envía 48V de golpe (quemaría un dispositivo no-PoE). Sigue un proceso de seguridad:

**1. Detección**
El PSE envía un voltaje muy bajo para buscar una resistencia concreta en el dispositivo conectado, según la variación de la carga al paso de esa resistencia.
- **Si la encuentra:** Sabe que es un PD válido y pasa a la siguiente fase. 
- **Si NO la encuentra:** Solo envía datos (protege tu PC o consola).
