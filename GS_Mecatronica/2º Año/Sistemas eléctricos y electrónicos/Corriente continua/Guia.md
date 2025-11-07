# Guía de Estudio: Fundamentos de Electricidad y Circuitos de Corriente Continua

### Introducción

Este documento sirve como una guía de estudio clara y estructurada, diseñada para complementar y clarificar los materiales de clase sobre los conceptos fundamentales de los circuitos eléctricos. La guía progresa de manera lógica, comenzando por las magnitudes eléctricas básicas y avanzando hacia el análisis de circuitos complejos, proporcionando las herramientas esenciales para comprender el comportamiento de la electricidad en corriente continua.

## 1. Magnitudes Eléctricas Fundamentales

Comprender la tensión, la corriente y la resistencia es la base absoluta para analizar cualquier circuito eléctrico. Estos tres conceptos están intrínsecamente interconectados y describen cómo se comporta la electricidad, desde su capacidad para realizar trabajo hasta la oposición que encuentra a su paso.

### 1.1 Tensión Eléctrica (Diferencia de Potencial)

La **tensión (V)**, también conocida como diferencia de potencial, se define como la energía necesaria para mover una carga eléctrica entre dos puntos de un circuito.

La relación matemática es: $V = \frac{W}{Q}$

- **V**: Tensión o voltaje, medida en **voltios (V)**.
- **W**: Trabajo o energía, medido en **julios (J)**.
- **Q**: Carga eléctrica, medida en **culombios (C)**.

En términos prácticos, una tensión más alta proporciona más energía para mover los electrones a través del circuito. La tensión se mide con un **voltímetro**, el cual debe conectarse **en paralelo** con el componente cuya diferencia de potencial se desea conocer.

### 1.2 Corriente Eléctrica

La **corriente eléctrica (I)** es el movimiento ordenado de electrones a través de un material conductor, impulsado por una diferencia de potencial.

Es importante distinguir entre las dos convenciones para su dirección:

- **Dirección real**: El flujo real de electrones, que va del terminal negativo (-) al positivo (+).
- **Dirección convencional**: El sentido adoptado históricamente para el análisis de circuitos, que va del terminal positivo (+) al negativo (-).

La intensidad de la corriente mide la cantidad de carga que fluye por un punto en un tiempo determinado: $I = \frac{Q}{t}$

- **I**: Intensidad de corriente, medida en **amperios (A)**.
- **Q**: Carga eléctrica, medida en **culombios (C)**.
- **t**: Tiempo, medido en **segundos (s)**.

Existen dos tipos principales de corriente:

- **Corriente Continua (CC/DC)**: Los electrones se mueven siempre en la misma dirección. Es la corriente generada por pilas, baterías y paneles solares.
- **Corriente Alterna (CA/AC)**: El sentido del flujo de electrones cambia constantemente debido a que la polaridad de la fuente varía. Es el tipo de corriente que encontramos en las tomas de corriente de las viviendas.

La corriente se mide con un **amperímetro**, el cual debe conectarse **en serie** en el circuito para que toda la corriente que se desea medir pase a través de él.

### 1.3 Resistencia Eléctrica

La **resistencia eléctrica (R)** es la oposición que presenta un material al paso de la corriente. Esta oposición se debe a las colisiones de los electrones con los átomos del material conductor.

La relación es inversamente proporcional: a mayor resistencia, menor será el flujo de corriente para una misma tensión. Los elementos de un circuito se clasifican según su función:

- **Generadores**: Mantienen la diferencia de potencial entre sus terminales (ej. baterías, fuentes de alimentación).
- **Receptores o Cargas**: Convierten la energía eléctrica en otras formas de energía. Las transformaciones más comunes son:
    - **Eléctrica → Térmica**: Calefactores, hornos.
    - **Eléctrica → Mecánica**: Motores.
    - **Eléctrica → Química**: Cargadores de batería.

Una ley fundamental, descrita a continuación, relaciona de manera precisa estas tres magnitudes.

