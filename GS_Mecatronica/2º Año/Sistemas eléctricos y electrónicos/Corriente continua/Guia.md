# Guía de Estudio: Fundamentos de Circuitos Eléctricos

### **Introducción General**

Este documento ha sido diseñado para servir como una guía de estudio clara y estructurada que te ayudará a comprender los conceptos esenciales de la electricidad, reemplazando material de clase que pueda resultar confuso. La guía está organizada de manera lógica, comenzando con los conceptos más básicos como la tensión y la corriente, avanzando hacia las leyes fundamentales de análisis de circuitos, e incluyendo ejercicios prácticos al final para reforzar el aprendizaje y asegurar una comprensión sólida del material.

--------------------------------------------------------------------------------

### **1. Los Pilares de la Electricidad: Tensión y Corriente**

#### **Introducción a la Sección**

La tensión y la corriente son los conceptos más fundamentales en el estudio de la electricidad. Representan la "causa" y el "efecto" en cualquier circuito: la tensión es la fuerza que impulsa a las cargas eléctricas, y la corriente es el flujo resultante de esas cargas. Entender su naturaleza, su relación y cómo se miden es el primer paso indispensable para poder analizar cualquier circuito eléctrico, desde el más simple hasta el más complejo.

#### **Definición de Corriente Eléctrica**

La **corriente eléctrica** se define como el movimiento ordenado de electrones a través de un material conductor. Para que este flujo de electrones ocurra, es imprescindible que exista una **diferencia de potencial (tensión)** entre dos puntos del conductor.

Existen dos convenciones para describir la dirección de la corriente:

- **Dirección real:** Es el flujo físico de los electrones, que se mueven desde el punto de menor potencial (terminal negativo) hacia el de mayor potencial (terminal positivo).
- **Dirección convencional:** Es la adoptada históricamente y la más utilizada en el análisis de circuitos. Considera el flujo de corriente desde el terminal positivo hacia el negativo.

#### **Tipos de Corriente**

#### Corriente Continua (CC o DC)

En la corriente continua, los electrones se mueven siempre en la misma dirección, manteniendo una polaridad constante. Es el tipo de corriente que encontramos en dispositivos alimentados por pilas, baterías o paneles solares.

#### Corriente Alterna (CA o AC)

En la corriente alterna, el sentido del flujo de electrones cambia constantemente porque la polaridad de la fuente de tensión varía en el tiempo. Este es el tipo de corriente que llega a nuestras viviendas a través de los enchufes.

#### **Análisis de la Tensión Eléctrica (Diferencia de Potencial)**

La **tensión (V)**, también conocida como diferencia de potencial, es la energía necesaria para mover una unidad de carga eléctrica entre dos puntos de un circuito. Se expresa matemáticamente como:

V = \frac{W}{Q}

- `V`: Tensión o voltaje, medida en **voltios (V)**.
- `W`: Trabajo realizado o energía, medida en **julios (J)**.
- `Q`: Carga eléctrica, medida en **culombios (C)**.

💡 _Cuanto mayor sea la tensión aplicada, mayor será la energía disponible para mover los electrones._

La tensión se mide utilizando un **voltímetro**, el cual debe conectarse **en paralelo** con el componente o los puntos del circuito cuya diferencia de potencial se desea conocer.

#### **Análisis de la Intensidad de Corriente**

La **intensidad de corriente (I)** mide la cantidad de carga eléctrica que atraviesa la sección de un conductor por unidad de tiempo. Su fórmula es:

I = \frac{Q}{t}

- `I`: Intensidad de corriente, medida en **amperios (A)**.
- `Q`: Carga eléctrica, medida en **culombios (C)**.
- `t`: Tiempo, medido en **segundos (s)**.

La corriente se mide con un **amperímetro**, que debe conectarse **en serie** dentro del circuito para que toda la corriente que se quiere medir pase a través de él.

#### **Componentes Básicos del Circuito**

