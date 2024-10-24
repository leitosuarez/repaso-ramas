# Clase 06 bootcamp

Si yo ahora creo un repositorio de git, en este se va a guardar y hacer referencia al contenido de la carpeta 01-repaso-git-ramas, no en la carpeta CLASE-06

Para sacar un archivo de la zona verde, osea de la staging area (SA), que seria revertir el "git add" (porque me arrepenti o por lo que sea) que hice tengo que usar el comando:

``` sh
git rm --cached <file>
```

Esto va a hacer que vuelva al working directory

Cuando creamos o terminamos una funcionalidad, o una microtarea de una proyecto, es ahi donde deberiamos agregar el commit (un posible commit)con

```sh
git commit 
```

asi pelado, abrimos la consola nano en con lo cual podemos escribir una descripcion mucho mas extensa de lo que hicimos en el commit. El formato seria: poner el titulo y luego a partir de la tercera linea un mensaje mas descriptivo y extenso osea la explicacion

# Cambiar el editor por nano

```sh
git config --global core.editor nano #(editor de la consola, el mejor)
```

```sh
git config --global core.editor "code --wait" #(editor del vsco)
```

# Ver listado de commits que hice en el repo 

```sh
git log #version corta (aparecen mas detallados)
git log --oneline #version larga
```

Usar o agregar el README.md a la hora de crear un repositorio de github, es practicamente obligatorio 

# Agregar un remoto a mi repositorio local

```sh
git remote add origin <url-al-repo-remoto> #(siempre con el https)
```

# Git remote-agregar/eliminar repo
La forma de visualizar si tengo un repositorio agregado o no o 
cuantos tengo es usando el comando 

```sh
git remote -v
```

Si quiero eliminar un repo que tengo agregado por y o x, tengo que usar 

```sh
git remote remove
```

Si quiero saber mas comandos con el argumento o subcomando "remote" , pongo:

```sh
git remote -help 
```
y ahi me van a saltar todos

# Crear repo y mas 
Si tengo (master) a la hora de crear el repo debo usar el comando:

```sh
 git branch -M main 
 ```
 
 y recien ahi subo al repositorio local al repositorio de github digamos, osea creo el repositorio. Usando:

```sh
git push -u origin main
```