# Shell
#linux 

---
## Introducción
### Mapa de ficheros
- **/bin**: Los binarios más basicos del sistema (ls,cd,apt)
- **/boot**: Archivos de arranque, imagen kernel
- **/etc**: Archivos de configuraciones 
- **/dev**: Donde se encuentran todos los dispositivos del sistema, en forma de fichero
- **/home**: Directorios particulares de los usuarios
- **/lib**: Librerias del sistema
- **/lost+found**: Archivos perdidos durante chequeo de disco
- **/mnt**: Punto de montaje (opcional)
- **/proc**: Sistema de ficheros que refleja el estado y configuración del sistema
- **/sbin**: Binarios de configuración utilizados por el Kernel
- **/usr**: Binarios de servidores, programas, manuales…
- **/opt**: Binarios opcionales
- **/root**: Home del superusuario (root)
- **/tpm**: Directorio temporal
- **/var**: Almacenaje de variables
### Ver versión y distro
```bash
neofetch
```
### Ver bateria
```bash
acpi -i
```
### Ayuda
```bash
comando -h
comando -help
comando -?
```
### Manual
```bash
man comando
```
### Busqueda comandos (apropos)
```bash
apropos palabra_comando
```
### Cambiar fondo
```bash
feh --bg-scale image.jpg
```
## Comandos
#### Cambiar directorio (change directory)
```bash
cd ruta_directorio
```
#### Ruta actual (pwd)
```bash
pwd
```
#### Listar contenido (ls)
```bash
ls
```
Podemos especificar directorio a listar como:
```bash
ls ruta_directorio
```
En algunas personalizaciónes vemos todos los permisos si queremos ver solo los archivos de manera mas simple haremos:
```bash
lsd
```
Algunas opciones utilizadas son:
```bash
-a #all
-l #long list format
-al
```
#### Copy (cp)
Para copiar un acrhivo a otro lugar
```bash
cp [options] archivo destino
```
Para copiar el archivo en el mismo sitio con otro nombre:
```bash
cp [options] archivo nombre_copia
```
#### remove (rm)
Eliminar archivo:
```bash
rm  [options] nombre_archivo
```
Eliminar directorio con cosas:
```bash
rm -r directorio
```
#### make directory (mkdir)
```bash
mkdir nombre
```
#### remove directory (rmdir)
```bash
rmdir directorio
```
#### mover y renombrar (mv)
Mover directorio:
```bash
mv directorio/archivo destino
```
Renombrar directorio:
```bash
mv archivo nombre_nuevo
```
#### Editar fichero (vim nano nvim)
```bash
nano archivo
```
```bash
vim archivo
```
```bash
nvim
```
#### Limpiar consola (clear)
```bash
clear
```
#### Salir de la consola (exit)
```bash
exit
```
#### Filtar (grep)
```bash
grep
```
#### Listar interior de archivo (cat)
```bash
cat
```
#### Editar permisos (chmof)
```bash
chmod 700/+r-- archivo
```
#### Change owner (chown)
```bash
chown
```
#### tar
```bash
tar  [options]
```
#### gunzip
```
gunzip fichero
```
#### gestor de paquetes debian
```bash
dpkg
```
#### Alias
```bash
alias 
```
#### montar y desmontar unidades extraibles (mount unmount)
Montar:
```bash
mount /dev/disc_sdc_sdb /mnt_media
```
Desmontar:
```bash
umount /dev/disc_sdc_sdb
```
#### Ordenar contenido (short)
```bash
short
```
#### Crear accesos directos
```bash
ln
```
#### Cabeza y rabo (head tail)
```bash
tail #Muestra las ultimas 10 lineas
```
```bash
head #Muestra las primeras 10 lineas
```
#### Tipo de archivo (file)
```bash 
file fichero
```
#### Comparar ficheros (cmp)
```bash
cmp fichero1 fichero2 #Nos reporta si son distintos
```
#### Diferencia archivos (diff)
```bash
diff fichero1 fichero2 #Nos devuelve la diferencia entre los dos archivos
```
#### Contar palabras (wc)
```bash
wc ficher
```
#### Añadir usuario (adduser)
```bash
adduser nombre
```
#### Borrar usuario (deluser)
```bash
deluser nombre
```
#### Modificar usuario (usermod)
```bash
usermod
```
#### Ver espacio disponible (df)
```bash
df
```
#### Información conexiones activas (netstat)
```bash
netstat
```
#### Informacion de procesos activos (ps)
```bash 
ps
```
#### Matar proceso (kill)
```bash
kill -9 proceso
```
#### Estado ram y swap (free)
```bash
free
```
#### Uso de disco(du)
```bash
du
```
#### Gestión  de discos (fdisk)
```bash 
fdisk /dev/disco
```
> [!danger] Formateo
> Primero eliminamos particiones 
> Creamos tabla de contenidos
#### Formatear disco (mkfs)
```bash
sudo mkfs.fat32:ntfs:ext4 /dev/partición
```
### Comandos comunicación 
#### Conectar a puertos TCP (telnet)
```bash
telnet host port
```
#### Comprobar si se aceptan mensajes (mesg)
```bash
mesg -y
```
#### Mandar mensaje a usuario (write)
```bash
write usuario mensaje
```
#### Mandar mensaje a usuarios conectados (wall)
```bash
wall "A mamarla parla"
```
