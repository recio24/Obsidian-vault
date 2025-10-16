
# Ejercicios estática
---
### 1. Calcula las reacciones que aparecen en las uniones para que la barra esté en equilibrio. 
$a =6 m$
$P = 30N$
![[Ejercicio 1.svg]]
$\sum\limits Fx=0$
	$A_{x}=0$
$\sum\limits Fy=0$
	$Ay -P -P =0$ 
$\sum M_{A}=0$
	$M_{A}-(P\cdot a) -(P\cdot 2a)=0$ 
- Podemos formalizar un sistema de ecuaciones de tres incógnitas
$$\huge\begin{cases} Ax=0 \\ Ay -P-P=0 \\ M_{A}-(P\cdot a)-(P\cdot 2a) \end{cases}$$
$Ax$ lo tenemos despejado que es $0$.
$Ay$ lo despejamos:$$Ay-30-30=0 \rightarrow Ay =60N$$
Despejamos $M_{A}$:$$M_{A}= 30\cdot 6 + 30\cdot (2\cdot6)\rightarrow M_{A}=540N_{/M}$$
Los valores de las reacciones serian:$$\begin{align} \huge A_{x}=0 \\ \huge Ay=60N \\ \huge M_{A}=540N_{/M} \end{align}$$

---
### 2. En la siguiente figura se indican las cargas que soporta una viga de 4,8m de longitud. Calcula las reacciones que aparecen en las uniones, esto es, en los puntos A y B.
![[Ejercicio 2.svg]]
- Planteamos las ecuaciones de las reacciones
$\sum\limits Fx=0$
$Bx=0$
$\sum\limits Fy=0$
$F1-F2+F3-F4+Ay+By=0$
$\sum M_{A}=0$
$-F1\cdot 3.8 -Ay \cdot2.8\ +F2\cdot2.2-F3\cdot 1+F4\cdot1=0$ 
- Resolvemos $Bx$:
$Bx =0$
- Despejamos $Ay$ de la ecuación del momento:$$Ay=\frac{150\cdot3.8-600\cdot2.2+100\cdot1+250\cdot1}{-2.8}\rightarrow Ay=143N$$
- Sustituimos en la ecuación de $Fy$ y calculamos $By$:$$By=-150-143+600-100+250=457N$$
- Las reacciones serian:$$\begin{align} \huge B_{x}=0 \\ \huge Ay= 143N \\ \huge By=457N \end{align}$$
---
### 3. La viga BC está unida mediante una articulación a una pared vertical y se mantiene en equilibrio por el cable AC. Calcula la tensión del cable teniendo en cuenta que se aplica una fuerza de 300N en el punto C. La masa de la viga es despreciable.
![[Ejercicio 3.svg]]
- Debemos descomponer el vector $T$ para tener su $Tx$ y $Ty$:
$\huge cos\alpha = \frac{Tx}{T}\rightarrow=Tx=T\cdot cos\alpha$
$\huge sen\alpha = \frac{Ty}{T}\rightarrow=Ty=T\cdot sen\alpha$
- Ahora realizamos los sumatorios de los ejes:
$\sum\limits Fx=0$
$Bx -Tx=0$
$\sum\limits Fy=0$
$By+Ty-F1=0$
$\sum M_{A}=0$
$F1\cdot 45m+Ty\cdot 45m=0$
- Despejamos $Ty$ y calculamos de la ecuación del momento:$$\frac{300N\cdot45}{45}=Ty=300N$$
- Calculamos T con $Ty$:
$$\alpha\rightarrow tg\alpha=\frac{30}{45}\rightarrow\alpha=33.69º$$
$$Ty=T\cdot cos\alpha\rightarrow 300N=T\cdot sen(33.69º)=540.83$$
- Solución:$$T=540.83N$$
---
### 4. Sabiendo que la fuerza vertical $P$ es 400N, Calcula las reacciones del punto C y B.
![[Ejercicio 4.svg]]
- Debemos descomponer C:
$\huge sen\alpha=\frac{Cy}{C}\rightarrow Cy=C\cdot sen\alpha$
$\huge cos\alpha=\frac{Cx}{Cy}\rightarrow Cx=C\cdot cos\alpha$
- Hacemos las sumatorias de las fuerzas:
$\sum\limits Fx=0$
$Px+Bx-Cx=0$
$\sum\limits Fy=0$
$-Py+By-Cy=0$
$\sum M_{A}=0$
- Calculamos Cx y Cy $$\huge \begin{align}cos70º\cdot P=\end{align}$$
- Averiguamos el valor de C:$$160N=C\cdot sen$$

