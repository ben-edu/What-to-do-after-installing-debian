# What-to-do-after-installing-debian

## Drivers Dell

### Wifi

```
sudo nano /etc/apt/sources.list 
 deb http://httpredir.debian.org/debian/ stretch main contrib non-free  
 sudo apt-get update && apt-get install firmware-iwlwifi  
 sudo modprobe -r iwlwifi 
 sudo modprobe iwlwifi
 ```

## Software

### Git

``` sudo apt-get install git```

### Enpass 

``` 
sudo echo "deb https://apt.enpass.io/ stable main" > \   /etc/apt/sources.list.d/ enpass.list 
sudo wget -O - https://apt.enpass.io/keys/enpass-linux.key | apt-key add -
sudo apt-get update
sudo apt-get install enpass
``` 
## Otros

### Crear iconos 

```
sudo nano /usr/share/applications/Ejemplo.desktop

[Desktop Entry]
#Nombre de la aplicación
Name=Thunderbird
#Comentario que aparece al seleccionar el lanzador
Comment=Gestor de Correo
#Comando a ejecutar, generalmente el nombre de la aplicación
Exec=/opt/thunderbird/thunderbird
#Icono del lanzador, puede ser generico o especificar la ruta del mismo
Icon=/opt/thunderbird/chrome/icons/default/default256.png
#Para no abrir una terminal
Terminal=false
#Tipo de archivo
Type=Application
#Codificación del texto
Encoding=UTF-8
#Categoria de la aplicación
Categories=Application;Network;MailClient;Email;News;GTK;
```


