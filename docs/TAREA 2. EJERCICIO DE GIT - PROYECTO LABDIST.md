[TOC]

# TAREA 2. EJERCICIO DE GIT - PROYECTO LABDIST

## TRABAJO EN LOCAL

1- Inicializa un nuevo repositorio Git en una carpeta llamada "labdist" y agrega los
archivos proporcionados en el aula virtual. Renombra la rama master a main , si es
necesario. Realiza el primer commit. Muestra el log del repositorio.

``````
mkdir labdist -> Para crear el fichero labdist
cd labdist -> Colocarnos en el fichero creado
git init -> Para crear el repositorio del fichero
git branch -m main -> Renombrar la rama master por main
git add . -> para agregar los archivos al staging area
git status -> mostrar el estado actual del repositorio
git commit -m "mensaje" -> realizar el commit aplicandole un mensaje
``````



<img src="D:/USER/Pictures/Screenshots/Captura%20de%20pantalla%202025-01-30%20124528.png" alt="Captura de pantalla 2025-01-30 124528" style="zoom:80%;" />

<img src="D:/USER/Pictures/Screenshots/Captura%20de%20pantalla%202025-01-30%20125809.png" alt="Captura de pantalla 2025-01-30 125809" style="zoom:80%;" />

<img src="D:/USER/Pictures/Screenshots/Captura%20de%20pantalla%202025-01-30%20130012.png" alt="Captura de pantalla 2025-01-30 130012" style="zoom:80%;" />

<img src="D:/USER/Pictures/Screenshots/Captura%20de%20pantalla%202025-01-30%20173625.png" alt="Captura de pantalla 2025-01-30 173625"  />

2-Incluye un fichero .gitignore para que los ficheros README.md , LICENCE.txt y
passwords.txt sean ignorados por el control de versiones. Realiza el commit y muestra
los logs del repositorio en una línea.

``````
git log --oneline -> mostrar los logs del repositorio en una linea
``````



<img src="D:/USER/Pictures/Screenshots/Captura%20de%20pantalla%202025-01-30%20174010.png" alt="Captura de pantalla 2025-01-30 174010" style="zoom: 50%;" />

![Captura de pantalla 2025-01-30 174818](D:/USER/Pictures/Screenshots/Captura%20de%20pantalla%202025-01-30%20174818.png)

3-En el repositorio, crea los archivos README.md , LICENCE.txt y passwords.txt con
algún contenido. Muestra el estado del repositorio. Muestra el listado de archivos
ignorados.

``````
echo "mensaje > README.md" -> escribir mensaje en README.md
echo "mensaje" LICENCE.txt -> Dar contenido a LICENCE.txt
echo "mensaje" passwords.txt -> escribir contenido en passwords.txt
git status -> ver el estado del repositorio
git status --ignored -> ver archivos ignorados
``````



![Captura de pantalla 2025-01-30 175712](D:/USER/Pictures/Screenshots/Captura%20de%20pantalla%202025-01-30%20175712.png)

![Captura de pantalla 2025-01-30 180237](D:/USER/Pictures/Screenshots/Captura%20de%20pantalla%202025-01-30%20180237.png)

4-Crea una rama feature-estilos . Cámbiate a ella.
Modifica el archivo estilos.css :
propiedad color del body y de h2 : #2a2a2a
propiedad background-color de header y footer: #2a75ff
Comprueba el estado del repositorio. Añade los cambios, realiza un commit con el
mensaje "actualizados estilos a azules"

``````
git checkout -b feature-estilos --> Crea la rama feature-estilos y cambia a esa rama
git status -> comprobar el estado del repositorio
git add css/estilos.css -> añadir a staging area los cambios
git commit -m -> confirmar los cambios con un commit, escribiendo un mensaje que los defina
``````



![Captura de pantalla 2025-01-30 130240](D:/USER/Pictures/Screenshots/Captura%20de%20pantalla%202025-01-30%20130240.png)

![Captura de pantalla 2025-01-30 182135](D:/USER/Pictures/Screenshots/Captura%20de%20pantalla%202025-01-30%20182135.png)

![Captura de pantalla 2025-01-30 182252](D:/USER/Pictures/Screenshots/Captura%20de%20pantalla%202025-01-30%20182252.png)

![Captura de pantalla 2025-01-30 182655](D:/USER/Pictures/Screenshots/Captura%20de%20pantalla%202025-01-30%20182655.png)

5-Vuelve a la rama main . En el archivo index.html añade un comentario donde se indique
tu nombre como autor de la página. Comprueba el estado del repositorio. Añade los
cambios, realiza un commit con el mensaje ' añadido autor en index'. Muestra los logs del
repositorio en una línea, gráficamente y con 'decoración'