## 2. La Ley de Ohm: La Relación Clave

La Ley de Ohm es la piedra angular del análisis de circuitos, ya que proporciona una relación matemática simple y directa entre la tensión, la corriente y la resistencia.

La ley establece que **la corriente que circula por un conductor es directamente proporcional a la tensión aplicada e inversamente proporcional a su resistencia.**

La fórmula principal de la Ley de Ohm es: V$ = I \cdot R$

De esta ecuación se derivan las fórmulas para calcular la corriente y la resistencia: $I = \frac{V}{R} y R = \frac{V}{I}$

Las proporcionalidades clave son:

- Si la tensión aumenta (con R constante), la corriente **aumenta**.
- Si la resistencia aumenta (con V constante), la corriente **disminuye**.

#### Ejemplo de Aplicación

Una lámpara con una resistencia de 200 Ω se conecta a una fuente de alimentación de 220 V. ¿Qué corriente circula por ella? $I = \frac{V}{R} = \frac{220}{200} = 1.1\text{ A}$

|   |   |   |
|---|---|---|
|Unidad|Símbolo|Equivalencia|
|Ohmio|Ω|Unidad base|
|Kiloohmio|kΩ|10^3 Ω|
|Megaohmio|MΩ|10^6 Ω|
|MiliOhmio|mΩ|10^{-3} Ω|

Es importante notar que el valor de la resistencia (R) en la Ley de Ohm no siempre es constante, ya que depende de las propiedades del material y de su temperatura.

## 3. Propiedades de los Materiales: Resistividad y Temperatura

La resistencia no es un valor abstracto, sino una propiedad intrínseca de un material, determinada por su estructura física, sus dimensiones y, de manera significativa, por la temperatura a la que se encuentra.

### 3.1 Resistividad

La **resistividad (ρ)** es una propiedad característica de cada material que mide su oposición intrínseca al flujo de corriente. La resistencia de un conductor específico se calcula con la siguiente fórmula: $R = ρ \cdot \frac{L}{A}$

- **R**: Resistencia, medida en ohmios (Ω).
- **ρ**: Resistividad del material, medida en (Ω·m).
- **L**: Longitud del conductor, medida en metros (m).
- **A**: Área de la sección transversal, medida en metros cuadrados (m²).

Un material con menor resistividad es un mejor conductor. A continuación se comparan algunos valores a 20 °C:

- **Cobre**: $ρ = 1.72 \times 10^{-8}\ \Omega·m$
- **Aluminio**: $ρ = 2.82 \times 10^{-8}\ \Omega·m$
- **Hierro**: $ρ = 9.71 \times 10^{-8}\ \Omega·m$

### 3.2 Efecto de la Temperatura en la Resistencia

Para la mayoría de los metales, la resistencia aumenta a medida que aumenta la temperatura. Este cambio se debe fundamentalmente a que la resistividad intrínseca del material varía con la temperatura, según la fórmula: $\rho_{T}=\rho_{0}[1+\alpha(T -T_{0})]$

A partir de esta relación, se deriva la fórmula práctica para calcular la resistencia de un conductor a una temperatura específica: $R_T = R_0 \cdot [1 + \alpha \cdot (T - T_0)]$

- **R_T**: Resistencia a la temperatura final T.
- **R_0**: Resistencia a la temperatura de referencia T_0 (generalmente 20 °C).
- **\alpha**: Coeficiente de temperatura del material (en 1/°C).
- **T**: Temperatura final (en °C).
- **T_0**: Temperatura de referencia (en °C).

#### Ejemplo de Cálculo

Se desea calcular la resistencia de un conductor de cobre a 150 °C, sabiendo que su resistencia a 20 °C es de 10 Ω. El coeficiente de temperatura del cobre es \alpha = 0.00393\ (1/°C).

1. Se aplica la fórmula: $R_T = 10 \cdot [1 + 0.00393 \cdot (150 - 20)]$
2. Se calcula la diferencia de temperatura: $R_T = 10 \cdot [1 + 0.00393 \cdot 130]$
3. Se resuelve la operación: $R_T = 10 \cdot 1.5109$

