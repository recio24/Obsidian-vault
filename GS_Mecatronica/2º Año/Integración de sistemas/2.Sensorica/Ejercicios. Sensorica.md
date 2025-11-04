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
Segun su tabla unas 
- ¿Que tornillos se necesita para su montaje?