``````
git checkout main -> volver a la rama main
nano index.html -> para modificar el archivo de texto index.html
git add index.html -> enviar cambios al staging area
git commit -m -> hacer el commit dejando mensaje de definicion del cambio
git log --oneline --graph --decorate --all -> mostrar los log del repositorio en una sola linea, con gráficos, decoracion y todos
``````



![Captura de pantalla 2025-01-30 184038](D:/USER/Pictures/Screenshots/Captura%20de%20pantalla%202025-01-30%20184038.png)

![Captura de pantalla 2025-01-30 184151](D:/USER/Pictures/Screenshots/Captura%20de%20pantalla%202025-01-30%20184151.png)

6-Fusiona la rama feature-estilos en la rama main . Muestra los logs del repositorio en
una línea, gráficamente y con 'decoración'

``````
git merge feature-estilos -> desde la rama main indico que fusione feature-estilos a la tama en la que estoy que es la main
git log --oneline --graphs --decorate --all -> mostrar los log segun caracteristicas indicadas
``````



![Captura de pantalla 2025-01-30 184901](D:/USER/Pictures/Screenshots/Captura%20de%20pantalla%202025-01-30%20184901.png)

## TRABAJO EN REMOTO

1-Continúa con el repositorio labdist . Añade el repositorio a Sourcetree.

![Captura de pantalla 2025-01-30 194013](D:/USER/Pictures/Screenshots/Captura%20de%20pantalla%202025-01-30%20194013.png)

![Captura de pantalla 2025-01-30 194036](D:/USER/Pictures/Screenshots/Captura%20de%20pantalla%202025-01-30%20194036.png)

2-En tu cuenta de GitHub, crea un repositorio remoto y sube al remoto los ficheros de tu
repositorio local. Debes subir todas las ramas. Muestra, además, la captura de pantalla
donde se vean en GitHub, algo similar a esto:



![Captura de pantalla 2025-01-30 195349](D:/USER/Pictures/Screenshots/Captura%20de%20pantalla%202025-01-30%20195349.png)



![Captura de pantalla 2025-01-30 202557](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-01-30%20202557.png)

![Captura de pantalla 2025-01-30 202803](D:/USER/Pictures/Screenshots/Captura%20de%20pantalla%202025-01-30%20202803.png)

![Captura de pantalla 2025-01-30 202841](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-01-30%20202841.png)

4-En el repositorio local, crea una rama feature-index . Añade el siguiente código dentro
de la <section class="about"> . Añade los cambios y crea un commit con el mensaje
"Añadido párrafo equipo en index.html". Sube los cambios al remoto. (Recuerda que
debes usar SourceTree en todo este apartado )

![Captura de pantalla 2025-01-31 185750](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-01-31%20185750.png)

![Captura de pantalla 2025-01-31 190400](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-01-31%20190400.png)

![Captura de pantalla 2025-02-01 191530](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20191530.png)

![Captura de pantalla 2025-02-01 191600](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20191600.png)

Los cambios ya están hechos en local, ahora vamos a ir a Push para subir los cambios a remoto.

![Captura de pantalla 2025-02-01 195354](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20195354.png)

![Captura de pantalla 2025-02-01 195757](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20195757.png)

Esto indica que se ha subido al remoto.

5-En el repositorio local, fusiona la rama feature-index en la rama main .

Comprobamos que estamos en la rama main, y en el Graphs que estamos parados en el punto donde queremos hacer el merge, con el boton derecho en ese punto 

![Captura de pantalla 2025-02-01 195950](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20195950.png)

Seleccionamos merge

![Captura de pantalla 2025-02-01 200134](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20200134.png)

En esta imagen se puede comprobar que el merge fue realizado con éxito.

![Captura de pantalla 2025-02-01 202449](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20202449.png)

6-Edita el fichero contacto.html . Borra unas líneas. Muestra los ficheros con cambios
pendientes y las diferencias. Añade los cambios y haz un commit.

![Captura de pantalla 2025-02-01 203645](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20203645.png)

![Captura de pantalla 2025-02-01 203834](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20203834.png)

Aquí se puede comprobar el código original,  lo que se ve en rojo es lo que se a eliminado y lo que se ve en verde lo que se ha añadido y en la imagen siguiente se puede comprobar que se ha hecho commit con los cambios.

![Captura de pantalla 2025-02-01 204411](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20204411.png)

7-Te das cuenta del error. Deshaz TOTALMENTE el commit anterior. Captura el estado
actual del repositorio. (Asegúrate de que el fichero contacto.html ha recuperado todas
las líneas borradas y no hay cambios pendientes en el repositorio.)

