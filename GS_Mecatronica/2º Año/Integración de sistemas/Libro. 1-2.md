# Fundamentos de Sistemas de Control y Sensores Industriales

--------------------------------------------------------------------------------

## PARTE 1: TEORÍA DE SISTEMAS DE CONTROL

### **Capítulo 1: Introducción a los Sistemas de Control**

El dominio de los sistemas de control es el pilar fundamental de la automatización industrial, permitiendo que las máquinas y procesos operen de forma autónoma, eficiente y segura. Comprender sus principios es esencial para diseñar, implementar y mantener cualquier solución automatizada, desde una simple línea de montaje hasta complejos procesos químicos.

Un **sistema** se define como un conjunto de elementos relacionados entre sí que trabajan en conjunto para cumplir un objetivo. En el contexto de la automatización, el objetivo principal es gobernar el comportamiento de una o más variables del proceso. Para lograrlo, se manejan una serie de conceptos clave:

- **Controlar:** Es la acción de medir el valor de una variable y actuar sobre el sistema para reducir la diferencia entre el valor real y el deseado.
- **Variable controlada:** Es la magnitud física que se mide y que se desea mantener estable (por ejemplo, la temperatura de un horno o el nivel de un depósito).
- **Consigna:** Se refiere al valor deseado que debe alcanzar y mantener la variable controlada.
- **Acción de control:** Es la magnitud sobre la que se actúa para modificar la variable controlada, como la apertura de una válvula o la potencia aplicada a una resistencia.
- **Perturbación:** Es una entrada no deseada que altera el comportamiento del sistema y que el control debe ser capaz de compensar.

Los sistemas se clasifican principalmente en dos categorías según si utilizan o no la retroalimentación para corregir su comportamiento: lazo abierto y lazo cerrado.

|                                 |                                                                                                                                       |                                                                                                                                            |
| ------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| Característica                  | Lazo Abierto                                                                                                                          | Lazo Cerrado                                                                                                                               |
| **Principio de funcionamiento** | La salida no influye sobre la entrada. El controlador genera la orden sin tener en cuenta el resultado real.                          | La salida influye en la entrada mediante retroalimentación. El controlador compara la salida real con la consigna y corrige la diferencia. |
| **Características clave**       | - A cada entrada le corresponde una salida fija.<br>- No se compara la salida con el valor deseado.<br>- No existe retroalimentación. | - Existe retroalimentación.<br>- La salida se compara continuamente con la consigna.<br>- El sistema se corrige automáticamente.           |
| **Ventajas**                    | - Simplicidad <br> - Bajo coste y fácil implementación.                                                                               | - Alta inmunidad a perturbaciones externas<br>- Mayor precisión                                                                            |
| **Desventajas**                 | - No se corrige ante errores <br> - Requiere calibración exacta.                                                                      | - Mayor complejidad <br> - Puede volverse inestable <br> - Coste y mantenimiento mayores.                                                  |
| **Ejemplo representativo**      | El acelerador manual de un coche: si se mantiene en una posición fija, no se ajusta automáticamente si el coche encuentra una cuesta. | Un regulador de temperatura que ajusta automáticamente la potencia de una resistencia según la lectura de un termómetro.                   |
La elección entre estas dos topologías de control depende directamente de la naturaleza del proceso a automatizar, lo cual se explorará a continuación.
**Ejemplo lazo cerrado**
![[Pasted image 20251104084407.png]]
- **Referencia**: Es el valor deseado que queremos alcanzar.
- **Comparador**: Compara la señal de la consigna con la señal de realimentación y genera una señal con el error.
- **Organo de control**: Recibe una señal de control que actuará sobre la planta.
- **Actuador(amplificador)**: Transforma la señal en una acción sobre la planta.
- **Planta o proceso**: Es el sistema que queremos controlar, donde se produce la variable controlada.
- **Sensor(organo de medida)**: Mide la variable real de salida del proceso y la convierte en una señal de realimentación (feedback) al sistema.
### **Capítulo 2: Tipos de Procesos y Estrategias de Control Básicas**

La clasificación de los procesos industriales es un paso estratégico crucial, ya que esta distinción determina fundamentalmente la estrategia de control y el hardware más adecuado para la tarea. Principalmente, se dividen en procesos continuos, donde las variables se gestionan de forma constante, y procesos secuenciales, que operan por etapas discretas.

