# Guía de Estudio: Fundamentos de Circuitos Eléctricos

## Introducción

Este documento ha sido diseñado como una guía de estudio clara y estructurada para consolidar los conceptos fundamentales de los circuitos eléctricos de corriente continua. Su propósito es ofrecer una alternativa organizada al material de clase, abarcando desde las magnitudes básicas que definen el comportamiento de la electricidad hasta los métodos sistemáticos para el análisis de circuitos complejos. A través de esta guía, se busca construir una base sólida de conocimiento, paso a paso.

--------------------------------------------------------------------------------

## 1. Magnitudes Eléctricas Fundamentales

Para analizar cualquier circuito, es imprescindible dominar sus tres magnitudes constitutivas: la tensión, que impulsa a los electrones; la corriente, que es el flujo de esos electrones; y la resistencia, que se opone a dicho flujo. Comprender su interrelación es el primer paso esencial para el análisis riguroso de cualquier circuito eléctrico.

### 1.1. Tensión y Corriente Eléctrica

### Definiciones Clave

La **Corriente eléctrica** se define como el movimiento ordenado de electrones a través de un material conductor. Para que este flujo ocurra, es necesaria una **Tensión** (también llamada diferencia de potencial), que es la energía que impulsa a los electrones a moverse entre dos puntos de un circuito.

### Dirección del Flujo

El sentido en que fluye la corriente puede describirse de dos maneras:

- **Dirección real:** Corresponde al movimiento físico de los electrones, que fluyen del terminal de menor potencial (negativo) al de mayor potencial (positivo).
- **Dirección convencional:** Es el sentido adoptado universalmente por convenio en el análisis de circuitos, donde se asume que la corriente fluye desde el terminal positivo hacia el negativo. Aunque el flujo real es de electrones, la dirección convencional se mantiene por herencia histórica (desde antes del descubrimiento del electrón) y es el estándar universal para el análisis de esquemas eléctricos.

### Tipos de Corriente

- **Corriente continua (CC o DC):** Los electrones se mueven siempre en la misma dirección, manteniendo una polaridad constante. Ejemplos típicos son la energía suministrada por pilas, baterías o paneles solares.
- **Corriente alterna (CA o AC):** La dirección del flujo de electrones cambia de sentido constantemente debido a que la polaridad de la fuente varía con el tiempo. Es el tipo de corriente que encontramos en la toma de corriente de las viviendas.

### Fórmulas y Medición

La **Tensión (V)** se define como el trabajo o energía (W) necesario para mover una unidad de carga eléctrica (Q).

`V = W / Q`

- `V`: Tensión o voltaje, medida en **voltios (V)**.
- `W`: Trabajo o energía, medido en **julios (J)**.
- `Q`: Carga eléctrica, medida en **culombios (C)**.

Cuanto mayor sea la tensión aplicada, mayor será la energía disponible para mover los electrones.

La tensión se mide utilizando un **voltímetro**, el cual debe conectarse siempre **en paralelo** con el componente o los puntos del circuito cuya diferencia de potencial se desea conocer.

La **Intensidad de Corriente (I)** mide la cantidad de carga eléctrica (Q) que atraviesa la sección de un conductor por unidad de tiempo (t).

`I = Q / t`

- `I`: Intensidad de corriente, medida en **amperios (A)**.
- `Q`: Carga eléctrica, medida en **culombios (C)**.
- `t`: Tiempo, medido en **segundos (s)**.

La corriente se mide con un **amperímetro**, que debe conectarse **en serie** dentro del circuito para que toda la corriente que se desea medir pase a través de él.

### Componentes Básicos

- **Generador:** Es el elemento encargado de proporcionar y mantener una diferencia de potencial (tensión) entre sus terminales, como una batería o una fuente de alimentación.
- **Receptor (o carga):** Es cualquier dispositivo que recibe la energía eléctrica y la convierte en otro tipo de energía útil (luz, calor, movimiento, etc.).

|   |   |
|---|---|
|Tipo de energía|Ejemplo|
|Eléctrica → Mecánica|Motores|
|Eléctrica → Térmica|Calentadores, hornos|
|Eléctrica → Química|Cargadores de batería|

Al moverse a través de un receptor o de los propios conductores, los electrones encuentran una oposición natural a su paso. Este fenómeno se conoce como resistencia eléctrica.

### 1.2. Resistencia y Resistividad

### Análisis de la Oposición al Flujo

