# Curso Git desde cero
Sistema de control de versiones para el mantenimiento eficiente y confiable de archivos.

## Zonas de Git
1. Directorio de trabajo
2. Area de Preparacion
3. Directorio Git

## Flujo de trabajo basico en Git
1. Modificas una serie de archivos en tu directorio de trabajo.
2. Preparas los archivos, añadiendolos a tu area de preparacion.
3. Confirmas los cambios, lo que toma los archivos tal y como estan en el area de preparacion y almacena esa copia instantanea de manera permanente en tu directorio de Git.

## Configurando Git por primera vez
```
git config --global user.name "Hernan De La Cruz"
git config --global user.email jh@gmail.com
git config --global core.editor nano
git config --list
```


## Configuracion SSH en Windows
1. Ejecutamos el comando ´ssh-keygen´ en el disco ´C´ para evitar problemas de ruta.
2. Ejecutamos el comando ´ssh-keygen -t rsa -C "mi-correo@ejemplo.com"´.
El correo debe ser el mismo con el que nos regustramos en Github para evitar posibles problemas.
Dejamos el passhrase vacio y damos enter.
3.Iniciamos ssh-agent en background ejecutando el comando ´eval "$(ssh-agent -s)"´.
4.Agregamos la llave ssh generada a ssh-agent ejecutando el comando ´ssh-add /c/llaves-ssh/github_rsa´.
5. Desde ahora podemos hacer pull y push sin que Github nos este pidiendo los datos de acceso.