|   |   |   |
|---|---|---|
|Característica|Proceso Continuo|Proceso Secuencial|
|**Naturaleza de las variables**|Variables analógicas que varían de forma constante en el tiempo (temperatura, presión, nivel).|Operaciones discretas o por etapas definidas.|
|**Hardware de control típico**|Controladores específicos como los de tipo ON-OFF o PID.|Autómatas programables (PLC).|
|**Tipo de señales**|Variables analógicas.|Señales digitales (0/1) para avanzar de un estado a otro.|
|**Ejemplos**|Control de temperatura en un horno industrial, control del nivel de líquido en un depósito.|Una línea de montaje, el ciclo automático de una máquina herramienta.|

#### **Análisis del Control ON-OFF**

El control ON-OFF (todo o nada) es la estrategia de control más simple, donde la salida del controlador solo puede adoptar dos estados: completamente encendido (ON) o completamente apagado (OFF). Su lógica de funcionamiento es directa:

- Si `Error > consigna` → la salida se activa (ON).
- Si `Error ≤ consigna` → la salida se desactiva (OFF).

|   |   |
|---|---|
|Ventajas|Desventajas|
|- Simple y económico <br> - Robusto <br> - Fácil de implementar|- Oscilación permanente de la variable <br> - Conmutación frecuente que genera desgaste <br> - No apto para sistemas que requieren alta precisión|

El principal inconveniente del control ON-OFF es la oscilación constante de la variable alrededor de la consigna y el desgaste asociado a las conmutaciones frecuentes. Para mitigar este problema, se introduce el concepto de **Histéresis**. La histéresis crea una "banda muerta" alrededor de la consigna, de modo que el actuador no conmuta inmediatamente al cruzar el valor deseado, sino que espera a que el error sobrepase un margen predefinido.

Por ejemplo, un termostato con una consigna de 25 °C y una histéresis de ±3 °C se comportará de la siguiente manera:

- **Enciende** la calefacción cuando la temperatura desciende por debajo de **22 °C** (Consigna −3 °C).
- **Apaga** la calefacción cuando la temperatura supera los **28 °C** (Consigna +3 °C).

Este margen reduce drásticamente el número de encendidos y apagados, alargando la vida útil del equipo y resultando en una temperatura más estable para el usuario.

Si bien el control ON-OFF es efectivo para aplicaciones simples, los procesos que demandan mayor precisión requieren estrategias más sofisticadas que puedan modular la acción de control, como la familia de controladores PID.

### **Capítulo 3: El Controlador PID: Componentes y Funcionamiento**

El controlador Proporcional-Integral-Derivativo (PID) es el estándar de facto en la industria para el control de procesos continuos. Su gran eficacia reside en la combinación sinérgica de tres acciones de control distintas (proporcional, integral y derivativa), que actúan sobre el error del sistema para lograr una respuesta rápida, estable y precisa.

#### **Acción Proporcional (P)**

Esta acción genera una salida de control que es directamente proporcional al error actual. Es la respuesta inmediata del controlador.

$$\huge u = K_{p} \cdot error$$

Su comportamiento depende del valor de la ganancia proporcional (`Kp`):

- Un `Kp` **bajo** produce una respuesta lenta y puede dejar un error grande.
- Un `Kp` **alto** acelera la respuesta, pero puede causar sobreoscilaciones e inestabilidad en el sistema.

|   |   |
|---|---|
|Ventajas|Desventajas|
|- Rápido ante perturbaciones <br> - Fácil de ajustar|- Siempre existe un **error estacionario**, es decir, una pequeña diferencia persistente entre la consigna y el valor real.|

#### **Acción Integral (I)**

La acción integral tiene como objetivo principal eliminar el error estacionario que la acción proporcional no puede corregir. Lo logra acumulando (sumando) el error a lo largo del tiempo.

$$u(t) = K_i \int e(t) \, dt$$

Mientras exista un error, la acción integral irá aumentando la salida de control hasta que el error se anule por completo.

|   |   |
|---|---|
|Ventajas|Desventajas|
|- Elimina el error estacionario <br> - Mejora la exactitud final|- Hace la respuesta más lenta <br> - Puede introducir sobreoscilaciones|

La combinación **PI (Proporcional-Integral)** es una de las más utilizadas en la industria, ya que ofrece un excelente equilibrio entre la velocidad de respuesta de la acción P y la precisión final de la acción I.

#### **Acción Derivativa (D)**

