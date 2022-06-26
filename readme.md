# Respuestas Practica Git

- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
- El comando utilizado ha sido git reset --hard HEAD~1, porque necesitaba volver al paso anterior y 
perder el trabajo del working copy

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
- El comando utilizado ha sido primero git reflog para comprobar el id del commit que quiero rehacer y 
despues git reset --hard y el id del commit

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
- Primero tengo que moverme de la rama styled a la rama main con git checkout main  y despues absorber la 
rama styled en main con git merge styled, y 
el conflicto ha sido que al tener dos copias diferentes en cada rama de git-nuestro.md, deberemos usar el 
comando git status y leer la informacion para entender el problema. La solucion es abrir dicho archivo 
con nano, ver que cambios queremos mantener de manera manual, en nuestro caso mantenemos ambos y despues 
git add y git commit para completar el merge 

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
- Primero tengo que moverme de la rama htmlify a la rama styled con git checkout styled  y despues 
absorber la rama htmlify en la rama styled con git merge htmlify, y
el conflicto ha sido que al tener dos copias diferentes en cada rama de git-nuestro.md, deberemos usar el
comando git status y leer la informacion para entender el problema. La solucion es abrir dicho archivo
con nano, ver que cambios queremos mantener de manera manual,en este caso nos quedamos con el contenido 
de la rama styled  y despues git add y git commit para
completar el merge

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
- Primero nos movemos a la rama main con git checkout main y despues el comando git merge styled. No ha 
causado conflicto ya que que en el paso 13 resolvimos dicho conflicto

- ¿Qué comando o comandos utilizaste en el paso 25?

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
- No podria ser fast forward porque el commit tiene que heredar de dos padres y la rama title no 
pertenece a main, por lo que quedaria un commit fuera del flujo de nuestro grafo de la rama main

- ¿Qué comando o comandos utilizaste en el paso 27?
- El comando utilizado es git reset HEAD~1, sin hacer utilzar el comando --hard para mantener los cambios 
en el working copy

- ¿Qué comando o comandos utilizaste en el paso 28?
- El comando utilizado es git restore git-nuestro.md aunque previamente deberemos de comprobar que 
archivos hay que descartar con git status

- ¿Qué comando o comandos utilizaste en el paso 29?
- El comando utilizado ha sido git branch - D title, debemos utilizar la D ya que title es una rama que 
no esta totlamente mergeada por lo que al intentar usar d nos da error

- ¿Qué comando o comandos utilizaste en el paso 30?
- Los comandos utilizados han sido, primero git reflog para buscar el id del commit que habiamos desecho 
de merge no fast forward y despues utilizamos git reset --hard y el id del commit para volver a tener 
todo nuestro trabajo en dicho commit.

- ¿Qué comando o comandos usaste en el paso 32?
- Con git log buscamos el id de ese primer commit y despues con git checkout mas el id anterior, 
apuntamos el HEAD hacia ese primer commit

- ¿Qué comando o comandos usaste en el punto 33?
- Como hemos vuelto en el punto anterior al commit inicial, con git log no veremos nada por lo que 
tenemos que utilizar git reflog que nos muestra todos los commits y buscar el commit de cambio de titulo 
del poema, e igual que en el punto anterior, con git checkout mas el id de dicho commit podremos 
desplazarnos hasta ese commit.


**Roberto Rojo**
