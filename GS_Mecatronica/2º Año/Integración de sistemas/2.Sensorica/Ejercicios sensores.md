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