La acción derivativa actúa de forma predictiva. No se basa en el error actual, sino en su **velocidad de cambio**. Su función es anticipar el comportamiento futuro del error para mejorar la estabilidad del sistema.

$$\huge u(t) = K_d \frac{d(error)}{dt}$$

Esta acción frena la respuesta del sistema cuando el error cambia bruscamente, reduciendo las sobreoscilaciones y aumentando la estabilidad.

|   |   |
|---|---|
|Ventajas|Desventajas|
|- Aumenta la estabilidad del sistema <br> - Reduce las sobreoscilaciones <br> - Mejora la respuesta dinámica|- Es muy sensible al **ruido** en la señal de medición <br> - No elimina el error estacionario <br> - Puede amplificar vibraciones|

#### **El Controlador PID Completo**

El controlador PID combina las tres acciones para obtener lo mejor de cada una: una respuesta rápida (P), precisa (I) y estable (D). La fórmula completa que gobierna su salida es:

$$\huge u(t) = K_p \, error(t) + K_i \int error(t)\,dt + K_d \frac{d(error)}{dt}$$

|   |   |
|---|---|
|Ventajas|Desventajas|
|- Alta precisión y estabilidad <br> - Elimina el error estacionario <br> - Buen equilibrio entre respuesta y control|- Requiere un ajuste cuidadoso de sus tres parámetros (sintonización) <br> - Sensible al ruido en la señal (debido a la parte D)|

Gracias a su versatilidad y robustez, el control PID es el más utilizado en la industria para regular variables críticas como temperatura, velocidad, presión, caudal y nivel en innumerables procesos automáticos.

La implementación efectiva de cualquier sistema de control, especialmente los de lazo cerrado como el PID, depende de obtener mediciones fiables y precisas del proceso, lo cual es la función principal de los sensores industriales.

--------------------------------------------------------------------------------

## PARTE 2: SENSORES EN LA AUTOMATIZACIÓN INDUSTRIAL

### **Capítulo 4: Fundamentos de la Sensórica Industrial**

En cualquier sistema de automatización, los sensores actúan como los "sentidos" del proceso. Son dispositivos críticos que transforman una magnitud física del mundo real (como temperatura, presión o posición) en una señal eléctrica que un controlador, como un PLC, puede interpretar para supervisar el estado del sistema y tomar decisiones de control.

La secuencia típica de una señal desde el proceso hasta el controlador es la siguiente: **Sistema físico → Sensor → Transductor → Acondicionamiento → Conversor A/D → PLC**

Los sensores se pueden clasificar según diferentes criterios para facilitar su selección y aplicación:

- **Según la magnitud de medida:** Sensores de posición, velocidad, presión, temperatura, etc.
- **Según la alimentación:**
    - **Activos:** Generan su propia señal sin necesidad de alimentación externa (ej. termopares).
    - **Pasivos:** Requieren una fuente de alimentación externa para funcionar (ej. detectores inductivos).
- **Según la señal de salida:**
    - **Analógico:** Proporcionan una salida continua y proporcional a la magnitud medida, típicamente en formatos estándar como 0-10 V o 4-20 mA.
    - **Digital:** Ofrecen una salida binaria de dos estados (0/1 o ON/OFF).
- **Según el tipo de detección:**
    - **Con contacto:** Requieren contacto físico para la detección (ej. finales de carrera electromecánicos).
    - **Sin contacto:** Detectan objetos sin necesidad de tocarlos (ej. inductivos, capacitivos, fotoeléctricos).

#### **Parámetros de Calidad de un Sensor**

Para seleccionar el sensor más adecuado para una aplicación, es fundamental entender sus parámetros de calidad, que definen su comportamiento, precisión y fiabilidad.

**Rango de medición (y Span)** Define el intervalo de valores donde el sensor puede medir correctamente. El _Span_ es la diferencia entre el valor máximo y mínimo del rango. Por ejemplo, para un sensor de temperatura que mide de -30 °C a 80 °C: $Span = 80 - (-30) = 110^\circ C$ 

**Sensibilidad** Indica cuánto cambia la señal de salida por cada cambio unitario en la magnitud de entrada. Una alta sensibilidad permite detectar variaciones pequeñas. $S = \frac{\Delta\text{salida}}{\Delta\text{entrada}}$