- **Generador:** Es el elemento encargado de mantener una diferencia de potencial constante entre sus terminales, proporcionando la energía necesaria para impulsar los electrones. Ejemplos comunes son las baterías y las fuentes de alimentación.
- **Receptor o Carga:** Es cualquier dispositivo que recibe la energía eléctrica y la transforma en otro tipo de energía útil, como luz, calor o movimiento.

|   |   |
|---|---|
|Tipo de energía|Ejemplo|
|Eléctrica → Mecánica|Motores|
|Eléctrica → Térmica|Calentadores, hornos|
|Eléctrica → Química|Cargadores de batería|

Una vez comprendida la fuerza que impulsa (tensión) y el flujo que resulta (corriente), es necesario estudiar el elemento que se opone naturalmente a este flujo: la resistencia eléctrica.

--------------------------------------------------------------------------------

### **2. La Oposición al Flujo: Resistencia Eléctrica**

#### **Introducción a la Sección**

La resistencia eléctrica es una propiedad inherente de todos los materiales que se opone al paso de la corriente. No es un concepto negativo; de hecho, es fundamental para el diseño de circuitos, ya que permite controlar el flujo de electrones. Comprender qué es la resistencia y qué factores la determinan es clave para predecir y manipular el comportamiento de un circuito.

#### **Definición y Concepto**

La **resistencia eléctrica (R)** es la oposición que presenta un material al paso de la corriente. A nivel microscópico, esta oposición se debe a las colisiones de los electrones en movimiento con los átomos que conforman la estructura del material conductor.

La relación fundamental es simple: a mayor resistencia, menor será la corriente que circulará por el material para una misma tensión aplicada.

#### **Factores Determinantes de la Resistencia**

La resistencia de un conductor depende de sus características físicas y del material del que está hecho. Los tres factores principales son:

- **Longitud (L):** La resistencia es directamente proporcional a la longitud del conductor. A mayor longitud, mayor será la resistencia.
- **Sección (S):** La resistencia es inversamente proporcional a la sección (área transversal) del conductor. A mayor sección, menor será la resistencia.
- **Resistividad (ρ):** Es una propiedad específica de cada material que indica su capacidad para oponerse al flujo de corriente.

#### **Cálculo de la Resistencia**

La relación entre estos factores se expresa con la siguiente fórmula:

R = ρ \cdot \frac{L}{A}

- `R`: Resistencia, medida en **ohmios (Ω)**.
- `ρ`: Resistividad del material, medida en **ohmio-metro (Ω·m)**.
- `L`: Longitud del conductor, medida en **metros (m)**.
- `A`: Área de la sección transversal, medida en **metros cuadrados (m²)**.

#### **Influencia de la Temperatura**

La temperatura es otro factor crucial que afecta a la resistividad y, por lo tanto, a la resistencia. En la mayoría de los metales, la resistencia aumenta a medida que aumenta la temperatura. Esta relación se puede modelar con la siguiente fórmula:

\rho_{T}=\rho_{0}[1+\alpha(T -T_{0})]

- `ρT`: Resistividad a la temperatura T.
- `ρ₀`: Resistividad a una temperatura de referencia T₀ (normalmente 20 °C).
- `α`: Coeficiente de temperatura del material (en 1/°C).
- `T`: Temperatura actual (°C).
- `T₀`: Temperatura de referencia (°C).

Ahora que hemos definido la tensión, la corriente y la resistencia, estamos listos para explorar la ley que las une matemáticamente y que constituye el pilar del análisis de circuitos: la Ley de Ohm.

--------------------------------------------------------------------------------

### **3. La Ley Fundamental: Ley de Ohm**

#### **Introducción a la Sección**

La Ley de Ohm es, sin duda, la piedra angular del análisis de circuitos eléctricos. Nombrada en honor a Georg Simon Ohm, esta ley proporciona una relación matemática simple pero increíblemente poderosa entre la tensión, la corriente y la resistencia. Dominar la Ley de Ohm es esencial para calcular y predecir el comportamiento de prácticamente cualquier circuito de corriente continua.

#### **Enunciado de la Ley de Ohm**

La Ley de Ohm establece que la corriente que circula por un conductor es **directamente proporcional a la tensión**aplicada en sus extremos e **inversamente proporcional a su resistencia**.

