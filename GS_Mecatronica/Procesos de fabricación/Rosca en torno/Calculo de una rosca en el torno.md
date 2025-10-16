# Cálculos rosca torno 
---
Rosca $M35$ y paso $1,5$
![[Calculo rosca torno.svg]]
Necesitamos calcular:
- $N$
- $Av$ y selecciones
- Profundidades
1. [[Preparación maquina|Prepararemos la máquina]] en relación a la rosca a realizar.
2. Prepararemos la pieza.$$Diametro\ exterior\ pieza\ preparada= Diametro\ nominal-0,2=35mm-0,2mm=34,8mm$$
3. Preparar herramienta altura y perpendicularidad
4. Calcular la rosca.
a) Calculamos el número de profundizaciones en los tornos de la escuela tenemos una tabla en relación al paso:

| Paso       | n    |
| ---------- | ---- |
| Hasta 1,75 | n=10 |
| 1,75-2     | n=15 |
| Más de 2   | n=20 |
En este caso usaremos $10\ produndizaciones$
b) Calculamos profundidad total rosca:$$\huge H=0,7\cdot P=0,7\cdot 1,5=1,05$$
c) Calculamos primera profundización:$$\huge P_{primera}=\frac{H}{\sqrt{n}}=\frac{1,05}{\sqrt{10}}=0,33$$
d) Calculamos profundizaciones:$$\huge\begin{align}Pn= P_{primera}\cdot\sqrt{n} \\ 
P1= 0,33\cdot\sqrt{1}=0,33\\
P2= 0,33\cdot\sqrt{2}=0,467\\
P3= 0,33\cdot\sqrt{3}=0,572\\
P4= 0,33\cdot\sqrt{4}=0,66\\
P5= 0,33\cdot\sqrt{5}=0,738\\
P6= 0,33\cdot\sqrt{6}=0,808\\
P7= 0,33\cdot\sqrt{7}=0,873\\
P8= 0,33\cdot\sqrt{8}=0,933\\
P9= 0,33\cdot\sqrt{9}=0,99\\
P10= 0,33\cdot\sqrt{10}=1,0\\
\end{align}$$

---
#fabricación 