El resultado final es: $R_T = 15.1\ \Omega$.

- En los **metales**, la resistencia aumenta con la temperatura ($\alpha$ es positivo).
- En los **semiconductores**, la resistencia disminuye al aumentar la temperatura (\alpha es negativo).
- En los **superconductores**, la resistencia se vuelve prácticamente cero por debajo de una temperatura crítica.

La energía que se "pierde" debido a la resistencia de un material se convierte en otras formas de energía, principalmente calor, lo que nos lleva a los conceptos de potencia y energía eléctrica.

## 4. Potencia y Energía Eléctrica

Es crucial distinguir entre potencia y energía. La **potencia** es la _rapidez_ con la que la energía se consume o se genera en un instante, mientras que la **energía** es la _cantidad total_ de trabajo realizado o consumido a lo largo de un período de tiempo. Esta diferencia es fundamental para entender tanto el rendimiento de un dispositivo como el coste de su funcionamiento.

### 4.1 Potencia Eléctrica (P)

La **potencia eléctrica (P)** es la velocidad a la que la energía eléctrica se transforma en otra forma de energía (calor, luz, movimiento, etc.).

Su fórmula fundamental es: $P = \frac{E}{t}$ donde P es la Potencia (W), E es la Energía (J) y t es el Tiempo (s).

Combinando esta definición con la Ley de Ohm, obtenemos tres fórmulas prácticas de gran utilidad: $P = V \cdot I P = I^2 \cdot R P = \frac{V^2}{R}$

#### Ejemplo de Cálculo de Potencia

Un resistor de 100 Ω se conecta a una fuente de tensión de 20 V. ¿Cuál es la potencia que disipa?

$P = \frac{V^2}{R} = \frac{20^2}{100} = 4\ W$

Esto significa que el resistor está convirtiendo energía eléctrica en calor a un ritmo de 4 vatios (o 4 julios por segundo).

### 4.2 Energía Eléctrica (E)

La **energía eléctrica (E)** es el trabajo total realizado por la corriente eléctrica durante un período de tiempo específico. Representa el consumo acumulado.

Su fórmula principal es: $E = P \cdot t$

Sustituyendo las expresiones de la potencia, obtenemos:
$P = V \cdot I$ 
$E = I^2 \cdot R \cdot t$
$E = \frac{V^2}{R} \cdot t$

Para fines prácticos, como la facturación del consumo eléctrico, se utiliza el **kilovatio-hora (kWh)**. La conversión es: $1\ kWh = 3.6 \times 10^6\ J$

#### Ejemplo de Consumo de Energía

Una lámpara de 60 W permanece encendida durante 5 horas. Calcula la energía total consumida en julios y en kWh.

- **En Julios**: El tiempo debe estar en segundos (5 h = 5 × 3600 s = 18000 s). $E = P \cdot t = 60\ W \cdot 18000\ s = 1,080,000\ J$
- **En kWh**: La potencia debe estar en kW (60 W = 0.06 kW). $E = P \cdot t = 0.06\ kW \cdot 5\ h = 0.3\ kWh$

Para poder calcular la potencia o energía total en un circuito con múltiples componentes, primero debemos determinar la resistencia total o equivalente del circuito.

## 5. Análisis de Circuitos: Asociación de Resistencias

En un circuito real, los componentes rara vez están aislados. Se conectan en configuraciones específicas (serie, paralelo o una combinación de ambas) que determinan el comportamiento general del circuito. Dominar cómo calcular la resistencia equivalente de estas configuraciones es una habilidad fundamental para el análisis de circuitos.

### 5.1 Resistencias en Serie

En una conexión en serie, los componentes se conectan uno a continuación del otro, formando un único camino para el paso de la corriente.

Sus características clave son:

- La **corriente es la misma** a través de todas las resistencias (I = I_1 = I_2 = ...).
- La **tensión total es la suma** de las caídas de tensión en cada resistencia (V_T = V_1 + V_2 + ...).