La **Resistencia Eléctrica** es la medida de la oposición que presenta un material al paso de la corriente. Esta propiedad no solo depende de las dimensiones físicas del conductor (su longitud y sección), sino también de una característica intrínseca del material llamada **resistividad**, la cual es sensible a los cambios de temperatura.

### Factores Determinantes

La resistencia de un conductor está determinada por tres factores principales:

- **Longitud (L):** A mayor longitud del conductor, mayor es la resistencia, ya que los electrones deben recorrer un camino más largo.
- **Sección (A):** A mayor sección (área transversal) del conductor, menor es la resistencia, pues los electrones disponen de más espacio para fluir.
- **Resistividad (ρ):** Es una propiedad específica de cada material que indica su capacidad para oponerse al flujo de corriente.

### Fórmula de la Resistencia

La relación entre estos factores se expresa matemáticamente como:

`R = ρ · (L / A)`

- `R`: Resistencia, medida en **ohmios (Ω)**.
- `ρ`: Resistividad del material, medida en **ohmios por metro (Ω·m)**.
- `L`: Longitud del conductor, medida en **metros (m)**.
- `A`: Área de la sección transversal, medida en **metros cuadrados (m²)**.

_Nota: Aunque la unidad del SI es el ohmio-metro (Ω·m), en algunas tablas técnicas es común encontrar la resistividad expresada en Ω·mm²/m para facilitar los cálculos con secciones de cable dadas en milímetros cuadrados._

### Concepto de Resistividad

La resistividad (ρ) es una propiedad fundamental que distingue a los materiales conductores de los aislantes. Un valor bajo de resistividad indica que el material permite el paso de la corriente con facilidad.

A menor resistividad, mejor conductor.

### Efecto de la Temperatura

En los materiales metálicos, un aumento de la temperatura provoca una mayor agitación de sus átomos, lo que incrementa la probabilidad de colisiones con los electrones y, por tanto, aumenta su resistencia eléctrica. La fórmula que describe este cambio es:

`RT = R0 · [1 + α · (T - T0)]`

- `RT`: Resistencia a la temperatura final `T`.
- `R0`: Resistencia a la temperatura de referencia `T0` (generalmente 20 °C).
- `α`: Coeficiente de temperatura del material, medido en **1/°C**.
- `T`: Temperatura final (°C).
- `T0`: Temperatura de referencia (°C).

**Ejemplo de cálculo:** Calcular la resistencia de un conductor de cobre a 150 °C, si su resistencia a 20 °C es de 10 Ω y su coeficiente de temperatura es α = 0.00393 (1/°C).

1. **Cálculo:** `RT = 10 · [1 + 0.00393 · (150 - 20)]`
2. **Diferencia de T:** `RT = 10 · [1 + 0.00393 · 130]`
3. **Resultado:** `RT = 10 · 1.5109 = 15,1 Ω`

### Tabla de Materiales

|   |   |   |
|---|---|---|
|Material|ρ (Ω·m) a 20°C|α (1/°C)|
|Cobre|1.72·10⁻⁸|0.00393|
|Aluminio|2.82·10⁻⁸|0.00403|
|Hierro|9.71·10⁻⁸|0.00651|

Estos tres conceptos fundamentales —tensión, corriente y resistencia— no son independientes. Una ley simple pero poderosa los relaciona a todos: la Ley de Ohm.

--------------------------------------------------------------------------------

## 2. Leyes y Principios Clave en Circuitos

Una vez comprendidas las magnitudes básicas que describen el comportamiento eléctrico, el siguiente paso es estudiar las leyes que las gobiernan. La Ley de Ohm se erige como la piedra angular para el análisis de circuitos simples, estableciendo la relación matemática fundamental entre tensión, corriente y resistencia. Adicionalmente, los conceptos de potencia y energía nos permiten cuantificar el trabajo realizado y el consumo en dichos circuitos, aspectos cruciales en cualquier aplicación práctica.

### 2.1. La Ley de Ohm

### Definición y Significado

La Ley de Ohm es el principio fundamental que establece la relación directa y lineal entre la tensión aplicada a un componente, la corriente que lo atraviesa y su resistencia. El principio clave se puede resumir así: **la corriente que circula por un conductor es directamente proporcional a la tensión aplicada e inversamente proporcional a la resistencia que presenta**.

### Fórmula Fundamental

La expresión matemática de esta ley es:

`V = I · R`

A partir de esta fórmula principal, podemos despejar las otras dos magnitudes:

- Para calcular la corriente: `I = V / R`
- Para calcular la resistencia: `R = V / I`