Lo primero accederemos al último commit anterior al que queremos eliminar , clic derecho y nos dirá reset current branch this commit, al pinchar nos pedirá si deseamos conservar los cambios o elminarlos, soft o hard, elegiremos hard.

![Captura de pantalla 2025-02-01 204631](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20204631.png)

![Captura de pantalla 2025-02-01 204718](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20204718.png)

![Captura de pantalla 2025-02-01 204913](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20204913.png)

8-Crea una rama feature-mapa y cámbiate a ella. Incluye este código en el archivo
contacto.html . Añade los cambios. Realiza un commit

![Captura de pantalla 2025-02-01 205515](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20205515.png)

Aquí se puede comprobar la nueva rama feature-mapa y el commit.

9-Sube los cambios al remoto - los de todas las ramas. Muestra en el remoto los cambios
del archivo contacto.html en la rama feature-mapa .

Rama subida al remoto en la siguiente imagen

![Captura de pantalla 2025-02-01 210059](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20210059.png)

En Github en la rama feature-mapa accedo al fichero contacto.html

![Captura de pantalla 2025-02-01 210240](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20210240.png)

Y el código modificado se puede ver

![Captura de pantalla 2025-02-01 210321](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20210321.png)

10-En GitHub, en la rama main , fusiona la rama feature-mapa . Baja los cambios del remoto
a local. Deja los dos repositorios sincronizados. Muestra una captura de pantalla donde
se vea la página principal de tu repositorio remoto

En Git pinchamos en Pull requests, previo revisar que estamos en la rama main ubicados

![Captura de pantalla 2025-02-01 210726](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20210726.png)

New pull request

![Captura de pantalla 2025-02-01 210925](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20210925.png)

Eliges la rama que deseas fusionar

![Captura de pantalla 2025-02-01 210938](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20210938.png)



Comprobamos que se va a fusionar tal cual deseamos la rama feature-mapa en main

![Captura de pantalla 2025-02-01 211116](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20211116.png)

Comprobamos los cambios sean los desados



![Captura de pantalla 2025-02-01 211133](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20211133.png)

Añadimos opcionalmente titulo y descripción

![Captura de pantalla 2025-02-01 211704](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20211704.png)

Comprobamos que no hay conflictos

![Captura de pantalla 2025-02-01 211731](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20211731.png)

![Captura de pantalla 2025-02-01 212150](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20212150.png)

![Captura de pantalla 2025-02-01 212235](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20212235.png)

![Captura de pantalla 2025-02-01 212327](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20212327.png)

![Captura de pantalla 2025-02-01 212356](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20212356.png)

Finalmente podemos comprobar que se ha realizado el merge correctamente y se han fusionado.

En sourcetree desde la rama main realizamos pull.



![Captura de pantalla 2025-02-01 214600](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20214600.png)

![Captura de pantalla 2025-02-01 214835](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-01%20214835.png)

## CONFLICTOS

1-Crea una rama hotfix-js . Cámbiate a ella. Añade este código en el fichero script.js .
Confirma el cambio y haz un commit con el mensaje "corregido problema en script.js".
(Fíjate en los números de línea de tu editor ...)

![Captura de pantalla 2025-02-02 112543](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-02%20112543.png)

2-Vuelve a la rama main . En el fichero script.js en las mismas líneas que en la cuestión
anterior, añade el código siguiente. Confirma el cambio y haz un commit con el mensaje
"corregido problema en script.js rama main".

![Captura de pantalla 2025-02-02 112925](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-02%20112925.png)

3-Fusiona la rama hotfix-js en main . Debe producirse un conflicto. Resuélvelo como
consideres oportuno. Cuando termines la resolución del conflicto sube los cambios al
remoto.

Nos colocamos en la rama main haciendo checkout y hacemos click derecho sobre la rama a fusionar, ya me indica una ventana emergente que hay conflictos asi que sobre el archivo que tiene le conflicto hacemos click derecho y aparecera esta imagen



![Captura de pantalla 2025-02-02 114852](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-02%20114852.png)

Nos dara la opción de Resolve using "Mine", "Theirs ", Restart Merge.. . en mi caso elegí quedarme con mis cambios que como estoy ubicado en la rama main, son los cambios que se realizaron desde main.

![Captura de pantalla 2025-02-02 115430](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-02%20115430.png)

![Captura de pantalla 2025-02-02 115457](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-02%20115457.png)

![Captura de pantalla 2025-02-02 115741](./TAREA%202.%20EJERCICIO%20DE%20GIT%20-%20PROYECTO%20LABDIST.assets/Captura%20de%20pantalla%202025-02-02%20115741.png)

En estas 3 últimas imágenes se puede comprobar como no existe ninguna notificación sobre el conflicto, ni en Sourcetree, ni en Visual-Estudio ni en GitHub. 
