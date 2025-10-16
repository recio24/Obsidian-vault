# Markdown
#programming

---
## Lenguaje de marcas
![[0100 - Fundamentos#^markdown]]

---
## Formateo del texto
> [!danger] 
> Markdown no permite subrayado para no liarse con los enlaces, ni tener mas de dos líneas en blanco si te fijas las unificara en uno.



## Negrita y cursiva

	**negrita**
	*cursiva*
	***negrita y cursiva***
	___negrita y cursiva___

## Tachado 

	~~tachado~~

## Resaltado

	==resaltado==
---
## Citas y llamadas de atención

> Así marcaríamos una cita:
> 	> seguido del texto

>[!note]  
>	>[!tipo] titulo
>Esto se puede hacer con otros tipos como:

>[!abstract]

>[!info]    

>[!todo]

>[!tip]

>[!success]

  >[!question]
  >

>[!warning]
>

>[!failure]
>

>[!danger]
>

>[!bug]
>

>[!example] 
>

>[!quote]
>

## Insertar un código de programación

> [!quote] Programa ejemplo
> 
> 	``` Nombre del lenguaje
> 	programa
> 	```
> >[!bug] Python
> >``` python
> >print("hola")
> >```
> 

---
## Listas

Podemos hacer listas de varias maneras:
 
 Simples:
> 	-  
 
  - cosa 1
  - cosa 2
  - cosa 3
 
 Numeradas: 
>	X. 

  1. Casa
	  1. Cocina
  2.  Apartamento
	  1. Habitación 1

 Palomitas:
>	 - [ ]

   - [ ] Tarea 1
   - [ ] Tarea 2
   - [ ] Tarea 3

 >[!quote] 
 >Si tabulamos podemos crear subgrupos dentro de los mismos puntos de una lista y aplicar sobre ellos en conjunto

---
## Exclusión de caracteres
> [!info]
> Cuando queramos que un carácter no sea interpretado por Markdown haremos lo siguiente 
> 
>	\-

---
## Enlazar texto

>	Pincha aquí [Texto que queremos enlazar] (enlace)

Si pinchas te llevara a [Google](https://google.com/)

---
## Referencias

^baca73

Las referencias nos sirven para referenciar una nota o parte de ella con otra nota ya sea enlazando un texto o insertándolo podemos seleccionas desde una nota completa a seleccionar por encabezados o por bloques. 

#### Referencia no insertada
[[Markdown]]
Su sintaxis es la siguiente:
```py
[[Nota]] Referencia a nota com pleta
[[Nota#Encabezado]] Referencia a encabezado concreto
[[Nota#Bloque]] Referencia a un bloque concreto

```

#### Referencia insertada 
![[Markdown#Negrita y cursiva]]
```
![[Reglas Markdown#^]] Su sintaxis es igual que en las no insertadas
```

Cuando en la sintaxis utilizamos ^ para referirnos a un bloque también podemos ir antes al bloque y al final añadirle \^nombre y utilizar este como método de referencia 
```
![[nota^nombre]]
```

---