### Relaciones Clave

Las implicaciones directas de esta ley son:

- Si la **tensión** aumenta (manteniendo la resistencia constante), la **corriente aumenta** proporcionalmente.
- Si la **resistencia** aumenta (manteniendo la tensión constante), la **corriente disminuye** en la misma proporción.

### Ejemplo Práctico

Se conecta una lámpara con una resistencia de 200 Ω a una toma de corriente de 220 V. ¿Qué corriente circula por ella?

- **Cálculo:** `I = V / R = 220 V / 200 Ω = 1.1 A`
- **Resultado:** Por la lámpara circula una corriente de 1.1 amperios.

La Ley de Ohm nos permite calcular las magnitudes instantáneas en un circuito. Sin embargo, para entender el consumo o la entrega de energía a lo largo del tiempo, debemos analizar los conceptos de potencia y energía eléctrica.

### 2.2. Potencia y Energía Eléctrica

### Diferenciación Conceptual

Es fundamental distinguir entre Potencia y Energía. La **potencia (P)** es una medida instantánea que describe la _rapidez_con la que se consume o se entrega energía en un circuito. Por otro lado, la **energía (E)** representa el _consumo total acumulado_ de potencia a lo largo de un período de tiempo determinado.

### Análisis de la Potencia Eléctrica (P)

La potencia se calcula como el producto de la tensión y la corriente.

- Fórmula principal: `P = V · I`

Utilizando la Ley de Ohm, podemos derivar dos fórmulas equivalentes que son muy útiles en la práctica:

- En función de la corriente y la resistencia: `P = I² · R`
- En función de la tensión y la resistencia: `P = V² / R`

**Ejemplo:** Un resistor de 100 Ω se conecta a una fuente de 20 V. ¿Qué potencia disipa?

- **Cálculo:** `P = V² / R = (20 V)² / 100 Ω = 400 / 100 = 4 W`
- **Resultado:** El resistor disipa 4 vatios de potencia, generalmente en forma de calor.

### Análisis de la Energía Eléctrica (E)

La energía es el producto de la potencia consumida y el tiempo durante el cual se consume.

- Fórmula principal: `E = P · t`

De manera similar a la potencia, podemos obtener fórmulas derivadas:

- `E = V · I · t`
- `E = I² · R · t`

En contextos de consumo eléctrico, como la factura de la luz, la energía no se suele medir en julios, sino en **kilovatio-hora (kWh)**.

- Equivalencia: `1 kWh = 3,6 x 10^6 J`

**Ejemplo:** Una lámpara de 60 W permanece encendida durante 5 horas. ¿Qué energía consume?

- **En julios:** `E = 60 W · (5 h · 3600 s/h) = 1,080,000 J` o `1.08 MJ`
- **En kWh:** `E = (60 W / 1000) · 5 h = 0.06 kW · 5 h = 0.3 kWh`

Si bien estas leyes se aplican perfectamente a componentes individuales, los circuitos reales suelen tener múltiples componentes conectados de diversas formas, lo que requiere métodos de análisis más estructurados.

--------------------------------------------------------------------------------

## 3. Análisis de Circuitos

Los circuitos eléctricos rara vez contienen una única resistencia. Por lo general, se componen de múltiples elementos interconectados de maneras complejas. Por ello, es crucial aprender a analizar estas configuraciones. Se comenzará por estudiar cómo simplificar las asociaciones más comunes de resistencias (serie, paralelo y mixta) para encontrar una resistencia equivalente. Posteriormente, se introducirán las Leyes de Kirchhoff, una herramienta universal y mucho más potente, capaz de resolver cualquier circuito de corriente continua sin importar su estructura.

### 3.1. Asociación de Resistencias

### Clasificación de Conexiones

Las resistencias en un circuito pueden conectarse de tres formas básicas: **serie**, **paralelo** y **mixta**.

### Resistencias en Serie

En una configuración en serie, las resistencias se conectan una detrás de otra, formando un único camino para la corriente.

- **Resistencia Equivalente:** La resistencia total es la suma de las resistencias individuales. `Req = R1 + R2 + ...`
- **Corriente:** La corriente es la misma en todos los componentes del circuito. `I_Total = I1 = I2 = ...`
- **Tensión:** La tensión total de la fuente se reparte entre cada una de las resistencias. `V_Total = V1 + V2 + ...`

**Ejemplo:** Tres resistencias de 100 Ω, 220 Ω y 330 Ω se conectan en serie. Su resistencia equivalente es: `Req = 100 + 220 + 330 = 650 Ω`

