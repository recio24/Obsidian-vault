# Python
#programming 

---
## Que es Python

Es un lenguaje de programación de alto nivel con una sintaxis simple y fácil de aprender y utilizar lo que lo ha hecho un lenguaje utilizado en en gran cantidad de campos y propósitos.
Entre sus ventajas podemos contar cosas como su gran comunidad y la gran cantidad de [[0100 - Fundamentos#- Librerías]] y [[0100 - Fundamentos#- Frameworks]] que tiene también es importante señalar que entre los campos en los que se trabaja es un lenguaje con capacidad para trabajar en lo llamado "[[Programación orientada a objetos (OOP)]]".

La facilidad de su sintaxis reside entré varias cosas que a la hora de trabajar cada línea es una línea real de programa es decir que para hacer otra función por ejemplo pasaríamos a la siguiente línea.

En pequeño vistazo su sintaxis se vería así:

``` python
a = 23
b = "El número es: "
print(b,a)
```

---
## Tipos de datos (Data type)

![[0100 - Fundamentos#Data types]]

Para declarar este tipo de datos en un programa utilizamos las [[0100 - Fundamentos#- Variables]], para declarar una variable en Python es muy simple se debe indicar el nombre de la variable seguido de un igual y lo que le queramos asignar el único que cambia entre ellos es el ***string*** que debe ir metido entre comillas.
Su sintaxis se vería algo así: 
``` python
a = 1 #int a = número
b = 2,5 #float b = número decimal
c = "Hola mundo" #string c = "Texto"
```

#### \- Valor booleano
Ejemplos de [[0100 - Fundamentos#^booleano|valor booleano]]:
``` python
a = True > False
print(a) #Esto nos daría como resultado un True en consola

b = False > True
print(b) #Esto nos daría como resultado un False en consola
```

---

## Funciones básicas

##### \- Print()
Para representar datos en la pantalla (consola) podemos utilizar una función que hemos podido ver en los ejemplos anteriores llamada print() su sintaxis seria así:
>print(dato a imprimir)
``` python
a = 2
print(a)
#Esto nos imprimiria en la consola el número 2 
```

##### \- Input()
Sirve para cuando queramos que el programa le pida al usuario un dato y si lo predecimos por una variable este input se almacene podemos hacer input de cualquiera de los Data types básicos que conocemos su sintaxis seria algo así:
```python
variable = input("Escriba un número: ", )
```

Como se aprecia en el ejemplo si ponemos una cadena de texto dentro del input seguido de la coma el 
programa imprimirá el texto y seguido le pedirá al usuario que haga el input antes de seguir el programa.

Si necesitamos que en la variable se almacene siendo de uno de los Data types, podemos hacer la conversión si no fuese posible el programa daría error y pararía el programa, se vería así:
```python
variable = float(input("Escriba un número: ", ))
```

---
## Comentarios
Para insertar comentario en Python normalmente se inserta un ```#``` seguido del comentario
```python
x = 2 + 3 #Esto es una suma
```
Lo que pasa que esto esta limitado a un comentario en una sola línea si quisiésemos hacer un comentario multilínea se podría hacer poniendo ``` ''' ``` al principio y al final del comentario se vería algo así: 
``` python
x = 2 + 3 '''Esto es un comentario 
multilinea'''
x = 2
```

---
## Operadores básicos  
> [!info] 
> Si quieres saber más puedes ir a la nota [[00 - Operaciones básicas]]

Un operador en programación es un símbolo que es capaz de realizar operaciones con los valores, por ejemplo ```+```  (suma) es capaz de sumar dos valores ```2 + 3 = 5```. Los principales operadores en Python son:

##### \- Suma [[00 - Operaciones básicas#Suma|>]]
La suma ```+``` nos permite la adición de un valor a otro valor en Python se vería así: 
``` python
3 + 4 
```

##### \- Resta [[00 - Operaciones básicas#Resta|>]]
La resta ```-``` sustrae un valor a otro valor en Python se vería así: 
``` python
3 - 2 
```

##### \- Multiplicación [[00 - Operaciones básicas#Multiplicación|>]]
La multiplicación ```*``` permite suma el mismo valor tantas veces como indiques, en Python se vería así
```python
3 * 2 
```

##### \- División [[00 - Operaciones básicas#División|>]]
La división ```/``` nos permite [[00 - Operaciones básicas#División|dividir]] los valores que le indiques en Python se vería así:
``` python
4 / 2 
```

##### \- El modulo
El modulo ```**``` nos permite obtener el [[00 - Operaciones básicas#\- Resto|resto]] de una división en Python se vería así: 
``` python 
5 ** 3
```

##### \- División entera
La división ```//``` entera nos permite hacer la división y [[00 - Operaciones básicas#- Truncar|truncar]] su resultado para imprimir únicamente el número que precede a la coma en Python se vería así:
``` python
4 // 3
```

##### \- Potencia [[00 - Operaciones básicas#Potencia|>]]
La potencia ```**``` nos permite multiplicar un número por si mismo tantas veces como se le indique en Python se vería así:
```python
4 ** 3
```

---

## Operadores abreviados
Los operadores básicos en algunos casos se pueden abreviar cuando queramos aplicarlo a una variable ya que si ponemos el signo que queramos ejecutar justo antes del igual este se aplicara utilizando la variable y lo seguido después del igual, por ejemplo:

```python
i = i + 2 --> i += 2

var = var / 2 --> var /= 2
```

---
## Comparadores
Sirven para comprar dos valores, serian lo siguientes: 

| Signo | Definición                                                |
| ----- | --------------------------------------------------------- |
| >     | Revisa si el primer valor es mayor que el segundo         |
| <     | Revisa si el primer valor es menor que el segundo         |
| <=    | Revisa si el primer valor es menor o igual que el segundo |
| >=    | Revisa si el primer valor es mayor o igual que el segundo |
| ==    | Revisa si los dos valores son iguales                     |
| !=    | Revisa si los valores son distintos te da True            |

---
## Operadores booleanos
Son usados para comparar valores verdad sores o falsos, serian los siguientes:

| and | Compara entre dos valores y da True si ambos valores lo son       |
| --- | ----------------------------------------------------------------- |
| or  | Compara entre dos valores y da True si uno o ambos valores lo son |
| not    | Compara de manera negada osea el True pasa a False y viceversa |

---
## Operador `In` y `Not in`

| in     | Nos sirve para ver si algo se encuentra dentro de algo por ejemplo un [[#- Diccionarios\|Diccionario]] |
| ------ | ------------------------------------------------------------------------------------------------------ |
| not in | Nos sirve para vcer si algo no se encuentra dentro de algo por ejemplo una [[#Listas\|lista]]          |

---

## Condiciones básicas
Las condiciones nos permiten hacer funciones sobre una condición, es decir si algo se cumple hacerlo y si no lo es no hacerlo.v

##### \- if
Usa comparadores para determinar si el código que contiene ha de ser ejecutado un ejemplo seria:
```python
if valor1 condición valor2:
	codigo

if número de trozos > 6:
	comerse la mitad
	darle la otra mitad a Juan
```

##### \- else
Ejecuta una pieza de código en caso de que el if al que va encadenado no sea True, un ejemplo se vería así: 
```python
if valor1 condición valor2:
	codigo
else:
	codigo

if numero de trozos > 6:
	comerse la mitad
	darle la otra mitad a Juan
else:
	comerme toda yo
```

##### \- elif
El elif es un else pero que también lleva una condición puede usarse para encadenar varias condiciones es decir:  
```python
if valor1 condición valor2:
	codigo
elif valor1 condición valor2:
	codigo
elif valor1 condición valor2:
	codigo
else:
	codigo
```



>[!info] Información
>También se pueden anidar estas condiciones dentro de condiciones, para que se vea mas claro aquí ahí un ejemplo: 
> ````python
> if valor 1 condición valor2:
> 	if valor1 condición valor2:
> 		codigo
> 	else:
> 		codigo
> else:
> 	codigo
> ````

---
## Bucles

![[0100 - Fundamentos#^bucle]]

##### \- Bucle while
La función ```while``` ejecuta una porción de código una y otra vez hasta que la condición especificada sea falsa; o, dicho de otro modo, ejecuta una porción de código mientras que la condición sea verdadera 
```python 
a = 1
while a < 10:
	print("Hola mundo")
	a = a + 1
```
Ahora el resultado es distinto: el mensaje se imprime nueve veces. Analicemos por qué pasa esto. Cuando el intérprete tiene que ejecutar el bucle, evalúa la condición `a < 10`, que en un primer momento equivale a `1 < 10`, que es verdadero. Entonces, ejecuta el bloque de código dentro del bucle: imprime el mensaje en pantalla y luego le suma `1` a la variable `a`. Cuando el bloque de código finaliza, se vuelve a evaluar la condición, que ahora resulta ser `2 < 10`, aún verdadero. Luego se ejecuta nuevamente el bloque de código y el proceso se repite hasta llegar a la condición `10 < 10`, que es falsa y por ende el bucle termina. Esto se puede ver más claro si imprimimos la variable `a`:

```python
a = 1
while a < 10:
	print("Hola mundo")
	print(a)
	a += 1 
```

Además, cambié la última línea por `a += 1`, que es simplemente un atajo para `a = a + 1`.

##### \- El bucle while junto a la rama else
La rama `else` del bucle siempre se ejecuta una vez, independientemente de si el bucle ha entrado o no en su cuerpo.

```python
i = 1
while i < 5:
    print(i)
    i += 1
else:
    print("else:", i)

```

Como podemos ver al salir del bucle `i` vuelve a su estado inicial en caso de editar el programa para que el bucle  `while` no funcionase marcándole un False veremos que el `else` si se ejecuta: 

```python
i = 5
while i < 5:
    print(i)
    i += 1
else:
    print("else:", i)
```

##### \- Bucle for
![[0100 - Fundamentos#^for]]

Su sintaxis en Python será así:

```python
for i in cosa:
	print(i)
```

Un ejemplo curioso que nos permite el `for` es iterar en una palabra y hacer un programa que cuente letras por ejemplo

```python
word = str(input("Escribe una palbra para contar sus letras: ", ))
a = 1
for b in word:
	print(a)
	a += 1
```

También podemos utilizar el `range()` en un bucle `for` para determinar un rango de números que le servirá al bucle para saber cuantas veces se va a repetir. El `range()` se vería algo así `range(1 , 11)` o `range(5)` un ejemplo en código sería algo así: 

```python
for i in range(1 , 11):
	print(i)
```

##### \- El bucle for junto a la rama else
Los bucles `for` se comportan de manera un poco diferente: echa un vistazo al fragmento en el editor y ejecútalo. La variable `i` conserva su último valor.

```python
for i in range(5):
    print(i)
else:
    print("else:", i)

```

##### \- Sentencias break y continue

- break = sale del bucle inmediatamente, e incondicionalmente termina la operación del bucle; el programa comienza a ejecutar la instrucción más cercana después del cuerpo bucle.

```python
# break - ejemplo

print("La instrucción break:")
for i in range(1, 6):
    if i == 3:
        break
    print("Dentro del bucle.", i)
print("Fuera del bucle.")

```

- continue = se comporta como si el programa hubiera llegado repentinamente al final del cuerpo; el siguiente turno se inicia y la condición expresión se prueba de inmediato.

```python
# continue - ejemplo

print("\nLa instrucción continue:")
for i in range(1, 6):
    if i == 3:
        continue
    print("Dentro del bucle.", i)
print("Fuera del bucle.")

```

---
## Listas

Es posible que en algún momento necesites almacenar gran cantidad de números y hacer esto mediante variables es posible pero cuando hablamos de mucho es un trabajo duro y lento, para solucionar eso existen las listas, para crear una lista pondremos el nombre la lista segundo de un igual y dos corchetes que contendrán todos los números que componen la lista, los números serán separados por comas. Se vería algo así `nombre = [1, 2, 3, 4, 5]` Los elementos dentro de la lista pueden ser de distintos tipos como números enteros, flotantes o pueden ser otras listas.

```python
numbers = [1, 2, 3, 4, 5]
print("Contenido de la lista:", numbers)
```

Si quisiéramos cambiar un número de una lista es simple solo hay que saber que en las listas la numeración de posición comienza por el 0 ósea que el primer digito seria el 0 el segundo seria el 1 y así sucesivamente. También es importante recalcar que los números negativos tambien sirven para declarar una posición en una lista por ejemplo -1 es el ultimo número de la lista, -2 es el penultimo y asi sucesivamente.
Si quisiésemos cambiar un número por otro haríamos lo siguiente:

```python
numbers = [1, 2, 3, 4, 5]

numbers [0] = 111 #Aqui cambiamos el número en la posición 0 por un 111
print("Contenido de la lista:", numbers)
```

De igual manera también es posible copiar el número de una posición a otra posición, se haría de la siguiente forma:

```python
numbers = [1, 2, 3, 4, 5]

numbers [0] = numbers [4] #Aqui estamos copiando el valor de posición 4 por el 0
print("Contenido de la lista", numbers)
```

De esta anterior manera se nos puede ocurrir intentar intercambiar dos números dentro de una lista pero esto no es posible ya que primero se ejecutara una linea y después la otra cuándo uno de los valores ya ha sido reemplazado. Imagina que queremos intercambiar la ultima posición de la lista con el primero ósea pasar el número 1 por el 5 así que podemos hacer lo siguiente: 

```python
numbers = [1, 2, 3, 4, 5]

numbers [0], numbers [4] = numbers [4], numbers [0]

print("Contenido de la lista:", numbers)
```

Como podemos ver hemos aplicado una doble igualdad en la misma linea lo cual ha intercambiado sus valores.

##### \- La función len()

La longitud de una lista puede variar durante la ejecución de un programa, si deseamos verificar o averiguar la longitud de una lista podemos utilizar la función `len()` 
Esta función toma el nombre de la lista como argumento y nos devuelve la longitud de la lista, podemos ver su funcionamiento y sintaxis en el siguiente ejemplo:
```python 
numbers = [1, 2, 3, 4, 5]

print("La longitud de la lista numbers es de:", len(numbers))
```

##### \- Eliminación de elementos en una lista

Para eliminar elementos de una lista se utiliza la función `del` seguido por la lista y la posición del elemento a eliminar podemos apreciarlo mejor en el siguiente ejemplo:
```python
numbers = [1, 2]

print(numbers) #Hacemos un primer print para ver el estado inicial de la lista

del numbers[1] #Aplicamos la función y eliminamos el segundo número

print(numbers) #Volvemos a imprimir y vemos el estado final de la lista
```

##### \- Agregar elementos a una lista

Para cumplir este propósito podemos utilizar el `append()` y el `insert()`. 

- append() = Este toma el valor de su argumento y lo coloca al final de la lista que posee en el [[Programación orientada a objetos (OOP)#\- Método frente a función|método]] su uso se vería de la siguiente manera: 
```python
list.append(value)
```

- insert( ) = Este es algo mas inteligente ya que nos permite agregar un elemento en cualquier punto de la lista, solo al final como nos ocurría en `append()`
	
	Este tomaria dos argumentos
	- El primero muestra la ubicación requerida del elemento a insertar (Los elementos a existentes a la derecha del nuevo elemento incluido el que estaba en esa posición originalmente se desplazaran a la derecha) 
	- El segundo es el elemento a insertar 

Su uso se vería de la siguiente manera:
```python
list.insert(location, value)
```

>[!info] Listas vacias
>Cabe indicar que es posible iniciar la vida de una lista estando esta vacía y insertar y eliminar elementos a ella mediante los métodos anteriormente indicados. Podríamos declararla así:
>```python
>numbers = [] #lista vacia
>```

##### \- Haciendo uso de for en las listas

El bucle `for` tiene una variante muy especial que puede procesar las listas de manera muy efectiva. Supongamos que deseas calcular la suma de todos los valores de una lista, pues podríamos usar el `for` para iterar en la lista almacenando en cada iteración cada elemento de la lista y sumarlo a una variable que almacenara la suma total. Este ejemplo se vería algo así: 

```python
numbers = [1, 4, 5, 12, 564]
total = 0

for i in numbers:
	total += i
print(total)
```

También podríamos hacerlo utilizando en la condición del bucle el largo de la lista y utilizando este como posición después en el código del bucle:

```python
numbers = [1, 4, 5, 12, 564]
total = 0


for i in range (len(numbers)) :
	total += numbers [i]
print(total)
```

>[!tip] 
>Con estos dos ejemplos podemos ver como siempre hay muchas soluciones para el mismo problema utilizando distintos métodos condiciones y funciones 

##### \- Ordenamiento burbuja

- sort()

Cuando queramos ordenar una lista siempre podemos imprimirla y hacer un código que vaya intercambiando las posiciones de los valores de la lista para que esta quede ordenada como deseemos. 

Para esta misión también hay que decir que Python cuenta con un [[Programación orientada a objetos (OOP)#\- Método frente a función|método]] llamado `sort()` que nos ordenara la lista, podemos utilizar este método de la siguiente manera:

```python
numbers = [8, 10, 6, 2, 4]
print(numbers)

numbers.sort() #Aqui podemos ver el uso de el método sort
print(numbers)
```

- reverse

Este [[Programación orientada a objetos (OOP)#\- Método frente a función|método]] nos sirve para invertir una lista su uso es simple:

```python
numbers = [1, 2, 3, 4]
print(numbers)

numbers.reverse() #Aqui aplicamos el metodo reverse para invertir la lista 
print(numbers)
```

#### \- La vida en las listas

>[!danger] Importante
>Las listas (y muchas otras entidades complejas) no se almacenan igual que las variables (escalares) se podría decir que: 
>	- El nombre de una variable es el nombre de su contenido
>	- El nombre de una lista es el nombre de una ubicación de memoria donde se almacena la lista

Si tomamos en cuenta esto ultimo y en nuestro código hacemos la siguiente declaración:

```python
list_1 = [1]
list_2 = list_1
list_1[0] = 2

print(list_2)
```

Esto sucede ya que ambos nombres apuntan al mismo sitio en memoria con lo que al editar uno el otro también se ve afectado.

#### \- Listas dentro de listas

Las listas pueden contar con escalares (números) pero también pueden estar formadas por listas. Un ejemplo podría ser un **tablero de ajedrez**.

Un tablero de ajedrez esta compuesto de filas y columnas. Hay ocho filas y ocho columnas, cada columna está marcada con las letras de la A a la H y cada línea esta marcada con números del 1 al 8. Con lo que una posición e identifica con un par par formador por una letra y un número. 

Si quisiésemos crear la lista de la segunda dila del tablero podríamos utilizar el siguiente código:

```python
row = []

for i in range(8):

row.append(WHITE_PAWN)
```

Este código se puede comprimir (este método se utiliza para generar listas masivas durante la ejecución de un código) mediante el siguiente código:

```python
row = [WHITE_PAWN for i in range(8)]

#Ejemplo lista comprimida: odds = [x for x in squares if x % 2 != 0 ]
```

Si suponemos que la palabra "EMPTY" se refiere a una casilla vacía entonces si quisiésemos crear el tablero de ajedrez podríamos hacerlo de la siguiente manera:

```python
board = []
empty = "EMPTY"

for i in range(8):
	row = [empty for i in range(8)]
	board.append(row)

print(board)
```

Este modelo imita perfectamente el tablero de ajedrez real, que en realidad es una lista de elementos de ocho elementos, todos ellos en filas individuales. Resumamos nuestras observaciones:

- Los elementos de las filas son campos, ocho de ellos por fila.
- Los elementos del tablero de ajedrez son filas, ocho de ellos por tablero de ajedrez.

La variable `board` ahora es un **arreglo bidimensional**. También se le llama, por analogía a los términos algebraicos, una **matriz**.

Como las listas de comprensión puede ser **anidadas**, podemos acortar la creación del tablero de la siguiente manera:

```python
board = []
empty = "EMPTY"

board = [[empty for i in range(8)] for j in range(8)]
print(board)
```

Si queremos hacer un código que nos forme el tablero total, se vería algo así:

```python
EMPTY = "-"
PAWN = "PEON"
ROOK = "TORRE"
KNIGHT = "CABALLO"
board = []

for i in range(8):
    row = [EMPTY for i in range(8)]
    board.append(row)

board[0][0] = ROOK
board[0][7] = ROOK
board[7][0] = ROOK
board[7][7] = ROOK

print(board)

```

Para referirnos a las distintas casillas dentro de las listas deberemos utilizar las coordenadas en este ejemplo podemos verlas en la imagen del tablero

![[Pasted image 20230710224548.png]]

---
## Slides (Rebanadas)

Las slides son una funcionalidad de Python que permite extraer un subconjunto de elementos de una lista o cadena de caracteres. Este se hace utilizando el operador de rebanada, que es el signo de `:` . La sintaxis se vería algo así:
>- lista\[inicio:fin:paso]
>- cadena\[inicio:fin:paso]

Donde "inicio" es el índice del primer elemento s incluir en la rebanada, "fin" es el índice del último elemento a incluir en la rebanada y "paso" es la cantidad de elementos que se saltaran entre cada elemento incluido en la rebanada. Si no se indica el "inicia" se asumirá que es 0 (start). Si no se especifica "fin" se asumirá que este será el ultimo índice (end) de la lista o cadena de caracteres. Si no se especifica el "paso" se asumirá que es 1. Ejemplos de rebanadas (Se tomara en los ejemplos una lista básica aunque se pueden aplicar también sobre cadenas de texto):

Si queremos extraer los elementos del índice 2 al índice 6 (sin incluir el elemento del índice 6), podemos hacer lo siguiente:
```python
numeros = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

rebanada = numeros[2:6]
print(rebanada)
```

Si queremos extraer los elementos del índice 0 al índice 9, pero saltándonos de 2 en 2, podemos hacer lo siguiente: 
```python
numeros = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

rebanada = numeros[0:10:2]
print(rebanada)
```

Ahora vamos a poner un ejemplo con cadenas de caracteres, si queremos extraer los caracteres del índice 2 al índice 6 (sin incluir el 6), podemos hacer lo siguiente:

```python
cadena = "Hola mundo"

rebanada = cadena[2:6]
print(rebanada)
```

Si queremos extraer los caracteres del índice 0 al índice 9, pero saltándonos de 2 en 2, podemos hacer lo siguiente:

```python
cadena = "Hola mundo"

rebanda = cadena[0:10:2]
print(rebanada)
```

---

## Funciones

Hasta ahora hemos utilizado funciones muy básicas como el `input( )` o el `print( )` . También hemos visto algunos métodos, que son un tipo de función pero declarados de manera muy especifica.

Cuando un programa repite muchas veces un mismo trozo de código puede ser frustrante pero para ellos podemos crear nuestras propias funciones de esos códigos e importarlas y usarlas en nuestro programa facilitando el trabajo y evitando el error humano de la repetición.

##### \- Procedencia de las funciones 

Generalmente las funciones pueden provenir de tres sitios:
- De **Python** mismo: entre ellas funciones como `print( )` y siempre que programemos en Python estarán disponibles.
- De los **módulos preinstalados** de Python: muchas de las funciones, las cuales comúnmente son menos utilizadas que las integradas, están disponibles en módulos instalados juntamente con Python; para poder utilizar estas funciones el programador debe realizar algunos pasos adicionales (se explicará acerca de esto en un momento).
- **Directamente del código**: tu puedes escribir tus propias funciones, colocarlas dentro del código, y usarlas libremente.

##### \- Crear una función

Imagina que el siguiente código esta repetido decenas de veces en un programa y tu jefe te pide que cambies la cadena de texto si hacemos una función de el con cambiar el código de la función se aplicara en todos los sitios que referencien a esta función.

```python
print("Ingresa un valor")
a = int(input() )
```

Para convertir ese código en una función utilizamos `def` una definición simple se vería así:

```python
def function_name():
	function_body
```

>[!important]
>No es necesario marcarle un argumento a la función si miras el siguiente punto hay dos ejemplos uno con argumento y otro sin 

Si definimos el ejemplo se vería algo así: 

```python
def message():
	print("Ingresa un valor: ")
	a = int(input() )
	print(a)
 
message()
```

Un esquema básico de función seria así:

![[Pasted image 20230710230904.png]]

El proceso sería algo así:
- Cuando se **invoca** una función, Python recuerda el lugar donde esto ocurre y _salta_ hacia dentro de la función invocada.
- El cuerpo de la función es entonces **ejecutado**.
- Al llegar al final de la función, Python **regresa** al lugar inmediato después de donde ocurrió la invocación.

>[!danger]
>No se debe invocar una función antes de definirlo, recordar que Python lee en orden de arriba a abajo si aun no ha leído la definición de la función n o sabrá interpretarlo y dará un error 

>[!danger]
>Una función y una variable no pueden compartir el mismo nombre

##### \- Funciones parametrizadas 

El potencial completo de las funciones se revela cuando las parametrizamos, un parámetro es una variable pero existen dos factores que hacen a un parámetro diferente:
- **Los parámetros solo existen dentro de las funciones en donde han sido definidos**, y el único lugar donde un parámetro puede ser definido es entre los paréntesis después del nombre de la función, donde se encuentra la palabra reservada `def`.
- **La asignación de un valor a un parámetro de una función se hace en el momento en que la función se manda llamar o se invoca**, especificando el argumento correspondiente.

>[!quote]
>- **Los parámetros solo existen dentro de las funciones** (este es su entorno natural).
>- **Los argumentos existen fuera de las funciones**, y son los que pasan los valores a los parámetros correspondientes.

Ejemplo con argumento:

```python
def message(number):
	print("Ingresa un número:", number)

message(2)
```

Es posible tener una variable con el mismo nombre que un argumento iran de manera independiente ya que para que la función nos diese la vriable stendriamos que indicarle la variable en el argumento a la hora de la llamada si no no se tomara en cuenta

```python
number = 10

def message(number):
	print("Ingresa un número:", number)

message(2)

message(number)
```

>[!info] Sombreado
>- El parámetro `x` sombrea cualquier variable con el mismo nombre, pero...
>- ... solo dentro de la función que define el parámetro.

La cantidad de parámetros que puede tener una función es ilimitado pero cuantos mas parámetros tenga una función mas difícil será memorizar su rol y propósito. 

>[!example] Ejemplo función con 2 parámetros 
>```python
>def message(what, number):
>	print("Ingresa", what, "número", number)
>
>message("teléfono", 1)
>message("precio", 5)
>message("número", "número")
>```

##### \- Paso de parámetros posicionales

La técnica que asigna cada argumento al parámetro correspondiente, es llamada **paso de parámetros posicionales**, los argumentos pasados de esta manera son llamados argumentos posicionales.

```python
def introduction(first_name, last_name):

print("Hola, mi nombre es", first_name, last_name)

introduction("Luke", "Skywalker")

introduction("Jesse", "Quick")

introduction("Clark", "Kent")
```

```python
def introduction(first_name, last_name):

print("Hola, mi nombre es", first_name, last_name)

introduction("Skywalker", "Luke")

introduction("Quick", "Jesse")

introduction("Kent", "Clark")
```

Aquí podemos ver como la posición original al marcar los argumentos lo define la posición de estos y si lo ponemos al revés sale al revés. 

##### \- Paso de argumentos con palabras clave

Python ofrece otra manera de pasar argumentos, donde **el significado del argumento está definido por su nombre**, no su posición, a esto se le denomina **paso de argumentos con palabra clave**.

```python
def introduction(first_name, last_name):

	print("Hola, mi nombre es", first_name, last_name)

introduction(first_name = "James", last_name = "Bond")

introduction(last_name = "Skywalker", first_name = "Luke")
```

Si al llamar a la función en vez de poner los argumentos sin mas y se marque por su posición, podemos utilizar una igualdad. 

>[!fail] Argumento inexistente 
>Si hacemos una igualdad as un argumento no definido en la función nos devolverá un error

>[!info]
>Claro esta que estos dos últimos puntos son combinables puedes poner algunos argumentos por igualdad y otros de manera posicional  

También podemos marcar opciones por defecto en una función por ejemplo con algo simple como un apellido muy común:

```python
def present(first_name, last_name="Gonzalez"):
	print("Hola, mi nombre es", first_name, last_name)

present("Juan", "Carlos")
present("Juan") #Aquí no marcamos el segundo argumento lo que nos usara el definido antes
```

#### \- Efectos y resultado: la instrucción 

Todo lo visto de crear funciones nos han dado algún tipo de efecto como imprimir un texto en la consola, pero las funciones también nos pueden entregar un resultado (al igual que lo hace una operación matemática por ejemplo) para lograr esto utilizamos la función `return` 

###### \- Return sin una expresión

Cuando este se utiliza dentro de una función, provocara la terminación inmediata de la ejecución de la función, y un retorno instantáneo al punto de invocación.

```python
def happy_new_year(wishes = True):
    print("Tres...")
    print("Dos...")
    print("Uno...")
    if not wishes:
        return
    
    print("¡Feliz año nuevo!")

input("Pon True o False segun si es tu cumple o no")

happy_new_year(wishes = True)
```

###### \- Return con una expresión 

Esta variante esta extendida con una **expresión**:

```python
def function():
	return expression  
```

Existen dos consecuencias de utilizarlo:
- Provoca la terminación inmediata de la ejecución de la función (Común con el primer tipo de `return`)
- Además, la función evaluará el valor de la expresión y lo devolverá como el resultado de la función.

```python
def boring_function():

	return 123

x = boring_function()

print("La función boring_function ha devuelto su resultado. Es:", x)
```

Su estructura se podría definir visualmente de la siguiente manera:

![[Pasted image 20230711021035.png]]

En resumen `return` con expresión "transporta" el valor de la expresión al lugar donde se ha invocado la función.

>[!tip] Importante
>- Siempre se te **permite ignorar el resultado de la función** y estar satisfecho con el efecto de la función (si la función tiene alguno).
>- Si una función intenta devolver un resultado útil, debe contener la segunda variante de la instrucción `return`.

#### \- El _none_

El valor `none` es un valor que significa nada un ejemplo para ver como lo toma Python es hacer una suma en la qué uno de los dos sumandos sea `none` esto nos dará un error.

>[!info] Circunstancias para `none`
>- Cuando se le asigna a una variable (o se devuelve como resultado de una función)
>- Cuando se compara con una variable para diagnosticas su estado interno

Un ejemplo podría ser:

```python
value = None

if value is None:

print("Lo siento, no contienes ningún valor")
```

>[!danger] Nota
>No olvides que si una función no devuelve un valor utilizando `return`, se asume que devuelve `None` automaticamente

##### \- Ejemplo con none

Aquí hemos definido una función que reporta un `True` si el numero es par:

```python
def strange_function(n):
	if (n % 2 == 0):
		return True

print(strange_function(2))

print(strange_function(1))
```

#### \- Listas y funciones 

Podemos enviar una lista a una función como un argumento, un ejemplo podría ser el siguiente (Programa sumatorio de una lista): 

```python
def sumatori(lst):
	s = 0
	for elem in lst:
		s += elem

	return s

print(sumatori([5, 4, 3]))
```

También una lista puede ser el resultado de una función, aquí tenemos un código que nos pide dándole un número a la función esta nos devolverá una lista con la cantidad de números indicado:

```python
def strange_list_fun(n):
	strange_list = []

	for i in range(0, n):
		strange_list.insert(0, i)
	return strange_list

print(strange_list_fun(5))
```

#### \- Funciones y sus alcances

El alcance de un nombre es la parte de código donde el nombre es reconocido correctamente, por ejemplo el alcance del parámetro de una función es la función es sí. Se puede apreciar en el siguiente ejemplo:

```python
def scope_test():
	x = 123

scope_test()
print(x)
```

>[!Warning] 
>En un editor de código normal cuando hagamos este código nos devolvería un error si lo creemos en las notas de Obsidian nos da bien pero no es correcto para que eso fuese así deberíamos especiar que la variable es global de la siguiente manera: 
>```python
>def scope_test():
>	global x
>	x = 123
>```

Al igual que esto si ponemos el siguiente código en [[Visual Code Shortcuts|Visual]] podemos ver que una variable que se indique en el programa fuera de la función no afectara a esta

```python
def scope_test():
	x = 123
	print(x)

x = 200
print(x)
scope_test()
```

>[!info]
>Es importante decir que los cambios hechos sobre el argumento dentro de la definición de la función no afectara fuera.
>```python
>def my_function(n):
>	print("Yo recibí", n)
>	n += 1
>	print("Ahora tengo", n)
>
>var = 1
>my_function(var)
>print(var)
>```


#### \- Recursividad

Un buen ejemplo de recursividad seria los factoriales, una función para ello sería lo siguiente:

```python
def factorial_function(n):
    if n < 0:
        return None
    if n < 2:
        return 1
    return n * factorial_function(n - 1)

print(factorial_function(5))
```

#### \- Funciones simples ejemplos

##### \- IMC

```python
def IMC(weight, height):
	return weight/height ** 2

print(IMC(94 , 1.75))
```

##### \- Verificador de triángulos

```python
def is_a_triangle(a,b,c):
	if a + b <= c or b + c <= a or c + a <= b:
		return False
	return True

a = input("Escriba el lado a del triangulo:",)
b = input("Escriba el lado b del triangulo:",)
c = input("Escriba el lado c del triangulo:",)

print(is_a_triangle(a,b,c))
```

##### \- Evaluando el área de un triangulo

También es posible evaluar el área de un triangulo. La formula de Heron será útil aquí:

```python
def is_a_triangle(a, b, c):
    return a + b > c and b + c > a and c + a > b


def heron(a, b, c):
    p = (a + b + c) / 2
    return (p * (p - a) * (p - b) * (p - c)) ** 0.5


def area_of_triangle(a, b, c):
    if not is_a_triangle(a, b, c):
        return None
    return heron(a, b, c)


print(area_of_triangle(1., 1., 2. ** .5))


```

>[!abstract] Puntos clave
>1. Una función puede invocar otras funciones o incluso a sí misma. Cuando una función se invoca a si misma, se le conoce como **recursividad**, y la función que se invoca a si misma y contiene una condición de terminación (la cual le dice a la función que ya no siga invocándose a si misma) es llamada una función **recursiva**.
>
>2. Se pueden emplear funciones recursivas en Python para crear funciones **limpias, elegantes, y dividir el código en trozos más pequeños**. Sin embargo, se debe tener mucho cuidado ya que es **muy fácil cometer un error y crear una función la cual nunca termine.** También se debe considerar que **las funciones recursivas consumen mucha memoria**, y por lo tanto pueden ser en ocasiones ineficientes.

---
## Tuplas y diccionarios

Antes de explicar los diccionarios y las tuplas se deben introducir dos conceptos importantes:
- **Tipos de secuencia**: es un tipo de dato en Python el cual es capaz de almacenar más de un valor (o ninguno si la secuencia estuviese vacía), los cuales pueden ser secuencialmente examinados. Las secuencia es un tipo de dato que puede ser escaneado por el bucle `for`. La lista es un ejemplo de secuencia aunque hay mas tipos
- **Mutabilidad**: es una propiedad de cualquier tipo de dato en Python que describe su disponibilidad para poder cambiar libremente durante la ejecución de un programa. En Python hay dos tipos de datos los **mutables** y los **inmutables** 
	- Los datos **Mutables** pueden ser actualizados libremente en cualquier momento, a esta operación se le denomina ***in situ*** (***In situ*** es una expresión del Latín que se traduce literalmente como en posición, en el lugar o momento. Por ejemplo, la siguiente instrucción modifica los datos "in situ")
		``` list.append(1)```
	- Los datos **Inmutables** no pueden ser modificados de esta manera, imagina que una lista solo puede ser asignada y leída. No podrías adjuntar ni remover un elemento de la lista. Si se agrega un elemento al final de la lista provocaría que la lista se cree desde cero. Se tendría que crear una lista nueva, la cual contenga los elemento ya existentes más el nuevo elemento. La **tupla** es una secuencia inmutable, se puede comportar como una lista pero no puede ser modificada en el momento.

#### \- Tuplas

Lo primero que distingue una _lista_ de una _tupla_ es la sintaxis empleada para crearlas. Las tuplas utilizan paréntesis, mientras que las listas usan corchetes , aunque también es posible crear una tupla tan solo separando los valores por comas.

```python
tuple_1 = (1, 2, 4, 8)
tuple_2 = 1., .5, .25, .125
```

Si las imprimimos se ven así:

```python
tuple_1 = (1, 2, 4, 8)
tuple_2 = 1., .5, .25, .125

print(tuple_1)
print(tuple_2)
```

También es posible crear una tupla vacía:
```python
tuple = ()
```

Si se desea crear una tupla de un solo elemento, se debe de considerar el hecho de que, debido a la sintaxis (una tupla debe de poder distinguirse de un valor entero ordinario ), se debe de colocar una coma al final:

```python
one_element_tuple_1 = (1, )
one_element_tuple_2 = 1., 
```

> El quitar las comas no arruinará el programa en el sentido sintáctico, pero serán dos variables, no tuplas

##### \-  Como utilizar una tupla 

Si deseas leer los elementos de una tupla, lo puedes hacer de la misma manera que se hace con las listas

```python
my_tuple = (1, 10, 100, 1000)

print(my_tuple[0])
print(my_tuple[-1])
print(my_tuple[1:])
print(my_tuple[:-2])

for elem in my_tuple:
    print(elem)
```

>[!danger]
>Todas estas instrucciones (con excepción de la primera) nos causara error de ejecución ya que una tupla no puede ser editada durante la ejecuciónç
>
>my_tuple = (1, 10, 100, 1000)
>
>my_tuple.append(10000) 
>del my_tuple[0] 
>my_tuple[1] = -10

Entre otras cosas en las tuplas podemos:
- Utilizar la función `len()` acepta tuplas, y regresa el número de elementos contenidos dentro.
- El operador `+` puede unir tuplas (ya se ha mostrado esto antes).
- El operador `*` puede multiplicar las tuplas, así como las listas. 
- Los operadores `in` y `not in` funcionan de la misma manera que las listas 

En el siguiente código podemos apreciar lo anterior dicho: 

```python
my_tuple = (1, 10, 100)

t1 = my_tuple + (1000, 10000)
t2 = my_tuple * 3

print(len(t2))
print(t1)
print(t2)
print(10 in my_tuple)
print(-10 not in my_tuple)
```

Una propiedad de las tuplas muy útil es que pueden aparecer en el lado izquierdo del operador de asignación. Observa el siguiente código:

```python
var = 123

t1 = (1, )
t2 = (2, )
t3 = (3, var)

t1, t2, t3 = t2, t3, t1

print(t1, t2, t3)
```

>[!tip]
>Este ejemplo nos enseña algo importante y es que los elementos de una tupla pueden ser variables, no solo literales. Además, pueden ser expresiones si se encuentran en el lado derecho del operador de asignación

#### \- Diccionarios 

El **diccionario** es otro tipo de estructura de datos en Python. No es una secuencia ( pero puede adaptarse fácilmente a un procesamiento secuencial) y además es mutable. Para entender que es un  diccionario en Python es importante comprender de manera literal lo que es un **diccionario**. 

Un diccionario en Python funciona de la misma manera que un diccionario bilingüe. Por ejemplo, se tiene la palabra en español "gato" y se necesita su equivalente en francés. Lo que se haría es buscar en el diccionario para encontrar la palabra "gato". Eventualmente la encontrarás, y sabrás  que la palabra equivalente en francés es "chat".

![[Pasted image 20230711060640.png]]

En el mundo de Python la palabra que se esta buscando se le denomina `clave(key)`. La palabra que se obtiene del diccionario es denominada `valor`. Esto significa que un diccionario es un conjunto de pares de `claves` y `valores`. 

>[!note]
>- Cada clave debe ser única. No se puede tener una clave duplicada.
>- Una clave puede ser un tipo de dato de cualquier tipo: puede ser un número, o incluso una cadena.
>- Un diccionario no es una lista. Una lista contiene un conjunto de valores numerados, mientras que un diccionario 
>- La función `len()` aplica también para los diccionarios, regresa la cantidad de pares (clave - valor) en el diccionario
>- Un diccionario es una herramienta de un solo sentido. Si fuese un diccionario español-francés, podríamos buscar en español para encontrar su contraparte en francés más no viceversa.

##### \- Crear un diccionario 

Para asignar algunos pares a un diccionario se haría de la siguiente manera: 

```python
dictionary = {"gato" : "chat", "perro" : "chien", "caballo" : "cheval"}
phone_numbers = {'jefe' : 5551234567, 'Suzy' : 2265784310}
empty_dictionary = {}

print(dictionary)
print(phone_numbers)
print(empty_dictionary)
```

En este primer ejemplo, el diccionario emplea claves y valores las cuales ambas son cadenas. En el segundo, las claves con cadenas pero los valores son enteros. El orden inverso (claves --> números, valores --> cadenas) también es posible, así como la combinación número a número. 

La lista de todos los pares es **encerrado con llaves**, mientras que los pares son **separados por comas**, y las **claves y valores por dos puntos**. El primer diccionario es muy simple, es un diccionario Español - Francés. El segundo es un directorio telefónico muy pequeño. Los diccionarios vacíos son construidos por **un par vacío de llaves** - nada inusual. 

>[!note]
>Primeramente, recordemos que **los diccionarios no son listas** - no guardan el orden de sus datos, el orden no tiene significado (a diferencia de los diccionarios reales). El orden en que un diccionario **almacena sus datos esta fuera de nuestro control**. Esto es normal. 

##### \- Como utilizar un diccionario 

Si deseas obtener cualquiera de los valores, debes de proporcionar una clave válida:

```python
print(dictionary['gato'])
print(phone_numbers['Suzy'])
```

Obtener un valor de un diccionario es semejante a la indexación, gracias a los corchetes alrededor  
del valor de la clave.

>[!note]
>- Si una clave es una cadena, se tiene que especificar como una cadena.
>- **Las claves son sensibles a las mayúsculas y minúsculas**: 'Suzy' seria diferente a 'suzy'

>[!danger] 
>Si reclamamos una clave inexistente el programa nos dará error 

Pero si quisiésemos ver si una palabra se encuentra en el diccionario podemos buscarla con el operador `in`, junto con su acompañante `not in`. Aquí tenemos un código que busca palabras en francés en un diccionario: 

```python
dictionary = {"gato" : "chat", "perro" : "chien", "caballo" : "cheval"}
words = ['gato', 'león', 'caballo']

for word in words:
    if word in dictionary:
        print(word, "->", dictionary[word])
    else:
        print(word, "no está en el diccionario")
```

##### \- Método keys()

Si nosotros itermaos sobre un diccionario con un bucle for este iterara sobre el valor de la izquierda  de cada par si quisiesemos referirnos al segundo podemos utilizar el `.keys()` y el diccionario[key]

```python
dictionary = {"gato" : "chat", "perro" : "chien", "caballo" : "cheval"}

for key in dictionary.keys():
	print (key, "-->", dictionary[key])

```

##### \- La función sorted()

Si queremos que los diccionarios se impriman ordenador podemos aplicarles la función sorted( ) de la siguiente manera:

```python
dictionary = {"gato" : "chat", "perro" : "chien", "caballo" : "cheval"}

for key in sorted(dictionary.keys()):
	print (key, "-->", dictionary[key])

```

Esto nos lo imprimirá de manera ordenada alfabéticamente

##### \- items()

Otra manera de hacerlo es utilizar el método `items()`. Este método **regresa una lista de tuplas** (este es el primer ejemplo en el que las tuplas son mas que un ejemplo de si mismas) **donde cada tupla es un par de cada clave con su valor**. Se vería algo así:

```python
dictionary = {"gato" : "chat", "perro" : "chien", "caballo" : "cheval"} 
for spanish, french in dictionary.items(): 
	print(spanish, "->", french)
```

El `for` itera sobre las tuplas que genera el `items()` 

##### \- values()

También existe un método denominado `values()`, funciona de una manera muy similar al de `keys()`, pero regresa una lista de valores. Un ejemplo sencillo:

```python
dictionary = {"gato" : "chat", "perro" : "chien", "caballo" : "cheval"} 
for french in dictionary.values(): 
	print(french)
```

Como el diccionario no es capaz de automáticamente encontrar la clave de un valor dado, el rol de este método es algo limitado. 

##### \- Como cambiar valores en un diccionario

El asignar un nuevo valor a una clave existiendo es sencillo, debido a que los diccionarios son completamente **mutables**, no existen obstáculos para modificarlos. En el siguiente ejemplo remplazamos un valor por otro:

```python
dictionary = {'gato' : 'minou', 'perro' : 'chien', 'caballo' : 'cheval'}

dictionary['gato'] = 'minou'
print(dictionary)
```

##### \- Agregar nuevas claves a un diccionario

El agregar una nueva clave con su valor a un diccionario es tan simple como cambiar un valor. Solo tienes que asignar una clave a un valor que no haya exista en ese diccionario.

>[!info] Nota
>Este comportamiento es muy distinto al de las listas, las cuales no permiten asignar valores a índices no existentes

A continuación un ejemplo en el que se agrega un par nuevo al diccionario: 

```python
dictionary = {"gato" : "chat", "perro" : "chien", "caballo" : "cheval"}

dictionary['cisne'] = 'cygne'
print(dictionary)
```

Esto también es posible utilizando el método `update()`, por ejemplo:

```python
dictionary = {"gato" : "chat", "perro" : "chien", "caballo" : "cheval"}

dictionary.update({"pato" : "canard"})
print(dictionary)
```

##### \- Eliminar una clave de un diccionario 

>[!note] 
>Cabe decir que al eliminar la clave también se removerá el valor asociado. Ya que los valores no pueden existir sin sus clvaes

Esto se puede hacer con la instrucción `del`. Se vería de la siguiente forma:

```python

dictionary = {"gato" : "chat", "perro" : "chien", "caballo" : "cheval"}

del dictionary['perro']
print(dictionary)
```

Si quisiésemos eliminar el ultimo elemento del diccionario podemos utiliza el método `popitem()`:

```python 
dictionary = {"gato" : "chat", "perro" : "chien", "caballo" : "cheval"}

dictionary.popitem()
print(dictionary)
```

>[!warning] 
>En versiones anteriores de Python, por ejemplo antes de las 3.6.7, el método `popitem()` elimina un elemento al azar del diccionario.

#### \- Las tuplas y los diccionarios pueden trabajar juntos

Para ver esto vamos a poner un ejemplo sencillo, mostrando como las tuplas y los diccionarios pueden trabajar juntos. Imaginemos el siguiente ejemplo:

- Necesitas un programa para calcular los promedios de tus alumnos.
- El programa pide el nombre del alumno seguido de su calificación.
- Los nombres son ingresados en cualquier orden.
- El ingresar un nombre vacío finaliza el ingreso de los datos (nota 1: ingresar una puntuación vacía generará la excepción ValueError, pero no te preocupes por eso ahora, verás cómo manejar tales casos cuando hablemos de excepciones en el segundo parte de la serie del curso).
- Una lista con todos los nombre y el promedio de cada alumno debe ser mostrada al final.

El código se vería algo así: 

```python
school_class = {}

while True:
    name = input("Ingresa el nombre del estudiante: ")
    if name == '':
        break
    
    score = int(input("Ingresa la calificación del estudiante (0-10): "))
    if score not in range(0, 11):
	    break
    
    if name in school_class:
        school_class[name] += (score,)
    else:
        school_class[name] = (score,)
        
for name in sorted(school_class.keys()):
    adding = 0
    counter = 0
    for score in school_class[name]:
        adding += score
        counter += 1
    print(name, ":", adding / counter)
```

Este seria el análisis del código línea por línea:

>- **Línea 1**: crea un diccionario vacío para ingresar los datos: el nombre del alumno es empleado como clave, mientras que todas las calificaciones asociadas son almacenadas en una tupla (la tupla puede ser el valor de un diccionario, esto no es un problema).
>- **Línea 3**: se ingresa a un bucle "infinito" (no te preocupes, saldremos de el en el momento indicado).
>- **Línea 4**: se lee el nombre del alumno aquí.
>- **Línea 5-6**: si el nombre es una cadena vacía (), salimos del bucle.
>- **Línea 8**: se pide la calificación del estudiante (un valor entero en el rango del 1-10).
>- **Línea 9-10**: si la puntuación ingresada no está dentro del rango de 0 a 10, se abandona el bucle.
>- **Línea 12-13**: si el nombre del estudiante ya se encuentra en el diccionario, se alarga la tupla asociada con la nueva calificación (observa el operador +=).
>- **Línea 14-15**: si el estudiante es nuevo (desconocido para el diccionario), se crea una entrada nueva, su valor es una tupla de un solo elemento la cual contiene la calificación ingresada.
>- **Línea 17**: se itera a través de los nombres ordenados de los estudiantes.
>- **Línea 18-19**: inicializa los datos necesarios para calcular el promedio (sum y counter).
>- **Línea 20-22**: se itera a través de la tupla, tomado todas las calificaciones subsecuentes y actualizando la suma junto con el contador.
>- **Línea 23**: se calcula e imprime el promedio del alumno junto con su nombre.

---
## Errores 

#### \- Error dato que no debería ser

Con el siguiente programa de ejemplo podemos ver que al entregarle un número natural al programa este nos devuelve su reciproco. Es decir un `2` se convertirá en `0.5` (1/2) y `4` en `0.25`. El programa será el siguiente:

```python
value = int(input("Ingresa el número  natural: ", ))
print("El recíproco de", value, "es", 1/value)
```

Esto nos puede dar problemas por que si el usuario nos entregase un número decimal, el programa nos entregaría un error como el siguiente: 

```python
Traceback (most recent call last):
	File "code.py", line 1, in
		value = int(input("Ingresa un número natural: "))
ValueError: invalid literal for int() with base 10: " "
```

Si analizamos este error podemos que todas las líneas son significativas pero la última línea parece ser la más valiosa, en esta ultima error la primera palabra nos indica el nombre de la excepción  la cual provoca que el código se detenga. En este caso su nombre es `ValueError`. El resto de la línea es una breve explicación que trata de especificar con más precisión la causa de la excepción.

La primera idea puede ser verificar si el número entregado es un número entero y si no lo es negarse a continuar el código esto podríamos hacerlo con el operador `is` y con `type()` de la siguiente manera `type(value) is int`, si integramos esto en el código podríamos verlo así:

```python
value = ("Ingresa el número natural: ", )

if type(value) is int:
	print("El recíproco de", value, "es", 1/value)
else:
	"El número entregado no es natural"
```

Esta podría ser una solución aunque no es la que Python nos recomienda, En la [[Programación orientada a objetos (OOP)]] de Python podremos ver otras maneras de hacer esto.

#### \- Los bloques try y except 

En resumen podríamos describir estos bloques de la siguiente manera:
- La palabra reservada `try` marca un bloque donde intentas hacer algo sin preguntar (puedes escribir algo sin miedo a que de error )
- La palabra reservada `except` comienza un bloque donde puedes pedir perdón(Ósea puedes usar tu segunda oportunidad para decirle al código que hacer en caso de excepción) 

```python
try:
	#codigo
except:
	#codigo
```

Aplicado al ejemplo del anterior punto podríamos hacer lo siguiente:

```python
try:
	value = input("Ingresa un número natural: ")
	print("El reciproco de", value, "es", 1/int(value))
except:
	print("No se que hacer con", value)
```

#### \- Como lidiar con más de una excepción

Por ejemplo sin en el ejemplo el usuario entregase un 0 el programa nos devolverá el error `ZeroDivisionError`, a un `try` le podemos encadenar varios `except`. Un ejemplo podría ser el siguiente:

```python
try:
	value = input("Ingresa un número natural:", )
	print("El recíproco de", value, "es", 1/int(value))
except ValueError:
	print("No se que hacer con", value)
except ZeroDivisionError:
	print("La división entre cero es matematicamente imposible")
```

Lo que pasa con este código es que no aprecia que pueda salir un error fuera de los marcados para ello podemos poner un `except` por defecto que afectara a todas las demás excepciones.

>[!danger]
>Importante el `except` por defecto debe ir siempre el ultimo

```python
try:
	value = input("Ingresa un número natural:", )
	print("El reciproco de", value, "es", 1/int(value))
except ValueError:
	print("No se que hacer con", value)
except ZeroDivisionError:
	print("La división entre cero es matematicamente imposible")
except:
	print("Ha sucedido algo extraño y es imposible la carga del codigo")
```

#### \-  Excepciones útiles

###### \- ZeroDivisionError

Esta aparece cuando intentas forzar a Python a realizar cualquier operación que provoque una división en la que el divisor es cero o no se puede distinguir de cero. Toma cuenta que hay más de un operador de Python que puede hacer que se genere esa excepción. Son los siguientes:

- `/`
- `//`
- `%`

##### \- ValueError

Espera esta excepción cuando estás manejando valores que puedan usarse de manera inapropiada en algún contexto. En general, esta excepción se genera cuando una función como `int()` o `float()` recibe un argumento de un tipo inadecuado, pero su valor es inaceptable.

##### \- TypeError

Esta excepción aparece cuando intentas aplicar un dato cuyo tipo no se puede aceptar en el contexto actual. Mira el ejemplo:

```python 
short_list = [1]
one_value = short_list[0.5]
```

En este caso nos da erro ya que un número de coma flotante no puede ser índice de una lista 

##### \- AttributeError

Esta excepción llega, entre otras ocasiones, cuando intentas activar un método que no existe en un elemento con el que está tratando. Por ejemplo:

```python
short_list = [1]
short_list.append(2)
short_list.depend(3)
```

La tercera línea del ejemplo intenta hacer uso de un método que no esta incluido en las listas. Este es el lugar donde se genera el error `AttributeError`

##### \- SyntaxError

Esta excepción se genera cuando el control llega a una línea de código que viola la gramática de Python. Puede sonar extraño, pero algunos errores de este tipo no se pueden identificar sin ejecutar primero el código. Este tipo de comportamiento es típico de los lenguajes interpretados: el intérprete siempre trabaja con prisa y no tiene tiempo para escanear todo el código fuente. Se conforma con comprobar el código que se está ejecutando en el momento. 

Estos errores no es recomendable manejarlos con excepciones, debes producir tu código sin errores de sintaxis, en lugar de tratar enmascarar las fallas que has causado.

#### \-  Rastreando las rutas de ejecución 

En nuestro código de ejemplo podemos rastrear tres rutas de ejecución independientes en el código, sentenciadas por `if-elif-else`. Por supuesto, las rutas de ejecución puede contribuirse mediante muchas otras sentencias como bucles, o incluso bloque como `try-except`.

```python
temperature = float(input('Ingresa la temperatura actual:'))

if temperature > 0:
    print("Por encima de cero")
elif temperature < 0:
    print("Por debajo de cero")
else:
    print("Cero")
```

En este código se ve como para evitar errores hemos hecho un código que aprecie las opciones que podría poner el usuario, esto es importante de hacer para ello deberemos apreciar las opciones y tener en cuenta que rutas de ejecución necesitamos. 

```python
temperature = float(input('Ingresa la temperatura actual:'))

if temperature > 0:
    print("Por encima de cero")
elif temperature < 0:
    prin("Por debajo de cero")
else:
    print("Cero")
```

Como podemos ver si no ponemos un input negativo el programa no da error.

La respuesta es más simple de lo esperado y también un poco decepcionante. Python, como seguramente sabes, es un lenguaje **interpretado**. Esto significa que el código fuente se analiza y ejecuta al mismo tiempo. En consecuencia, es posible que Python no tenga tiempo para analizar las líneas de código que no están sujetas a ejecución. Como dice un antiguo dicho de los desarrolladores: "es una característica, no un error" (no utilices esta frase para justificar el comportamiento extraño de tu código).

¿Entiendes ahora por qué el pasar por todos los caminos de ejecución es tan vital e inevitable?

Supongamos que terminas tu código y que las pruebas que has realizado son exitosas. Entregas tu código a los probadores y, ¡afortunadamente! - encontraron algunos errores en él. Estamos usando la palabra "afortunadamente" de manera completamente consciente. Debes aceptar que, en primer lugar, los probadores son los mejores amigos del desarrollador; no debes tratar a los errores que ellos encuentran como una ofensa o una malignidad; y, en segundo lugar, cada error que encuentran los probadores es un error que no afectará a los usuarios. Ambos factores son valiosos y merecen tu atención.

Ya sabes que tu código contiene un error o errores (lo segundo es más probable). Ahora, ¿Cómo los localizas y cómo arreglas tu código?

Aquí entran en juego cosas como la depuración si quieres saber algo más sobre ello ve [[0100 - Fundamentos#Error frente a depuración (Bug vs. debug)|aquí]].

---

# Python intermedio
#programming 

---

## Módulos 

### \- Que es un módulo

El código de computadora tiene una tendencia a crecer. Podemos decir que el código que no crece probablemente sea completamente inutilizable o esté abandonado. Un código real, deseado y ampliamente utilizado se desarrolla continuamente, ya que tanto las demandas de los usuarios como sus expectativas se desarrollan de manera diferente.

Un código que no puede responder a las necesidades de los usuarios se olvidará rápidamente y se reemplazará instantáneamente con un código nuevo, mejor y más flexible. Se debe estar preparado para esto, y nunca pienses que tus programas están terminados por completo. La finalización es un estado de transición y generalmente pasa rápidamente, después del primer informe de error. Python en sí es un buen ejemplo de cómo actúa esta regla.

El código creciente es, de hecho, un problema creciente. Un código más grande siempre significa un mantenimiento más difícil. La búsqueda de errores siempre es más fácil cuando el código es más pequeño (al igual que encontrar una rotura mecánica es más simple cuando la maquinaria es más simple y pequeña).

Además, cuando se espera que el código que se está creando sea realmente grande (puedes usar el número total de líneas de código como una medida útil, pero no muy precisa, del tamaño del código) entonces, se deseará, o más bien, habrá la necesidad de dividirlo en muchas partes, implementado en paralelo por unos cuantos, una docena, varias docenas o incluso varios cientos de desarrolladores.

Por supuesto, esto no se puede hacer usando un archivo fuente grande, el cual esta siendo editado por todos los programadores al mismo tiempo. Esto seguramente conducirá a un desastre.

Si se desea que dicho proyecto de software se complete con éxito, se deben tener los medios que permitan:

- Dividir todas las tareas entre los desarrolladores.
- Después, unir todas las partes creadas en un todo funcional.

Por ejemplo, un determinado proyecto se puede dividir en dos partes principales:

- La interfaz de usuario (la parte que se comunica con el usuario mediante widgets y una pantalla gráfica).
- La lógica (la parte que procesa los datos y produce resultados).

Cada una de estas partes se puede (muy probablemente) dividir en otras más pequeñas, y así sucesivamente. Tal proceso a menudo se denomina **descomposición**.

Por ejemplo, si te pidieran organizar una boda, no harías todo tu mismo: encontrarías una serie de profesionales y dividirías la tarea entre todos.

¿Cómo se divide una pieza de software en partes separadas pero cooperantes? Esta es la pregunta. Los **módulos** son la respuesta.

### \- Como hacer uso de un módulo 

Entonces, ¿qué es un módulo? El Tutorial de Python [](https://docs.python.org/3/tutorial/modules.html)lo define como **un archivo que contiene definiciones y sentencias de Python**, que se pueden importar más tarde y utilizar cuando sea necesario.

El manejo de los módulos consta de dos cuestiones diferentes:
- El primero (probablemente el más común) ocurre cuando se desea utilizar un módulo ya existente, escrito por otra persona o creado por el programador mismo en algún proyecto complejo: en este caso, se considera al programador como el **usuario** del módulo.
- El segundo ocurre cuando se desea crear un nuevo módulo, ya sea para uso propio o para facilitar la vida de otros programadores: aquí tu eres el **proveedor** del módulo.

Discutamos ambos por separado.
En primer lugar, un módulo se identifica por su **nombre**. Si se desea utilizar cualquier módulo, se necesita saber su nombre. Se entrega una cantidad (bastante grande) de módulos junto con Python. Se puede pensar en ellos como una especie de "equipamiento adicional de Python".

Todos estos módulos, junto con las funciones integradas, forman la **Biblioteca Estándar de Python** - un tipo especial de biblioteca donde los módulos desempeñan el papel de libros (incluso podemos decir que las carpetas desempeñan el papel de estanterías). Si deseas ver la lista completa de todos los "volúmenes" recopilados en esa biblioteca, se puede encontrar aquí
[https://docs.python.org/3/library/index.html](https://docs.python.org/3/library/index.html).

Cada módulo consta de entidades (como un libro consta de capítulos). Estas entidades pueden ser funciones, variables, constantes, clases y objetos. Si se sabe como acceder a un módulo en particular, se puede utilizar cualquiera de las entidades que almacena.

![Accediendo al módulo: math](https://edube.org/uploads/media/default/0001/02/PE2_source_file_ESP_1.1.1.2_2_ESP_PE2_.png)

Comencemos la discusión con uno de los módulos más utilizados, el que lleva por nombre `math`. Su nombre habla por sí mismo: el módulo contiene una rica colección de entidades (no solo funciones) que permiten a un programador implementar efectivamente cálculos que exigen el uso de funciones matemáticas, como _sen()_ o _log()_.

### \- Importando un módulo 

#### \- Método 1

Para que un módulo sea utilizable deberemos **importarlo**. La importación de un módulo se realiza mediante una instrucción llamada `import`. 

>[!danger]
>Recordad que `import` es una palabra reservada.

Si quisiésemos importar las siguientes entidades de `math`:
- Un símbolo **constante** tan preciso como sea posible utilizando aritmética de punto flotante doble, se suele nombrar con una letra griega pero aquí la trataremos de **pi**
- Una función llamada `sin()` (El equivalente informático de _seno_

Ambas entidades están disponibles en el módulo `math`, pero dependiendo de la forma en que importemos se usaran de manera diferente. La forma más sencilla de importar un módulo es la siguiente:

```python
import math
```

Esta cláusula contiene:
- La palabra reservada `import`
- El nombre del módulo a importar

>[!quote]
>Se puede importar un módulo en cualquier parte del código aunque siempre antes del primer uso de cualquiera de las entidades que contenga el módulo. Aunque lo normal es ponerlo al principio del codigo

Se puede repetir la cláusula `import` tantas veces como sea necesario o numerarlas de seguido utilizando comas 

```python
import math
import sys

import math,sys
```

Un termino que debes entender es **namespace**, es un espacio en el que existen algunos nombres y los nombres no entran en conflicto entre sí, es decir, no hay dos objetos diferentes con el mismo nombre. podríamos decir que cada grupo social es un **namespace**, el grupo tiene a nombrar a cada uno de sus miembros de una manera única. Esta singularidad se puede lograr de muchas maneras, por ejemplo mediante el uso de apodos junto con los nombres o asignando identificadores especiales a todos los miembros del grupo.

Dentro de un determinado **namespace**, cada nombre debe permanecer único. Esto puede significar que algunos nombres pueden desaparecer cuando cualquier otra entidad de un nombre ya conocido ingresa al **namespace**. Si el módulo de un nombre especificado existe y es accesible, Python importara su contenido se hacen conocidos todos los nombres definidos en el módulo.

Esto significa que puedes tener tus propias entidades llamadas `sin` o `pi` y no serán afectadas en alguna manera por la importación. Si queremos llamar al `pi` del módulo solo tendremos que llamar al **pi** el cual viene del módulo `math`, solo tendremos que llamar a `pi` con el nombre de módulo original.

Se utilizarían de la siguiente manera:

```python
import math
print(math.sin(math.pi/2))
```

- El nombre del módulo (`math`)
- Un punto
- El nombre de la entidad (`pi`) 

>[!danger]
>El eliminar cualquiera de las dos indicaciones del nombre del módulo hará que el código sea erróneo. No hay otra forma de entrar al namespace de `math` si se hizo lo siguiente:
>```python
>import math
>```

Ahora un ejemplo en el que vemos como pueden coexistir tu namespace y el del modulo:

```python
import math

def sin(x):
	if 2 * x == pi:
		return 0.9999999
	else:
		return None

pi = 3.14

print(sin(pi/2))
print(math.sin(math.pi/2))
```

#### \- Método 2

En el segundo método, la sintaxis del `import` señala con precisión que entidad/es del  módulo son aceptables en el código:

```python
from math import pi
```

La instrucción consta de lo siguiente: 
- La palabra clave reservada `from`
- El **nombre del módulo** a ser (selectivamente) importado
- La palabra clave reservada `import` 
- El **nombre o lista de nombres de la entidad o entidades** las cuales están siendo importadas al **namespace**.

La instrucción tiene este efecto:
- Las entidades listadas son las únicas que son **importadas del módulo indicado**
- Los nombres de las entidades importadas pueden ser accedidas dentro del código sin especificar el nombre del módulo origen.