---
### 5. Calcula el valor de P 
![[Ejercicio 5.svg]]
- Hacemos los sumatorios de los ejes:
$\sum\limits Fx=0$
$Bx+Fc+Fd=0$
$\sum\limits Fy=0$
$P+By=0$
$\sum M_{A}=0$
$-P\cdot0,3 +Fc\cdot0,075+Fd\cdot0.155$
- Calculamos P con la formula de Momento:$$\huge -P\cdot0,3+16\cdot9,8\cdot0.075+12\cdot9.8\cdot0.155=102N$$
---
### 6. Una barra de 100kg, tiene cilindros en sus extremos y se mantiene en equilibrio en la posición indicada por la cuerda CD. Calcula las reacciones en los puntos A y B y la tensión de la cuerda CD.

![[Ejercicio 6.svg]]
- Planteamos las ecuaciones:
$\sum\limits Fx=0$
$-Bx +T=0$
$\sum\limits Fy=0$
$Ay-P=0$
$\sum M_{A}=0$
$-T\cdot a-P\cdot b+Bx\cdot c=0$ 
Para marcar la distancia de T al punto A hay que utilizar trigonometría ya que al ser una fuerza horizontal necesitamos su altura vertical. Con la fuerza P necesitamos la distancia horizontal entre P y Ay. Con el punto Bx necesitamos la altura vertical.
$Cos30º=\frac{a}{4}\rightarrow a=3,46m$
$Sen30º=\frac{b}{6}\rightarrow b=3m$
$Cos30º=\frac{c}{12}\rightarrow c=10,4m$
Con lo que la ecuación del momento una vez calculadas las alturas seria:
$-T\cdot 3,46-P\cdot 3+Bx\cdot 10,4=0$
Podemos despejar la ecuación de y despejando Fy:
$Ay-P=0\rightarrow Ay=P=1000N$
Despejamos la primera ecuación
$-Bx+T=0\rightarrow T=Bx$
Sustituimos y despejamos la ultima ecuación del momento averiguando Bx
$-3,46\cdot Bx-3000+10,4Bx=0\rightarrow Bx=\frac{3000}{6,94}=433N$
---
### 11. 
![[Ejercicio 11.svg]]
- Planteamos las ecuaciones:
$\sum\limits Fx=0$
$Ax+Bx=0$
$\sum\limits Fy=0$
$Ay-P-T=0$
$\sum\limits Ma=0$
$+Bx\cdot1,5-P\cdot2-T\cdot6=0$
- Resolvemos las incógnitas conocidas $P$ y $T$
$P=m\cdot g=1000\cdot10=10000N$
$T=2400\cdot10=24000N$
- Despejaos $Ay$ de la ecuación de $Fy$:
$Ay-10000+24000=34000N$
- Despejamos $Bx$:
$1,5Bx=2\cdot10000+6\cdot24000\rightarrow Bx=\frac{164000}{1,5}=109333N$
- Despejamos $Ax$:
$-Ax+109333=0\rightarrow Ax=-109333N$
---
### Ejercicio 13. Calcula las reacciones en los puntos A y B para que la viga este en equilibrio.
![[Ejercicio 13.svg]]
- Planteamos las ecuaciones:
$\sum\limits Fx=0$
$Ax=0$
$\sum\limits Fy=0$
$Ay-F+By=0$
$\sum\limits Ma=0$
$-F\cdot10+By\cdot 15$
- Calculamos el valor de $F$
$F=w\cdot10=74\cdot10=740N$
- Podemos despejas $By$
$-740\cdot10+By\cdot15\rightarrow By=\frac{74100}{15}=493N$
- Despejamos $Ay$
$Ay=f-By\rightarrow Ay=740\cdot493=247N$
---

---
#Elementosdemaquinas 