De este enunciado se desprenden dos consecuencias lógicas clave:

- Si se mantiene la resistencia constante, un aumento de la tensión provocará un aumento de la corriente.
- Si se mantiene la tensión constante, un aumento de la resistencia provocará una disminución de la corriente.

#### **Fórmulas y Aplicaciones**

La relación matemática que describe la Ley de Ohm es:

**V = I · R**

- `V`: Tensión o voltaje, medida en **voltios (V)**.
- `I`: Intensidad de corriente, medida en **amperios (A)**.
- `R`: Resistencia, medida en **ohmios (Ω)**.

A partir de esta fórmula principal, podemos despejar las otras dos magnitudes:

- Para calcular la corriente: I = V/R
- Para calcular la resistencia: R = V/I

#### **Ejemplo Práctico**

- **Problema:** Una lámpara con una resistencia de 200 Ω se conecta a una tensión de 220 V. Calcular la corriente que circula por ella.
- **Resolución:** Aplicamos la fórmula para calcular la corriente. I = V/R = 220/200 = 1.1 A
- Por la lámpara circula una corriente de 1.1 amperios.

#### **Instrumentos de Medida y Unidades**

Para medir las tres magnitudes fundamentales, se utilizan los siguientes instrumentos:

- **Voltímetro:** Mide la tensión (se conecta en paralelo).
- **Amperímetro:** Mide la corriente (se conecta en serie).
- **Óhmetro:** Mide la resistencia de un componente (se usa con el componente desconectado del circuito).

Las unidades de resistencia y sus múltiplos más comunes se resumen en la siguiente tabla:

|   |   |   |
|---|---|---|
|Unidad|Símbolo|Equivalencia|
|Ohmio|Ω|Unidad base|
|Kiloohmio|kΩ|10^3 Ω|
|Megaohmio|MΩ|10^6 Ω|
|Miliohmio|mΩ|10^{-3} Ω|

Una vez entendida la relación fundamental V-I-R, el siguiente paso lógico es analizar la energía que se consume en un circuito y la rapidez con la que se consume, lo que nos lleva a los conceptos de potencia y energía eléctrica.

--------------------------------------------------------------------------------

### **4. El Consumo en un Circuito: Potencia y Energía Eléctrica**

#### **Introducción a la Sección**

Es crucial diferenciar entre potencia y energía. La **potencia** se refiere a la _rapidez_ con la que se consume o se entrega energía, mientras que la **energía** representa el _consumo total_ acumulado a lo largo de un período de tiempo. Comprender ambos conceptos es vital para todo, desde calcular el calentamiento de un componente hasta entender la factura de la luz.

#### **Potencia Eléctrica (P)**

La **potencia eléctrica** es la cantidad de energía consumida o entregada por un elemento del circuito por unidad de tiempo.

La fórmula general de la potencia es:

P = E/t

- `P`: Potencia, medida en **vatios (W)**.
- `E`: Energía, medida en **julios (J)**.
- `t`: Tiempo, medido en **segundos (s)**.

En términos eléctricos, la potencia se calcula principalmente como el producto de la tensión y la corriente:

P = V \cdot I

Combinando esta fórmula con la Ley de Ohm, obtenemos dos expresiones equivalentes muy útiles:

P = I^2 \cdot R y P = V^2/R

- **Ejemplo:** Un resistor de R = 100\ \Omega se conecta a una fuente de V = 20\ V.
    - **Cálculo:** P = V^2/R = 20^2/100 = 4\ W
    - **Conclusión:** El resistor disipa 4 W de potencia, que se transforman en calor.

#### **Energía Eléctrica (E)**

La **energía eléctrica** es el trabajo total realizado por la corriente eléctrica al circular por un circuito durante un tiempo determinado.

Su fórmula principal se deriva directamente de la de potencia:

E = P \cdot t

- `E`: Energía, medida en **julios (J)**.
- `P`: Potencia, medida en **vatios (W)**.
- `t`: Tiempo, medido en **segundos (s)**.