**Resolución** Es el cambio más pequeño en la magnitud de entrada que el sensor es capaz de detectar. Por ejemplo, un sensor de fuerza con un rango de 20 N a 150 N y una resolución del 0,1% puede detectar cambios de: $0,1\% \times (150-20) = 0,13N$

**Precisión o exactitud** Describe qué tan cerca está el valor medido por el sensor del valor real de la magnitud.

**Offset o error del punto cero** Es el valor que entrega el sensor cuando la magnitud de entrada es cero. Un offset puede ser calibrado para asegurar mediciones correctas.

**Histéresis** Es la diferencia entre el punto de activación y el de desactivación del sensor. Es útil para evitar conmutaciones erráticas debidas a pequeñas vibraciones o fluctuaciones de la señal.

**Repetibilidad** Es la capacidad del sensor para proporcionar la misma lectura cuando se mide la misma magnitud en las mismas condiciones repetidamente.

**Condiciones ambientales** Especifica los límites operativos del sensor en términos de temperatura, humedad, protección IP, etc., dentro de los cuales puede funcionar sin dañarse.

**Resumen rápido**

- **Rango:** valores que puede medir.
- **Sensibilidad:** cuánto varía la salida.
- **Resolución:** cambio mínimo detectable.
- **Precisión:** diferencia con el valor real.
- **Offset:** error del cero.
- **Histéresis:** diferencia entre activar y desactivar.
- **Repetibilidad:** mide siempre igual.

Una vez entendidas estas características generales, es posible analizar tipos específicos de sensores, comenzando por los más comunes en procesos secuenciales: los detectores de proximidad.

### **Capítulo 5: Detectores de Proximidad y Salidas Digitales**

Los detectores de proximidad son componentes fundamentales en la automatización discreta. Su función es detectar la presencia o ausencia de objetos sin necesidad de contacto físico, lo cual es clave para la ejecución de secuencias, el conteo de piezas y el posicionamiento en líneas de producción.

Existen varios tipos de detectores de proximidad, cada uno basado en un principio físico diferente:

- **Electromecánicos:** Requieren contacto físico para activarse, como los finales de carrera.
- **Inductivos:** Detectan la presencia de objetos metálicos mediante un campo electromagnético.
- **Capacitivos:** Detectan cualquier tipo de material (metálico, plástico, líquido) al medir cambios en la capacitancia.
- **Fotoeléctricos:** Utilizan un haz de luz; la detección ocurre cuando el objeto interrumpe o refleja dicho haz.
- **Magnéticos:** Se activan por la presencia de un campo magnético, como el generado por un imán.
- **Ultrasonidos:** Miden la distancia a un objeto emitiendo ondas de sonido y calculando el tiempo que tarda el eco en regresar.

#### **Parámetros de Rendimiento de los Detectores de Proximidad**

**Distancia nominal de detección (Sn)** Es la distancia de detección teórica, medida en condiciones de laboratorio estándar. Es un valor de referencia que puede variar en la práctica.

**Distancia de funcionamiento efectiva (Sr o Su)** Es la distancia de detección real del sensor en condiciones normales de operación, la cual se ve afectada por la temperatura y el voltaje de alimentación. Siempre es menor o igual que la distancia nominal (Sn).

**Histéresis de conmutación** Es la diferencia entre la distancia a la que el sensor se activa al acercarse un objeto y la distancia a la que se desactiva al alejarse. Esta característica evita conmutaciones erráticas causadas por vibraciones.

**Frecuencia de conmutación** Indica el número máximo de detecciones que el sensor puede realizar por segundo. Es un parámetro crítico en aplicaciones de alta velocidad, como el conteo de piezas en una cinta transportadora rápida.

**Factor de reducción** En sensores inductivos, este factor indica cómo varía la distancia de detección según el tipo de metal. El acero se toma como referencia (factor 1.0), mientras que otros metales reducen la distancia de detección.

- Acero (factor 1.0) → Detección a 10 mm
- Aluminio (factor 0.7) → Detección a 7 mm
- Cobre (factor 0.5) → Detección a 5 mm

#### **Diferencia entre Salidas de Sensor PNP y NPN**

Esta distinción es crucial para conectar correctamente un sensor de 3 hilos a una entrada digital de un PLC. Define cómo el transistor de salida del sensor conmuta la señal. El cableado estándar es:

- **Marrón:** +24V
- **Azul:** 0V (Masa)
- **Negro:** Señal de salida

La lógica de funcionamiento es:

