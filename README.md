# Ejecutar progamas al inicio de linux

El primer paso es crear un script que se encargue de arrancar nuestro software de manera automática. En nuestro caso era el script detector-init (para poner en marcha automáticamente un sensor de presencia). Para crearlo hacemos:

## Mover detector-init en 
```ssh
    /etc/init.d/
```
Cambiamos permisos de archivo:
```ssh
    sudo chmod 755 /etc/init.d/detector-init
```
Comprobamos que todo se ejecuta correctamente:
```ssh
    sudo /etc/init.d/detector-init start
```
Agregamos a ejecucion de inicio:
```ssh
    sudo update-rc.d detector-init defaults
```