Sustituyendo las fórmulas de potencia, obtenemos sus expresiones equivalentes:

E = V \cdot I \cdot t, E = I^2 \cdot R \cdot t, y E = (V^2/R) \cdot t

Para medir el consumo eléctrico a gran escala, como en una vivienda, se utiliza una unidad más práctica: el **kilovatio-hora (kWh)**.

1 \text{ kWh} = 3,6 \times 10^6 \text{ J}

- **Ejemplo:** Una lámpara de P = 60\ W permanece encendida durante t = 5 horas.
    - **Cálculo:**
        - Energía en kWh: E = (60\ W / 1000) \cdot 5\ h = 0,3\ kWh
        - Energía en julios: E = 60\ W \cdot (5 \cdot 3600\ s) = 1,08 \times 10^6\ J = 1,08\ MJ
    - **Conclusión:** La lámpara consume **1,08 MJ** o **0,3 kWh** de energía.

#### **Síntesis y Observaciones Clave**

- La **potencia** mide la _rapidez_ con la que se transforma la energía.
- La **energía** mide el _consumo acumulado_ o el trabajo total realizado.
- Un dispositivo que consume potencia es un receptor (bombilla), y uno que la entrega es un generador (batería).
- La unidad que aparece en la factura eléctrica es el **kilovatio-hora (kWh)**.

Para poder aplicar estos conceptos a circuitos reales, que raramente tienen un solo componente, es necesario aprender a tratar con múltiples resistencias conectadas de diferentes maneras.

--------------------------------------------------------------------------------

### **5. Configuración de Circuitos: Asociación de Resistencias**

#### **Introducción a la Sección**

En la práctica, los circuitos eléctricos casi siempre contienen múltiples resistencias. Para analizar estos circuitos de manera eficiente, es necesario simplificarlos calculando una única **resistencia equivalente** que reemplace a la combinación de resistencias originales. Esta sección analiza las tres configuraciones básicas de conexión: serie, paralelo y mixta.

### **Resistencias en Serie**

En una asociación en serie, las resistencias se conectan una a continuación de la otra, formando un único camino para la corriente.

- **Reglas clave:**
    - **La misma corriente** circula a través de todas las resistencias.
    - **La tensión total** aplicada al conjunto se reparte entre cada una de las resistencias.
- **Fórmulas:**
    - Resistencia Equivalente: R_{eq} = R_1 + R_2 + R_3 + \dots
    - Corriente: I_{total} = I_1 = I_2 = I_3
    - Tensión: V_{total} = V_1 + V_2 + V_3
- **Ejemplo:** Calcular la resistencia equivalente de tres resistencias en serie: R_1 = 100\ \Omega, R_2 = 220\ \Omega y R_3 = 330\ \Omega.
    - R_{eq} = 100 + 220 + 330 = 650\ \Omega
- **Observaciones:**
    - La corriente es **la misma** en todas las resistencias.
    - Las tensiones **se reparten** proporcionalmente al valor de cada resistencia.
    - Añadir resistencias en serie siempre **aumenta** la resistencia total del circuito.

### **Resistencias en Paralelo**

En una asociación en paralelo, las resistencias se conectan entre los mismos dos puntos o nodos del circuito, creando múltiples caminos para la corriente.

- **Reglas clave:**
    - **La misma tensión** está aplicada a todas las resistencias.
    - **La corriente total** que llega al conjunto se reparte entre las diferentes ramas.
- **Fórmulas:**
    - Resistencia Equivalente (General): \frac{1}{R_{eq}} = \frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3} + \dots
    - Resistencia Equivalente (para dos resistencias): R_{eq} = \frac{R_1 \cdot R_2}{R_1 + R_2}
- **Ejemplo:** Calcular la resistencia equivalente de dos resistencias en paralelo: R_1 = 100\ \Omega y R_2 = 200\ \Omega.
    - R_{eq} = \frac{100 \cdot 200}{100 + 200} = \frac{20000}{300} = 66,7\ \Omega
