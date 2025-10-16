# Fabricación aditiva
---
## ¿Que es?
- Fabricación sustractiva: retirar material sobrante hasta conseguir la forma
- Conformado fundición moldeo
**Fabricación aditiva**
Proceso de creación de objetos sólidos en 3D a partir de un archivo digital. El objeto se forma mediante la superposición de capas de material de manera sucesiva. Esta tecnología permite la producción de formas complejas y funcionales optimizando el material. 

---
### Impresión 3d
<font color="#92d050">Ventajas</font>.
- **Diseños complejos**: La complejidad de las piezas no incrementa los costos de fabricación.
- **Personalización**: Permite adpatar los diseños según necesidades.
- **Reducción de material**: Control preciso de la estructura interna.
- **Prototipado rápido y económico**: Agiliza el desarrollo de ideas
- **Producción rápida**
- **Adecuado para lotes pequeños o piezas únicas**
- **Opciones de postprocesado**
#### FDM (Extrusión de material)
Tecnología funciona mediante la adición de material, colocando capas sucesivas hasta completar la pieza
#### SLA (Fotopolimerización)
Consiste en endureces capas de una resina mediante el uso de un laser. Necesita un postprocesado de curado para la pieza.
#### DLP (Fotopolimerización)
Se basa en proyectar una luz como una especia de fotografía que hará que la resina se endurezca. Menos precisa pero más rápida que la SLA. Necesita un postprocesado de curado para la pieza. 

#### Proceso de impresión 3d
1. Primero creamos el model (CAD, Escultura digital, Ingeniería inversa).
2. Convertir el modelo CAD a STL (Archivo simplificado de la herramienta compatible con la impresora).
3. Selección de tecnología/material y programaremos:
	1. El interior de la pieza (forma cantidad de material).
	2. Los soportes para la impresión (se encarga de hacer de andamios si es necesario durante la impresión, en FDM por regla general a partir de los 45º).
	3. Normas de diseño (Grosor de las paredes, inclinación de las paredes, tamaño de geometrías sin soporte, dirección de las fuerzas y las curvas y cantos).
	4. Definición (precisión dependerá de la altura de capa en el eje Z y en el eje XY dependerá del ancho de boquilla).
	5. La optimización del programa de impresión para obtener el máximo rendimiento imprimiendo las 24h.
	6. Aveces sera conveniente dividir las piezas en partes mas pequeñas por distintas razones, pudiendo unirse después mediante enlaces químicos y enlaces mecánicos. 
4. Impresión.
5. Objeto final y postprocesado.
	