La resistencia equivalente se calcula sumando las resistencias individuales: $R_{eq} = R_1 + R_2 + R_3 + \dots$

Por ejemplo, si $R_1 = 100\ \Omega, R_2 = 220\ \Omega$ y $R_3 = 330\ \Omega$, la resistencia equivalente es $R_{eq} = 100 + 220 + 330 = 650\ \Omega$.

### 5.2 Resistencias en Paralelo

En una conexión en paralelo, los terminales de todos los componentes están conectados a los mismos dos puntos del circuito, lo que proporciona múltiples caminos para la corriente.

Sus características clave son:

- La **tensión es la misma** en todas las resistencias.
- La **corriente total es la suma** de las corrientes que circulan por cada rama.

La resistencia equivalente se calcula con la fórmula: $\frac{1}{R_{eq}} = \frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3} + \dots$

Para el caso especial de **dos resistencias** en paralelo, la fórmula se simplifica a: $R_{eq} = \frac{R_1 \cdot R_2}{R_1 + R_2}$

Por ejemplo, con $R_1 = 100\ \Omega y R_2 = 200\ \Omega$, la resistencia equivalente es $R_{eq} = \frac{100 \cdot 200}{100 + 200} = 66.7\ \Omega$. Es importante destacar que la resistencia equivalente en una configuración en paralelo es **siempre menor** que la más pequeña de las resistencias individuales.

### 5.3 Circuitos Mixtos

Un circuito mixto es aquel que contiene combinaciones de resistencias tanto en serie como en paralelo. Para resolverlos, se sigue un procedimiento de simplificación paso a paso:

1. **Identificar** los grupos simples de resistencias en serie o en paralelo.
2. **Calcular** la resistencia equivalente parcial de cada uno de esos grupos.
3. **Redibujar** el circuito simplificado con la nueva resistencia equivalente y repetir el proceso hasta que quede una única resistencia total.

Por ejemplo, el proceso para simplificar un circuito mixto comenzaría combinando las resistencias en serie, como $R_4 = 50\ \Omega y R_5 = 22\ \Omega$ para obtener una resistencia parcial de $72\ \Omega$. A continuación, esta resistencia parcial se resolvería en paralelo con $R_2 = 220\ \Omega$, resultando en $52.1\ \Omega$. Finalmente, se sumarían en serie las resistencias restantes (R_1 y R_3) a este resultado para obtener la resistencia total del circuito.

Cuando los circuitos son demasiado complejos para ser simplificados de esta manera, se requieren herramientas más potentes como las Leyes de Kirchhoff.

## 6. Análisis de Circuitos Complejos: Las Leyes de Kirchhoff

La Ley de Ohm y las reglas de asociación de resistencias son insuficientes para analizar circuitos con múltiples fuentes de alimentación o con interconexiones complejas. Las Leyes de Kirchhoff son principios universales, basados en la conservación de la carga y la energía, que permiten resolver cualquier circuito de corriente continua.

### 6.1 Primera Ley de Kirchhoff: Ley de Corrientes (LKC)

Esta ley establece que **la suma de las corrientes que entran en un nodo es igual a la suma de las corrientes que salen de él.** Un **nodo** es un punto en el circuito donde se unen tres o más caminos.

Este principio se basa en la **conservación de la carga eléctrica**: la carga no se crea ni se destruye en un nodo. \sum I_{entrantes} = \sum I_{salientes} o, de forma algebraica, \sum I = 0

Por ejemplo, si a un nodo llegan dos corrientes, I_1 = 2 A y I_2 = 3 A, la corriente que sale, I_3, debe ser la suma de ambas: I_3 = 2 + 3 = 5 A.

### 6.2 Segunda Ley de Kirchhoff: Ley de Tensiones (LKT)

Esta ley establece que **en cualquier bucle cerrado o malla dentro de un circuito, la suma algebraica de todas las subidas y caídas de tensión es igual a cero.** Una **malla** es cualquier camino cerrado en un circuito.