- **Observaciones:**
    - La **tensión** es la misma en todas las ramas del paralelo.
    - La **corriente total** se reparte entre las resistencias, circulando más corriente por la rama de menor resistencia.
    - Añadir resistencias en paralelo siempre **disminuye** la resistencia total del circuito.

### **Asociación Mixta**

Una asociación mixta es aquella que combina conexiones en serie y en paralelo dentro del mismo circuito.

- **Procedimiento de simplificación:**
    1. Identificar los grupos de resistencias que están claramente en serie o en paralelo.
    2. Calcular la resistencia equivalente de cada uno de estos grupos.
    3. Redibujar el circuito sustituyendo los grupos por sus resistencias equivalentes y repetir el proceso hasta obtener una única resistencia total.
- **Ejemplo:** En un circuito, R_4 = 50\ \Omega y R_5 = 22\ \Omega están en serie. Este conjunto está en paralelo con R_2 = 220\ \Omega. Finalmente, todo el bloque está en serie con R_1 = 100\ \Omega y R_3 = 100\ \Omega.
    1. **Cálculo serie** **R_{4-5}****:** R_{4-5} = 50\ \Omega + 22\ \Omega = 72\ \Omega
    2. **Cálculo paralelo entre** **R_{4-5}** **y** **R_2****:** R_{eq1} = \frac{72 \cdot 220}{72 + 220} = 52,1\ \Omega
    3. **Cálculo serie final:** R_T = R_1 + R_{eq1} + R_3 = 100 + 52,1 + 100 = 252,1\ \Omega
- **Observaciones:**
    - El análisis debe realizarse siempre **simplificando el circuito paso a paso**, desde las combinaciones más internas hacia las más externas.
    - Es fundamental aplicar la **Ley de Ohm** en cada etapa para obtener las corrientes o tensiones parciales a medida que se analiza el circuito.

Si bien la simplificación de resistencias es una técnica poderosa, hay circuitos más complejos donde no es posible aplicarla. Para estos casos, necesitamos herramientas de análisis más avanzadas, como las Leyes de Kirchhoff.

--------------------------------------------------------------------------------

### **6. Análisis Avanzado: Leyes de Kirchhoff**

#### **Introducción a la Sección**

Las Leyes de Kirchhoff son dos herramientas fundamentales que permiten analizar circuitos complejos donde la simple asociación de resistencias no es suficiente. Formuladas por Gustav Kirchhoff, estas leyes se basan en dos de los principios más básicos de la física: la conservación de la carga y la conservación de la energía, lo que las hace universalmente aplicables a cualquier circuito eléctrico.

### **Ley de Corrientes de Kirchhoff (LKC)**

También conocida como la primera ley o ley de los nodos, se basa en el **principio de conservación de la carga eléctrica**.

- **Definición:** La suma de todas las corrientes que entran en un nodo es igual a la suma de todas las corrientes que salen de ese mismo nodo.
- **Fórmulas:**
    - \sum I_{entrantes} = \sum I_{salientes}
    - O, de forma algebraica: \sum I = 0
- **Ejemplo:** A un nodo llegan dos corrientes, I_1 = 2 A y I_2 = 3 A. Del nodo sale una única corriente I_3.
    - **Cálculo:** I_1 + I_2 = I_3 \implies 2 A + 3 A = I_3 \implies I_3 = 5 A
    - La corriente saliente I_3 es de 5 A.
- **Observaciones:**
    - Por convenio, las corrientes **entrantes se consideran positivas** y las **salientes, negativas** al usar la forma algebraica \sum I = 0.
    - Esta ley se cumple porque **no hay acumulación de carga** en un nodo.
    - Es la base para el método de análisis de circuitos por **nodos**.

### **Ley de Tensiones de Kirchhoff (LKT)**

También conocida como la segunda ley o ley de las mallas, se basa en el **principio de conservación de la energía**.

- **Definición:** En cualquier malla o bucle cerrado de un circuito, la suma algebraica de todas las tensiones (subidas de potencial en fuentes y caídas de potencial en resistencias) es igual a cero.
- **Fórmulas:**
    - \sum V = 0
    - O, separando fuentes y caídas: \sum E = \sum V_{caídas} (la suma de las fuerzas electromotrices es igual a la suma de las caídas de tensión).