### Resistencias en Paralelo

En una configuración en paralelo, los terminales de todas las resistencias se conectan a los mismos dos puntos del circuito.

- **Resistencia Equivalente:** El inverso de la resistencia equivalente es la suma de los inversos de las resistencias individuales. `1/Req = 1/R1 + 1/R2 + ...`
- Para el caso específico de **dos resistencias en paralelo**, se puede usar esta fórmula simplificada: `Req = (R1 · R2) / (R1 + R2)`
- **Tensión:** La tensión es la misma en todas las resistencias conectadas en paralelo. `V_Total = V1 = V2 = ...`
- **Corriente:** La corriente total que entra al conjunto se reparte entre cada una de las ramas. `I_Total = I1 + I2 + ...`

**Ejemplo:** Dos resistencias de 100 Ω y 200 Ω se conectan en paralelo. Su resistencia equivalente es: `Req = (100 · 200) / (100 + 200) = 20000 / 300 ≈ 66,7 Ω`

### Resistencias Mixtas

Una asociación mixta es aquella que combina conexiones en serie y en paralelo dentro del mismo circuito. Para resolverlas, se debe simplificar el circuito por partes.

1. **Identificar** grupos simples de resistencias que estén claramente en serie o en paralelo.
2. **Calcular** la resistencia equivalente parcial de cada uno de esos grupos.
3. **Sustituir** cada grupo por su resistencia equivalente y redibujar el circuito simplificado. Repetir el proceso hasta obtener una única resistencia total.

Cuando los circuitos son demasiado complejos para ser simplificados con estas técnicas, se requieren leyes más generales y potentes, como las de Kirchhoff.

### 3.2. Leyes de Kirchhoff

Las Leyes de Kirchhoff son dos principios fundamentales que se basan en la conservación de la carga y la energía. Son herramientas esenciales para el análisis de circuitos, ya que permiten resolver sistemáticamente cualquier red eléctrica, sin importar su complejidad.

### Primera Ley: Ley de Corrientes de Kirchhoff (LKC)

Esta ley, también conocida como ley de los nodos, se basa en el **principio de conservación de la carga**.

- **Enunciado:** "La suma de todas las corrientes que entran en un nodo es exactamente igual a la suma de todas las corrientes que salen de ese mismo nodo".
- **Fórmula:** `Σ I_entrantes = Σ I_salientes` o, de forma algebraica, `Σ I = 0`.

**Ejemplo:** En un nodo entran dos corrientes, I1 = 2 A e I2 = 3 A. ¿Qué corriente (I3) debe salir del nodo para que se cumpla la ley? `I1 + I2 = I3` → `2 A + 3 A = 5 A`. Por lo tanto, `I3 = 5 A`.

### Segunda Ley: Ley de Tensiones de Kirchhoff (LKT)

Esta ley, también conocida como ley de las mallas, se basa en el **principio de conservación de la energía**.

- **Enunciado:** "En cualquier malla o lazo cerrado de un circuito, la suma algebraica de todas las tensiones (tanto las subidas de tensión de las fuentes como las caídas de tensión en las resistencias) es igual a cero".
- **Fórmula:** `Σ V = 0` (esto significa que en un circuito cerrado, toda la energía que proporcionan las fuentes es consumida por los componentes).

**Ejemplo:** En una malla cerrada hay una batería de 12 V y dos resistencias en serie de 2 Ω y 4 Ω. ¿Qué corriente (I) circula por la malla? Aplicando LKT, partimos del terminal positivo de la fuente (+12 V) y restamos las "caídas de tensión" en cada resistencia (V = I·R), que se oponen al flujo de corriente: `12 V - V_R1 - V_R2 = 0` → `12 V - (I · 2 Ω) - (I · 4 Ω) = 0` `12 V = I · (6 Ω)` → `I = 12 V / 6 Ω = 2 A`.

### Tabla Resumen

|   |   |   |   |
|---|---|---|---|
|Ley|Nombre|Expresión|Principio|
|**LKC**|Ley de Corrientes (Nodos)|`Σ I = 0`|Conservación de la Carga|
|**LKT**|Ley de Tensiones (Mallas)|`Σ V = 0`|Conservación de la Energía|

La aplicación sistemática y conjunta de estas dos leyes constituye un método infalible para la resolución de cualquier circuito de corriente continua.

### 3.3. Metodología de Resolución de Circuitos