Este principio se basa en la **conservación de la energía**: la energía ganada por una carga al pasar por una fuente debe ser igual a la energía que pierde al pasar por los componentes del bucle. \sum V = 0 o, de forma más explícita, \sum E = \sum V_{caídas}

Por convención, las subidas de tensión (fuentes) se consideran positivas y las caídas de tensión (resistencias) se consideran negativas. Por ejemplo, en un bucle con una batería de 12V y dos resistencias de 2 Ω y 4 Ω, la ecuación sería 12 V - I \cdot (2 \Omega) - I \cdot (4 \Omega) = 0. Resolviendo, se obtiene que la corriente I = 2 A.

### 6.3 Resumen y Aplicación

La siguiente tabla resume ambas leyes:

|   |   |   |   |
|---|---|---|---|
|Ley|Nombre|Expresión|Principio|
|**LKC**|Ley de Corrientes (Nodos)|\sum I = 0|Conservación de la Carga|
|**LKT**|Ley de Tensiones (Mallas)|\sum V = 0|Conservación de la Energía|

Estas leyes proporcionan un método sistemático para analizar cualquier circuito. Al aplicarlas, se genera un sistema de ecuaciones lineales que permite resolver las corrientes y tensiones desconocidas en cualquier parte del circuito.

## 7. Guía Práctica y Ejercicios Propuestos

Esta sección final consolida la teoría en una guía práctica para la resolución de problemas y ofrece ejercicios diseñados para poner a prueba y reforzar la comprensión de los conceptos presentados.

### 7.1 Pasos para la Resolución de Circuitos

1. **Simplificar**: Antes de aplicar métodos avanzados, combina cualquier grupo evidente de resistencias en serie o en paralelo para reducir la complejidad del circuito.
2. **Identificar Nodos y Mallas**: Marca claramente los nodos esenciales (donde se unen tres o más ramas) y las mallas o bucles independientes del circuito.
3. **Asignar Corrientes**: Dibuja una dirección de corriente arbitraria para cada rama del circuito. No te preocupes por acertar; si el resultado de una corriente es negativo, significa que su dirección real es la opuesta a la que supusiste.
4. **Aplicar LKC**: Escribe una ecuación de corrientes para cada nodo esencial, basándote en que la suma de corrientes que entran es igual a la suma de las que salen.
5. **Aplicar LKT**: Escribe una ecuación de tensiones para cada malla independiente, asegurándote de que la suma algebraica de las subidas y caídas de tensión sea cero.
6. **Resolver el Sistema**: Resuelve el sistema de ecuaciones lineales resultante para encontrar los valores de las corrientes desconocidas. Una vez conocidas las corrientes, puedes usar la Ley de Ohm (V = I \cdot R) para calcular cualquier caída de tensión que necesites.

### 7.2 Ejercicios para Practicar

**Ejercicio 1 (Ley de Ohm y Potencia):** Un calefactor eléctrico tiene una resistencia de 25 Ω y se conecta a una toma de corriente de 220 V. Calcula: a) La corriente que circula por él. b) La potencia que consume en vatios (W).

**Ejercicio 2 (Resistencia y Temperatura):** Un conductor de aluminio tiene una resistencia de 5 Ω a 20 °C. Calcula su resistencia si la temperatura aumenta a 100 °C. (Utiliza el coeficiente de temperatura para el aluminio del texto: \alpha = 0.00403\ 1/°C).

**Ejercicio 3 (Asociación de Resistencias):** Calcula la resistencia equivalente de un circuito donde una resistencia R_1 = 50\ \Omega está en serie con un conjunto en paralelo formado por R_2 = 100\ \Omega y R_3 = 100\ \Omega.

--------------------------------------------------------------------------------

Con estos principios fundamentales, desde la Ley de Ohm hasta las Leyes de Kirchhoff, ahora dispones del conjunto de herramientas esenciales para analizar y comprender los circuitos eléctricos de corriente continua.