

## Instalar git

Instala github en Ubuntu con el siguiente comando:

```shell
$ sudo apt-get install git-all
$ sudo apt-get install retext
```

Retext nos va a servir par poder editar archivos en lenguaje Markdown (como este mismo), puedes utilizar cualquier otro editor, incluso un editor de texto plano.

## Configurar git

Usa tu nombre de usuario de GitHub para configurar la autoría de tus cambios:

```shell
$ git config --global user.name "TU_NOMBRE"
```

Define una dirección de correo electrónico:

```shell
$ git config --global user.email "TU_CORREO_ELECTRONICO"
```


## Crear o clonar repositorios

Para clonar y descargarse un repositorio en github:

```shell
$ git clone https://github.com/xabier/github-minihowto
```

Si vas a crear un repositorio nuevo en github. Primero lo creas con un nombre específico en GitHub y luego, o bien lo clonas como antes o te creas uno en local

```shell
$ git init NOMBRE_PROYECTO
```


## Editar archivos y realizar cambios

Vas a la carpeta que tienes en local y editas un documento cualquier, por ejemplo el `README.md` con tu editor favorito

```shell
$ retext howto.es.md
```

Realizas cambios (por ejemplo puedes añadir tu nombre al final del archivo), los guardas con el editor y luego avisas a git de que ha realizado cambios en ese archivo:

```shell
$ git add README.md
```

Si has modificado varios documentos puedes añadir todos a la vez con:

```shell
$ git add *
```

Con esto lo que hemos conseguido es añadir los cambios al Index o Staging, que es, como el nombre indica, el índice de los archivos modificados, pero aún no hemos "guardado" esos cambios. Para eso tenemos que realizar un commit:

```shell
$ git commit -m "Mensaje de cambios"
```

El "Mensaje de cambios" es el mensaje con el que se guardarán dichos cambios explicando a terceros cual es, en resumen, la aportación o modificaciones que has realizado.


## Actualizar cambios en el servidor remoto

Para actualizar directamente a master hacemos:

```shell
git push origin master
```

Si en lugar de actualizar los cambios directamente en master queremos crear una rama, actualizar y sólo posteriormente fusionar o actualizar los cambios en la rama maestra (master), entonces, primero tenemos que crear una rama:

```shell
$ git checkout -b NOMBRE_RAMA
```

Y para subir (empujar, push) la rama al repositorio remoto hacemos:

```
$ git push origin NOMBRE_RAMA
```

Ahora si quieres fusionar tu rama con la maestra

```shell
$ git merge NOMBRE_RAMA
```


Para no acumular ramas es recomendable borrarlas una vez esten completadas:

```shell
$ git branch -d NOMBRE_RAMA
```


## Actualizar tus repositorios locales

Si hay cambios en los servidores remotos y tienes que actualizar tu repositorio local




```
```
```
```



git add  Identidad-censo-privacidad-poder.md 
git commit -m "nueva versión (o lo que sea)" 
git push origin master

# Personas que están aprendido con este tutorial

* Xabier

# References

* Markdown 
	* https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
* Git and Github
	* https://services.github.com/on-demand/downloads/github-git-cheat-sheet/
	* https://rogerdudler.github.io/git-guide/