- **PNP (Source):** Cuando el sensor detecta un objeto, la salida (cable negro) conmuta a la tensión positiva de la alimentación (+24V). Suministra corriente a la entrada del PLC.
- **NPN (Sink):** Cuando el sensor detecta un objeto, la salida conmuta a la tensión negativa (0V o masa). Drena corriente desde la entrada del PLC.

El comportamiento de la salida también depende de si el contacto es Normalmente Abierto (N.O.) o Normalmente Cerrado (N.C.):

|   |   |   |   |
|---|---|---|---|
|Tipo de sensor|Contacto|Estado "No detección"|Estado "Sí detección"|
|PNP|N.O.|Abierto (sin señal)|+24V|
|PNP|N.C.|+24V|Abierto (sin señal)|
|NPN|N.O.|+24V (flotante)|0V (sirve negativo a la entrada)|
|NPN|N.C.|0V (sirve negativo a la entrada)|+24V (flotante)|

Si bien la detección digital es vital para procesos secuenciales, el control preciso de procesos continuos requiere mediciones continuas de variables físicas, lo que nos lleva al estudio de los sensores analógicos.

### **Capítulo 6: Sensores para la Medición de Variables Físicas Clave**

Para implementar estrategias de control avanzadas como el PID, es indispensable contar con sensores que proporcionen una medida continua y proporcional de variables críticas como la posición, la temperatura y la presión. Estos sensores suministran la retroalimentación esencial que permite a un sistema de lazo cerrado ajustar su comportamiento de forma precisa y dinámica.

#### **Sensores de Posición**

Miden el desplazamiento o la ubicación de un objeto respecto a un punto de referencia.

**Potenciómetros** Convierten un desplazamiento mecánico (lineal o angular) en una variación de voltaje. Un cursor móvil se desplaza sobre una pista resistiva, cambiando la resistencia y, por lo tanto, la tensión de salida de forma proporcional a la posición. $$\huge V_{salida}= V_{alimentacion} \cdot \frac{R_{cursor}}{R_{total}}$$ Son simples y económicos, pero su principal desventaja es el desgaste mecánico debido al contacto físico, lo que limita su vida útil.

**Encoders** Generan una serie de impulsos eléctricos a medida que un eje gira. Se clasifican en:

- **Incrementales:** Generan pulsos que deben ser contados desde un punto de referencia para determinar la posición. No recuerdan su posición si se corta la alimentación.
- **Absolutos:** Asignan un código binario único a cada posición angular, por lo que siempre conocen la posición exacta, incluso después de un corte de energía.

Los encoders incrementales suelen tener tres canales:

- **Canal A:** Genera los pulsos principales.
- **Canal B:** Desfasado 90° respecto al canal A, permite determinar el sentido de giro.
- **Canal Z:** Emite un único pulso por vuelta, usado como referencia o "cero".

La resolución se puede multiplicar contando los flancos de los canales A y B:

|   |   |   |   |
|---|---|---|---|
|Modo|Flancos que cuenta|Multiplicador|Ejemplo (PPR = 1000)|
|x1|Flanco de subida de A|x1|1000 pulsos/vuelta|
|x2|Flanco de subida y bajada de A|x2|2000 pulsos/vuelta|
|x4|Flanco de subida y bajada de A y B|x4|4000 pulsos/vuelta|

Cálculo de resolución lineal: si un encoder de 1000 PPR en modo x4 (4000 pulsos/vuelta) mueve una cinta 35 mm por vuelta: $$\huge \text{resolucion} = \frac{35}{4000} = 0,00875mm\text{/} pulso$$

**Ultrasonidos y Ópticos**

- **Ultrasonidos:** Miden la distancia emitiendo una señal de ultrasonido y midiendo el tiempo que tarda en regresar el eco. Son útiles para detectar objetos transparentes o líquidos.
- **Ópticos:** Utilizan haces de luz para la detección. Son rápidos y precisos, pero pueden ser sensibles a la suciedad o a superficies brillantes.

#### **Sensores de Temperatura**

Comparan diferentes tecnologías para medir la temperatura, cada una con sus propias características.

### Termostatos

- **Principio:** <span style="background:#fff88f">Se basan en la dilatación de un bimetal que, al deformarse por la temperatura, abre o cierra un contacto eléctrico.</span>
- **Ventajas:**
    - Muy robustos, económicos y no necesitan alimentación.
