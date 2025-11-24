# Fundamentos 
#programming 

---
## Conceptos

#### \- Lenguajes de programación 
Un lenguaje de programación es un conjunto de instrucciones que utilizamos para comunicarnos con los dispositivos informáticos, algunos ejemplos de lenguajes de programación podrían ser:
- C
- C++
- [[01 - Python|01 - Python]]
- HTML
- CSS
- [[(ST) Texto estructurado|ST]] (Este es especifico de autómatas (PLC))
#### \- IDE (Entorno de desarrollo integrado)
Un entorno de desarrollo integrado (IDE) es una aplicación de software que ayuda a los programadores a desarrollar código de software de manera eficiente. Aumenta la productividad de los desarrolladores al combinar capacidades como editar, crear, probar y empaquetar software en una aplicación fácil de usar. Así como los escritores utilizan editores de texto y los contables, hojas de cálculo, los desarrolladores de software utilizan IDE para facilitar su trabajo.
#### \- Variables
Una variable en programación es un elemento de datos cuyo valor puede cambiar durante el curso de la ejecución de un programa.
#### \- Frameworks
En programación, un framework es un marco de trabajo que tiene como objetivo facilitar la solución de problemas que pueden surgir al programar. Los frameworks aceleran el proceso de programar facilitando tareas como la organización del código o el trabajo en equipo dentro de un proyecto. Un ejemplo de Framework podría ser:
- Django (Framework de Python )
- Qt (Framework de C)
#### \- Librerías
Las librerías de programación son conjuntos de archivos de código de código que conforman funciones para ayudarnos a desarrollar software importando estas en nuestro programa, existen muchas librerías algunos ejemplos son:
- Python: matplotlib, seaborn, bokeh, Numpy, Scipy, Pandas, Numba, gensim...
- C++: iostrem, cmath, cstring, ctime, algorithm...
#### \- Sintaxis
La sintaxis es el conjunto de normas que regulan y coordinan las distintas variables y su asociación
#### \- Anidamiento
El anidamiento es la practica de incorporar llamadas a funciones o procedimientos dentro de otras mediante la inclusión de diversos niveles mediante paréntesis o tabulaciones. 
>[!example] Ejemplo en Python
>```python
>if valor1 condición valor2:
>	if valor1 condición valor2:
>		code
>	else:
>		code
>else:
>	code
>```
#### \- Lenguaje de marcas 
Un lenguaje de marcas es un forma de codificar un documento que, junto con el texto, incorpora etiquetas o marcas que contienen información adicional acerca de la estructura del texto o su presentación.  Hay muchos ejemplos uno de los mas conocidos es HTML (_HyperText Markup Languaje_)
aunque sin irnos muy lejos por ejemplo Obsidian trabaja con un lenguaje de marcas llamado [[INFORMATICA/01.0 - Programación/0102 - Lenguajes/Markdown/Markdown|Markdown]] ^markdown

---

## Data types
- int (integer) = número entero ya sean positivos o negativos 
- float = número de coma flotante o número decimal (2,5)
- str (String) = cadena de texto "Hola mundo"
- Valor booleano = Es un valor que determina si algo es verdadero o falso es decir de manera simple sirven para representar la veracidad (En contexto numérico 0 es _**False**_ y 1 es _**True**) estos valores pertenecen a la [[Algebra booleana]]
>True or False ^booleano

---
## Bucles
Un bucle o ciclo, en Programación es una secuencia de instrucciones de código que se ejecuta repetidas veces, hasta que una condición asignada a dicho bucle deja de cumplirse. Los 3 bucles más utilizados en programación son el bucle while, el bucle for y el bucle do-while.  ^bucle

- **Bucle While** = Es un ciclo basado en resultados de una expresión lógica; se encuentra en la mayoría de los lenguajes de programación. El propósito es repetir el bloque de código mientras una condición se mantenga verdadera.  Su estructura básica suele ser algo así:
```C
mientras (condición) hacer:
	instrucciones 
fin mientras
```
- **Bucle For** = El bucle for es una estructura de control en programación en la que se puede iniciar de antemano el número máximo de iteraciones. Su estructura básica suele ser algo así ^for
```C 
for (i) hasta (n) a incrementos de s hacer:
	instrucciones
fin para
```
- **Bucle do-while** = El bucle do-while comprueba la condición al final del cuerpo del bucle, y si esta es cierta continua con el resto del programa, a veces esto resulta más adecuado. La instrucción se ejecutara al menos una vez.  Su estructura basica suele ser asi:
```C
REPEAT
	WriteString("Escribe el número")
	ReadInt(número)
UNTIL (número >= 3) AND (número <= 7)
```

---

## Error frente a depuración (Bug vs. debug)

La medida básica que un desarrollador puede utilizar contra los errores es, como era de esperarse, un **depurador**, mientras que el proceso durante el cual se eliminan los errores del código se llama **depuración**. Según un viejo chiste, la depuración es un complicado juego de misterio en el que eres simultáneamente el asesino, el detective y, la parte más dolorosa de la intriga, la víctima. ¿Estás listo para interpretar todos estos roles? Entonces debes armarte con un depurador.

