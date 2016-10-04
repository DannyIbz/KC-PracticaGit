##Respuestas a las preguntas de la práctica de Git


**Paso 11**
Usamos el comando *git reset --hard HEAD~1*. Porque usando el comando *reset HEAD~1* volvemos al commit anterior
y añadiendo el modificador *--hard* perdemos cualquier trabajo que quede pendiente de comitear en el *working
copy*.

**Paso 12**
Usamos *git reflog* y luego *git reset --hard <hash>*. Usando el comando *reflog* listamos todos los commits
por donde hemos pasado. Ahí podemos localizar el identificador (hash) del commit al cual queremos volver y con
el comando *reset --hard <hash>* le indicamos a Git que queremos volver a dicho commit recuperando todo el 
trabajo "perdido".

**Paso 13**
No. Porque desde la rama *styled* y su último commit se pueden acceder directamente al resto de los commits, y
al realizar un *merge* no queda ningún commit sin acceso.

**Paso 19**
Si. Porque al hacer *merge* el commit de la rama *htmlify* quedaría sin acceso.

**Paso 21**
No. Porque desde el commit de la rama *styled* se puede acceder a la rama *master* sin dejar ningún commit
inaccesible.

**Paso 25**
*git log --graph*. En mi caso uso el alias *git graph* que usamos durante el curso.

**Paso 26**
No. Porque el commit de la rama *title* quedaría entonces sin acceso.

**Paso 27**
*git reset HEAD~1* para no perder los cambios en el *working copy*.

**Paso 28**
*git checkout -- git-nuestro.md* para descartar los cambios que hayan en el *working copy*.

**Paso 29**
*git branch -D title*. Hacemos uso del modificador *-D* porque si lo hiciesemos con la *d* minúscula no nos 
dejaría debido a que la rama no ha sido *mergeada*.

**Paso 30**
*git reflog* y *git reset --hard <hash>*. Al igual que hicimos en el paso 12, hacemos uso del modificador 
*--hard* para recuperar todo el trabajo descartado con anterioridad.

**Paso 32**
*git log* para mostrar todos los commits a los que se tiene acceso y copiar el *hash del commit inicial. Usamos
*git reset --hard <hash> para movernos a ese commit con todo su contenido.

**Paso 33**
En este caso, usamos el comando *git reflog* para mostrar todos los commits por donde hemos pasado, ya que si 
usasemos el *git log* solo nos mostraría el commit donde nos encontramos y con *reflog* tenemos una vista 
global. Copiamos el *hash* del comit final y nos movemos a él con *git reset --hard <hash>*.


**Daniel Sánchez**
