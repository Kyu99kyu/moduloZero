# Laboratorio Git

<p>En este laboratorio creare un repositorio de git para demostrar mis conocimientos adquiridos en el Modulo 0.</p>

## Crear un repositorio en local

- Abre tu terminal y navega hasta el directorio donde deseas crear el repositorio.
- Crea una carpeta con el nombre del repositorio.
- Ingresa a la carpeta que acabas de crear.
- Inicializa el repositorio de Git.

```
git init
```

<img src="./img/parte1.png">

## Subir el repositorio a GitHub

- Crea un nuevo repositorio en GitHub.
- Copia el URL del repositorio que acabas de crear en GitHub
- Conecta tu repositorio local con el repositorio en GitHub.
- Verifica que la conexión se haya establecido correctamente.

<p> Previamente configuramos la clave ssh </p>

```
git remote add origin git@github.com:Kyu99kyu/moduloZero.git
```

<img src="./img/parte2.png">
<img src="./img/parte2v2.png">

## Hacer un commit y un push

- Crea un archivo en la carpeta del repositorio.
- Añade el archivo al staging.
- Crea un commit con un mensaje descriptivo.
- Sube los cambios al repositorio en GitHub.

```
git add .
git commit -m "primer commit"
git push -u origin master
```

<img src="./img/parte3.png">

<img src="./img/parte3v2.png">

## Crear una rama

- Crea una rama nueva llamada "development".
- Cambia a la nueva rama.
- Realiza algunos cambios en el archivo que creaste.
- Añade y haz un commit con los cambios en la rama "development".
- Sube los cambios a Github

```
git checkout -b development
```

<img src="./img/parte4.png">

<img src="./img/parte4v2.png">

## Hacer un merge

- Vuelve a la rama "main".
- Haz un merge de la rama "development" a la rama "main".
- Si no hay conflictos, los cambios realizados en la rama "development" se incorporarán a la rama "main".
- Hax un push de los cambios al repositorio en GitHub.

```
git checkout master
git merge development
```

<img src="./img/parte5.png">
<img src="./img/parte5v1.png">
<img src="./img/parte5v2.png">
