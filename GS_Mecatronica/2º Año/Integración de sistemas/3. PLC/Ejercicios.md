## Ejercicios
---
### Ejercicio 1. Cuando pulse marcha y la prensa este arriba, prensamos la pieza y cuando llegue abajo la prensa sube hasta llegar arriba.

**OUT**
- Prensa arriba
- Prensa abajo
**INPUT**
- Marcha
- a (Arriba)
- b (Abajo)

![[GS_Mecatronica/2º Año/Integración de sistemas/3. PLC/_ANEXOS_/Ejercicio 1.svg]]

---
### Ejercicio 2. Tras pulsar M1 y M2 y estando los cilindros en su posición retrasada, los cilindros deberían realizar el siguiente ciclo: A+,B+, B-, A-. Tras realizar el último movimiento volverán a la posición inicial. Realizar el Grafcet de 1º. Direccionamiento de las variables y Grafcet de 2º nivel para las opciones A) y B) .

![[GS_Mecatronica/2º Año/Integración de sistemas/3. PLC/_ANEXOS_/Ejercicio 2.svg]]

---

### Ejercicio 3. Debemos controlar la siguiente máquina de estampación: Al accionar sobre la Marcha y estando los tres cilindros retrasados, inicialmente el cilindro A alimenta la pieza. Tras la sujeción el cilindro B realiza la estampación descendiendo. Con B abajo, para que el proceso de estampación se lleve a cabo correctamente, será necesario estar 5 segundos prensando la pieza. Al finalizar el tiempo, B sube y empujamos la pieza al cestón mediante el cilindro C. Finalmente los cilindros C y A retrocederán a la vez. Realizar el Grafcet de 1er nivel, Direccionamiento de Variables, Grafcet de 2º Nivel y Programa de PLC.
![[GS_Mecatronica/2º Año/Integración de sistemas/3. PLC/_ANEXOS_/Ejercicio 3.svg]]

---
### Ejercicio 4. El carro de la imagen se desplaza de un lado a otro trasportando material. El sistema lo componen un pulsador de marcha y 2 sensores de proximidad. El funcionamiento es el siguiente: Para que el carro empiece a moverse se debe pulsar el botón de marcha y se debe encontrar en la posición A. Cuando llegue a la posición B esperará 10 segundos y pasado este tiempo deberá mover hacia la izquierda hasta que llegue al sensor A otra vez. El proceso se repetirá 5 veces y el carro se parará en la posición A una vez completado el ciclo.