- **Ejemplo:** Una malla contiene una batería de 12 V y dos resistencias en serie, R_1 = 2\ \Omega y R_2 = 4\ \Omega, por las que circula una corriente I.
    - **Cálculo:** 12 V - (I \cdot R_1) - (I \cdot R_2) = 0 \implies 12 - 2I - 4I = 0 \implies 12 = 6I \implies I = 2 A
    - La corriente que circula por la malla es de 2 A.
- **Observaciones:**
    - Por convenio, las **subidas de tensión** (fuentes) se consideran **positivas** y las **caídas de tensión**(resistencias) se consideran **negativas**.
    - Es la base para el método de análisis de circuitos por **mallas**.
    - Ambas leyes se utilizan conjuntamente para resolver circuitos complejos.

#### **Tabla Resumen**

La siguiente tabla resume y compara ambas leyes:

|   |   |   |   |
|---|---|---|---|
|Ley|Nombre|Expresión|Principio|
|**LKC**|Corrientes (nodos)|\sum I = 0|Conservación de la Carga|
|**LKT**|Tensiones (mallas)|\sum V = 0|Conservación de la Energía|

Equipado con la Ley de Ohm, las técnicas de asociación de resistencias y las Leyes de Kirchhoff, ya posees los conocimientos necesarios para resolver una gran variedad de problemas de circuitos eléctricos. Es hora de ponerlos en práctica.

--------------------------------------------------------------------------------

### **7. Ejercicios Prácticos para Reforzar Conocimientos**

#### **Instrucción General**

La mejor manera de consolidar la teoría es aplicándola. Te animo a resolver los siguientes problemas para poner a prueba tu comprensión de los conceptos estudiados en esta guía.

#### **Problema 1: Ley de Ohm y Potencia**

- **Enunciado:** Un calefactor eléctrico tiene una resistencia de 25 Ω y se conecta a una toma de corriente de 230 V. Calcula: a) La intensidad de corriente que consume. b) La potencia eléctrica que disipa en forma de calor.
- **Resolución:**
    - a)
    - b)

#### **Problema 2: Energía Eléctrica y Costo**

- **Enunciado:** Un ordenador consume una potencia media de 150 W. Si se mantiene encendido durante 8 horas al día, calcula: a) La energía consumida en un día, expresada en kWh. b) El costo de mantenerlo encendido durante un mes (30 días), si el precio del kWh es de 0.15 €.
- **Resolución:**
    - a)
    - b)

#### **Problema 3: Asociación de Resistencias**

- **Enunciado:** Dado el siguiente circuito: R1 = 50 Ω, R2 = 75 Ω y R3 = 100 Ω. R2 y R3 están conectadas en paralelo, y este conjunto está en serie con R1. Calcula la resistencia equivalente total del circuito.
- **Resolución:**

#### **Problema 4: Ley de Kirchhoff (Conceptual)**

- **Enunciado:** A un nodo llegan dos corrientes: I1 = 3 A y I2 = 4 A. Del mismo nodo salen otras dos corrientes: I3 y I4. Si se sabe que I3 = 2 A, ¿qué valor tiene la corriente I4? ¿Qué ley has aplicado para resolverlo?
- **Resolución:**

--------------------------------------------------------------------------------

### **Conclusión**

A lo largo de esta guía, hemos recorrido los pilares de la electricidad, desde los conceptos básicos de **Tensión, Corriente y Resistencia**, pasando por la relación fundamental que los une en la **Ley de Ohm**, hasta el análisis del consumo mediante la **Potencia y la Energía**. Además, hemos explorado cómo simplificar circuitos a través de la **Asociación de Resistencias** y hemos introducido las herramientas avanzadas de las **Leyes de Kirchhoff** para circuitos más complejos. Un entendimiento sólido de estos fundamentos es absolutamente esencial para cualquier estudio posterior o trabajo práctico en el vasto y fascinante campo de la electricidad y la electrónica.