Para resolver un circuito complejo de manera ordenada, es recomendable seguir un procedimiento paso a paso que aplique de forma sistemática las Leyes de Kirchhoff. Este método garantiza que se obtenga un sistema de ecuaciones completo para hallar todas las incógnitas del circuito.

### Pasos para la Resolución

1. **Simplificar el circuito:** Antes de aplicar las leyes, buscar y reducir cualquier asociación obvia de resistencias en serie o en paralelo para simplificar la red.
2. **Identificar nodos y ramas:** Marcar claramente los nodos (puntos donde se unen tres o más conductores) y las ramas (caminos entre dos nodos).
3. **Asignar sentidos de corriente:** Asignar una dirección arbitraria a la corriente en cada una de las ramas del circuito. No importa si la elección es incorrecta; si el resultado numérico de una corriente es negativo, simplemente significa que su sentido real es el opuesto al que se supuso.
4. **Aplicar LKC:** Plantear una ecuación de corrientes (`Σ I_entrantes = Σ I_salientes`) para cada nodo principal del circuito.
5. **Aplicar LKT:** Plantear una ecuación de tensiones (`Σ V = 0`) para cada malla o lazo independiente del circuito, recorriéndolo en un sentido definido (por ejemplo, horario).
6. **Resolver el sistema de ecuaciones:** Con las ecuaciones obtenidas de los pasos 4 y 5, resolver el sistema matemático para encontrar los valores de las corrientes desconocidas. Una vez conocidas las corrientes, se pueden calcular las caídas de tensión en cualquier resistencia usando la Ley de Ohm (`V = I·R`).

El objetivo de este método es transformar un diagrama de circuito complejo en un sistema de ecuaciones lineales algebraicamente soluble, garantizando que no se omita ninguna variable o condición.

La mejor manera de afianzar estos conceptos teóricos es a través de la práctica, resolviendo problemas que integren todos los principios estudiados.

--------------------------------------------------------------------------------

## 4. Ejercicios Prácticos

A continuación, se proponen una serie de problemas para poner a prueba la comprensión de los conceptos y leyes estudiados en esta guía. Los ejercicios cubren desde cálculos básicos de Ley de Ohm y potencia hasta el análisis de asociación de resistencias y la aplicación conceptual de las Leyes de Kirchhoff.

### Ejercicio 1: Ley de Ohm y Potencia

Un calefactor eléctrico tiene una resistencia de 30 Ω y se conecta a una toma de corriente de 220 V.

1. Calcula la corriente que circula a través de él.
2. Calcula la potencia que consume en vatios (W).
3. Si se deja encendido durante 2 horas, ¿qué energía consume en kilovatios-hora (kWh)?

### Ejercicio 2: Resistencia y Temperatura

Un conductor de aluminio tiene una resistencia de 5 Ω a una temperatura de 20 °C. Sabiendo que el coeficiente de temperatura del aluminio es α = 0.00403 (1/°C).

1. Calcula cuál será su nueva resistencia si su temperatura aumenta hasta los 100 °C.

### Ejercicio 3: Asociación de Resistencias

Dado el siguiente circuito mixto, donde R1 = 100 Ω, R2 = 220 Ω y R3 = 330 Ω. Las resistencias R2 y R3 están en paralelo entre sí, y este conjunto está en serie con R1.

1. Calcula la resistencia equivalente del paralelo entre R2 y R3.
2. Calcula la resistencia total equivalente de todo el circuito.

### Ejercicio 4: Leyes de Kirchhoff (Conceptual)

En un nodo de un circuito entran dos corrientes, I1 = 4 A e I2 = 1.5 A. Del mismo nodo salen otras dos corrientes, I3 e I4. Si se sabe que I3 = 2 A.

1. Aplicando la Ley de Corrientes de Kirchhoff (LKC), determina el valor y el sentido de la corriente I4. ¿Entra o sale del nodo?

--------------------------------------------------------------------------------

## Conclusión

Esta guía ha recorrido los pilares del análisis de circuitos eléctricos en corriente continua. Una comprensión sólida de las magnitudes fundamentales —Tensión, Corriente y Resistencia—, junto con el dominio de las reglas que las gobiernan —la Ley de Ohm para componentes individuales y las Leyes de Kirchhoff para redes complejas—, proporciona las herramientas necesarias para analizar y resolver sistemáticamente cualquier circuito. Dominar estos principios teóricos es el primer paso; la verdadera maestría se alcanza al aplicarlos de forma sistemática en la resolución de ejercicios, transformando las fórmulas en una auténtica intuición para el análisis de circuitos.