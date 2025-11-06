Tenemos un sensor de posición. La señal eléctrica es de 0 a +10V. Campo de medida de: 0-250mm.
- Cual es la sensibilidad
$$\huge \frac{10V-0V}{250mm-0mm}=\frac{10}{250}=0.04V/mm$$
- Numero de lecturas posibles para 10 bits:
$$\huge N=2^{10} = 1024$$
- Resolución en distancia
$$\huge resolución = \frac{Campo de medida}{Número de niveles}=\frac{250mm}{1024}= 0.244$$
- Valor de precisión absoluto de 0,1mm, precisión de la lectura 0,1%
	Error de lectura: $0,1\% \cdot 250 = 0,001 \cdot 250 = 0,25mm$
	Error absoluto: 0,1mm
La peor precisión será la de 0,1% de lectura.
---
En una aplicación industrial, se utiliza este detector D3V-163-1C5
- ¿Cuantos puntos tiene este detector? ¿Que significa SPDT?
Microinterruptor **SPDT** -> Single Pole Double Throw (un polo, doble tiro)
	COM
	NC
	NO
- Queremos utilizar el contacto NC, ¿como debemos alimentarlo?
Conectaríamos el +24V al borne **COM** del micro.
Conectaríamos el borne **NC** a la **entrada digital** del PLC.
- Que tipo de actuador tiene?
Cuenta con una palanca larga articulada
- ¿Cual es su número de ciclos?
Vida mecánica: 10.000.000 maniobras.
Vida eléctrica: 100.000 maniobras.
- ¿Que tornillos se necesita para su montaje?
El micro cuenta con agujeros de 3,1mm, por lo que para su montaje necesitariamos un par de tornillos y tuercas de M3.
---
Estamos trabajando en la empresa en el área de mantenimiento. Se ha roto un detector de una cinta transportadora. Su responsable de realizar el cambio le ha ofrecido la siguiente referencia de detector: M30BBE1-PSC25H-EP02
- ¿Qué tipo de detector es?
	Sensor de proximidad capacitivo.
- ¿Es cilindrica o Rectangular?
	Es cilindrico.
- ¿A qué métrica pertenece su cuerpo?
	Es una rosca de M30 x 1,5 (M30 estándar)
- ¿La salida es de NPN?
	Es un sensor PNP, normalmente abierto.
- ¿Podríamos alimentarlo si tenemos una fuente de alimentación de 35 Vdc?
	No, su tensión de servicio es de 10..30Vdc. 
- Si de la cinta pasaran 5000 piezas cada minuto, ¿puede servir para realizar el contaje/detección de las piezas?
	$\huge \frac{5000}{60}= 83,33$ piezas por segundo = 83,3Hz
	La frecuencia de conmutación del sensor es de 100Hz por lo que si admitiria ese ritmo de servicio. 
---
Sea un Encoder incremental de referencia de **E6C2-CWZ5B 500 2M OMRON**. Si el contador tiene una opción de lectura de resolución x1 ¿Que resolución de ángulo tiene el encoder en cada vuelta? ¿Si tuviera una resolución de x4?
- Resolución x1:
$$\huge resolución_{x1} = \frac{360^\circ}{500}= 0,72^\circ por \ pulsos$$
- Resolución x4:
En x4 se aprovechan los 4 flancos de la señal en cuadratura, así que:
$500 \cdot 4 = 2000 cuentas por vuelta$
