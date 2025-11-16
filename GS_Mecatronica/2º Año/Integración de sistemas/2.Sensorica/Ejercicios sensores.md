1. Las piezas realizadas mediante una máquina de inyección pasan por una cinta de transporte sobre un soporte rectangular. Al final de la cinta se encuentra un robot para que estos productos se paleticen. Los productos pueden ser de plástico o aluminio (brillante). Siempre habrá un pequeño espacio seguido de un producto a otro. Nos gustaría saber cuántos han pasado por cada producto. Identifique entre los diferentes detectores trabajados en clase, el sistema que debería utilizarse para llevar a cabo este proceso, justificando su decisión; creando el sistema más simple posible. Tener en cuenta que hay que contarlos. Dibuja manualmente el sistema para indicar la colocación del/ los detector/es.

He seleccionado dos sensores, un capacitivo para contar la totalidad de los productos que pasen, y un segundo sensor inductivo que detectaria los productos metálicos. Esto nos permitiría que con una simple cuenta sabríamos cuantos productos de cada han cruzado. 
![[GS_Mecatronica/2º Año/Integración de sistemas/2.Sensorica/Untitled Diagram.svg]]
2. Se trata de controlar el sistema de la puerta de la imagen. Si aparece algún objeto mientras se cierra la puerta, se debería parar el proceso de cierre. Selecciona la mejor familia de detectores que utilizarías en el sistema de detección, de forma razonada. ¿Cuáles son las razones para no seleccionar las demás familias?\

Utilizaremos un sensor de posición fotoeléctrico con emisor-receptor, que ambos componentes cuenten con cableado en ambos lados para asegurarnos que el sistema detecte ante el paso de cualquier coche o peatón.

3. 
a) Tenemos un encoder absoluto de 11 bits acoplado al eje de un motor. ¿Cuál es la resolución en º de cada vuelta del eje?
**Resolución**
$\huge 2^{11}=2048bits$
**Resolución**
$\huge\frac{360}{2048}=0,175º por pulso$
b) En el sistema de apertura de la puerta, imagen superior, se dispone de un encoder para controlar la posición de la apertura mediante un sistema de piñón cremallera. ¿Cuál será la resolución de posición de este sistema si la rueda/piñón tiene 20 dientes y la cremallera tiene 4 dientes por cm de longitud?
$\huge\frac{5}{2048}=0,002º por bit$

4. Un caudalímetro tiene un rango de medida de fondo de 570 l/min. Su área de trabajo es: valor mínimo de medición de 30 l/min y valor máximo de 600 l/min. Se ha realizado la medición de caudal en un tubo y su valor ha correspondido a 350 l/min. En el catálogo se menciona la precisión absoluta: ± 5 l/min. ¿En qué intervalo se encuentra el caudal real? ¿Y si la precisión fuese de ± 5% respecto al rango? ¿Y si fuera un 1% respecto a la lectura?
- El caudal real se encuentra a 350L $\pm$ 5L (345-355)
- $600\cdot 0,05 = \pm30$L
- $350\cdot 0,01 = \pm 3,5$ 356,5-353,5

5. Ejercicio de catálogo Sea el detector **E2K-C25MF2 2M**

	1.¿De qué familia es el detector?
Es un detector de presencia capacitivo.
	2.¿Es un detector binario?
Salida digital ON/OFF (binario).
	3.¿Qué señal de detección tiene?
Salida por transistor PNP. Distancia nominal de detección 25mm.
	4.¿Es un detector PNP o NPN?
Es **PNP**. Es decir envía +24V al detectar.
	5.¿Controla un contacto NO o NC? ¿Cuántos?
Tiene un contacto NC.
	6.¿Hay que unir la señal de salida con un cable de Métrica o cable de hilos?
Viene cableado directamente para conexionar.
	7.¿Con qué tensión hay que alimentarlo?
Se alimenta a 10-30 VDC
	8.¿Cuál es la frecuencia de conmutación del detector?
Trabaja a 60Hz
	9.¿Cuántos agujeros hay que hacer para montarlo con tuercas?
La montura cuenta con dos agujeros para M4
	10.Si el material fuese cristal (Glass), ¿cuál sería la distancia de detección?
Para el cristal seria sobre unos 5mm.

6.Supongamos que tenemos un termopar de tipo J, y que esta es la tabla que tiene. Calcula los siguientes valores:
a) Con el punto frío a 0ºC y el punto caliente a 47ºC,¿ cuál es el voltaje generado en la salida del termopar?
$47º=2,427mV$
b)¿Y con el punto frío a 0ºC y el punto caliente a 136ºC?
$136º = 7,329mV$
c)¿Y con el punto frío a 10ºC y el punto caliente a 100ºC?
$10º = 0,