Un depurador es un software especializado que puede controlar cómo se ejecuta tu programa. Con el depurador, puedes ejecutar tu código línea por línea, inspeccionar todos los estados de las variables y cambiar sus valores en cualquier momento sin modificar el código fuente, detener la ejecución del programa cuando se cumplen o no ciertas condiciones, y hacer muchas otras tareas útiles.

#### \- Depuración por impresión

Esta forma de depuración, que se puede aplicar a tu código mediante cualquier tipo de depurador, a veces se denomina **depuración interactiva**. El significado del término se explica por sí mismo: el proceso necesita su interacción (la del desarrollador) para que se lleve a cabo.

Algunas otras técnicas de depuración se pueden utilizar para cazar errores. Es posible que no puedas o no quieras usar un depurador (las razones pueden variar). ¿Estás entonces indefenso? ¡Absolutamente no!

Puedes utilizar una de las tácticas de depuración más simples y antiguas (pero aún útil) conocida como la **depuración por impresión**. El nombre habla por sí mismo: simplemente insertas varias invocaciones `print()` adicionales dentro de tu código para generar datos que ilustran la ruta que tu código está negociando actualmente. Puedes imprimir los valores de las variables que pueden afectar la ejecución.

Estas impresiones pueden generar texto significativo como _"Estoy aquí", "Ingresé a la función `fo0()`", "El resultado es `0`"_, o pueden contener secuencias de caracteres que solo tu puedes leer. Por favor, no uses palabras obscenas o indecentes para ese propósito, aunque puedas sentir una fuerte tentación; tu reputación puede arruinarse en un momento si estas payasadas se filtran al público.

Como puedes ver, este tipo de depuración no es realmente interactiva en lo absoluto, o es interactiva solo en pequeña medida, cuando decides aplicar la función input() para detener o retrasar la ejecución del código.

Una vez que se encuentran y eliminan los errores, las impresiones adicionales pueden comentarse o eliminarse; tu decides. No permitas que se ejecuten en el código final; pueden confundir tanto a los probadores como a los usuarios, y traer mal karma sobre ti.

#### \- Consejos útiles

Aquí hay algunos consejos que pueden ayudarte a encontrar y eliminar errores. Ninguno de ellos es definitivo. Úsalos de manera flexible y confía en tu intuición. No te creas a ti mismo, comprueba todo dos veces.

1. **Intenta decirle a alguien** (por ejemplo, a tu amigo o compañero de trabajo) qué es lo que se espera que haga tu código y cómo se espera que se comporte. Se concreto y no omitas detalles. Responde todas las preguntas que te hagan. Es probable que te des cuenta de la causa del problema mientras cuentas tu historia, ya que el hablar activa esas partes de tu cerebro que permanecen inactivas mientras codificas. Si ningún humano puede ayudarte con el problema, usa un patito amarillo de goma en su lugar. No estamos bromeando, consulta el artículo de Wikipedia para obtener más información sobre esta técnica de uso común: [Método de depuración del patito de goma](https://es.wikipedia.org/wiki/M%C3%A9todo_de_depuraci%C3%B3n_del_patito_de_goma).
  
3. **Intenta aislar el problema.** Puedes extraer la parte de tu código que se sospecha que es responsable de tus problemas y ejecutarla por separado. Puedes comentar partes del código para ocultar el problema. Asigna valores concretos a las variables en lugar de leerlos desde la consola. Prueba tus funciones aplicando valores de argumentos predecibles. Analiza el código cuidadosamente. Léelo en voz alta.
  
5. Si el error apareció recientemente y no había aparecido antes, **analiza todos los cambios que has introducido en tu código;** uno de ellos puede ser la razón.
  
7. **Tómate un descanso**, bebe una taza de café, toma a tu perro y sal a caminar, lee un buen libro, incluso dos, haz una llamada telefónica a tu mejor amigo; te sorprenderás de la frecuencia con la que esto ayuda.
  
9. **Se optimista**: eventualmente encontrarás el error; te lo prometemos.

# Prueba unitaria: un nivel más alto de codificación

También existe una técnica de programación importante y ampliamente utilizada que tendrás que adoptar tarde o temprano durante tu carrera de desarrollador: se llama **prueba unitaria**. El nombre puede ser un poco confuso, ya que no se trata solo de probar el software, sino también (y, sobre todo) **de cómo se escribe el código**.

Para resumir la historia, las pruebas unitarias asumen que las pruebas son partes inseparables del código y la preparación de los datos de prueba es una parte inseparable de la codificación. Esto significa que cuando escribes una función o un conjunto de funciones cooperativas, también estás obligado a crear un conjunto de datos para los cuales el comportamiento de tu código es predecible y conocido.

Además, debes equipar a tu código con una interfaz que pueda ser utilizada por un entorno de pruebas automatizado. En este enfoque, cualquier enmienda realizada al código (incluso la menos significativa) debe ir seguida de la ejecución de todas las pruebas unitarias que acompañan al código fuente.

Para estandarizar este enfoque y facilitar su aplicación, Python proporciona un módulo dedicado llamado `unittest`. 
