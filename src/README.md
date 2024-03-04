Primero realizamos un fork del repositorio

Para ello clickamos en FORK y renombramos, y desclickamos la pestaña de solo hacer fork a la main

Nos colocamos en la carpeta local donde queremos colocar los archivos, y realizamos el clonado con git clone y la url

Con el repositorio ya clonado, hacemos la rama readme, con el comando: git branch readme

Nos colocamos en ella con git checkout readme

Hacemos un checkout datos para colocarnos en la rama datos y realizar varias modificaciones y commits

Hacemos chekout a la rama interface

Y repetimos el paso anterior, hacemos dos modificaciones y commits de ellas

Repetimos el paso, checkout a la rama readme y hacemos un commit de lo que hemos ido añadiendo

Nos situamos en interfaz con checkout

Hay que borrar el último commit "I2" para ello nos situamos en el commit anterior a él "I1" y le damos al boton derecho->reset current branch to here->hard

Le damos a hard porque también queremos que borre el código de ese commit

Realizamos la fusión:
    
    nos colocamos en la main con checkout
    
    git ->merge ->datos y marcamos --squash

    git ->merge -> interface y marcamos --squash

Hacemos un commit "v1.0" para etiquetar la fusión

Para añadir el .gitignore en el último commit, primero nos colocamos en el .idea(que es lo que vamos a añadir al .gitignore) git->add to .gitignore

Luego comando: git commit --amend

Nos saldrá una pantalla de opciones donde tendremos que escribir el comentario: añadido gitignore y salimos de la pantalla

Ya estaría añadido el gitignore al último commit "v1.0"