- **Desventajas:**
    - Baja precisión y solo ofrecen una salida binaria (ON/OFF).

### Termopares

- **Principio:** Basados en el efecto Seebeck. <span style="background:#fff88f">La unión de dos metales distintos genera un pequeño voltaje (mV) proporcional a la diferencia de temperatura entre la unión de medida y los terminales de conexión.</span>
- **Ventajas:**
    - Amplio rango de temperatura, económicos y de respuesta rápida.
- **Desventajas:**
    - Baja sensibilidad y menor precisión que los RTD.
- **Ejemplo de cálculo:** Un termopar tipo K (sensibilidad ≈ 41 µV/°C) con una temperatura de medida de 330 °C y terminales a 20 °C generará: $$\huge V_{sensor}=V_{Tcaliente} - V_{Tambiente} = \alpha \cdot (T_{caliente}-T_{ambiente})$$
$$\huge V = 41 \times (330 - 20) = 12,79 \text{ mV}$$
### RTD (Detectores de Temperatura por Resistencia)

- **Principio:** La resistencia eléctrica de un metal (generalmente platino, Pt100/Pt1000) varía de forma muy precisa y lineal con la temperatura. El conexionado puede ser de 2, 3 o 4 hilos para compensar el error introducido por la resistencia de los cables.
$$\huge R_{T}=R_{o} \cdot [1+\alpha \cdot (T-T_{o})]$$
En el caso de una Pt100 la $R_{o}=100\ohm$  
- **Ventajas:**
    - Muy precisos, estables y con excelente linealidad.
- **Desventajas:**
    - Más caros y con una respuesta más lenta que los termopares.

### Termistores

- **Principio:** Son semiconductores cuya resistencia varía de forma muy pronunciada, pero no lineal, con la temperatura.
    - **NTC:** La resistencia disminuye al aumentar la temperatura.
    - **PTC:** La resistencia aumenta al aumentar la temperatura.
- **Ventajas:**
    - Alta sensibilidad, respuesta rápida y bajo coste.
- **Desventajas:**
    - Rango de temperatura limitado y no linealidad.

**Nota sobre Convertidores:** Las señales de bajo nivel de sensores como termopares y RTD deben ser amplificadas y acondicionadas mediante convertidores que las transforman a señales industriales estándar (0-10V, 4-20mA) para ser leídas por un PLC.

#### **Sensores de Presión**

Estos sensores transforman la presión de un fluido en una señal eléctrica. Primero, es importante diferenciar los tipos de presión:

|   |   |   |
|---|---|---|
|Tipo de Presión|Referencia de Medida|Ejemplo|
|**Absoluta**|Respecto al vacío absoluto (0 bar).|Sensores de vacío total.|
|**Manométrica**|Respecto a la presión atmosférica local.|Manómetros de taller para neumáticos.|
|**Diferencial**|Mide la diferencia de presión entre dos puntos.|Medición de caudal o saturación de filtros.|

**Presostatos**

- **Principio:** Son dispositivos mecánicos. Cuando la presión alcanza un punto de ajuste, un elemento elástico (diafragma, fuelle) se deforma y activa un contacto eléctrico.
- **Señal:** Binaria (ON/OFF).
- **Funcionamiento:** Se utilizan para control ON-OFF con histéresis, como en un compresor que se enciende a 6 bar y se apaga a 8 bar.
- **Ventajas:** Robustos, simples y no requieren alimentación.
- **Desventajas:** Solo proporcionan una señal binaria y sufren desgaste mecánico.

**Transductores de presión**

- **Principio:** Son dispositivos electrónicos que convierten la deformación de una membrana por la presión en una señal eléctrica proporcional y continua.
- **Señal:** Analógica (típicamente 0-10 V o 4-20 mA).
- **Acondicionamiento:** Requieren circuitos amplificadores para ajustar el **Offset (cero)**, que corresponde a la salida a presión mínima, y el **Span (ganancia)**, que corresponde a la salida a presión máxima.

|   |   |   |   |
|---|---|---|---|
|Característica|Presostato|Transductor|Observaciones|
|**Señal**|Digital ON/OFF|Analógica (0–10 V / 4–20 mA)||
|**Contacto**|Mecánico (N.O./N.C.)|Electrónico||
|**Precisión**|Media (≈1 %)|Alta (<0,5 %)||
|**Uso típico**|Control ON–OFF (compresores, bombas)|Medición continua para control de procesos|Robusto y simple|