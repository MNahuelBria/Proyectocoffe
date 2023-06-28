# Clase 06 - Git Intro

## Configuración inicial.

```sh
git config --global user.name "Nahuel Bria"
git config --global user.email "nagu.b.2012@gmail.com"
``` 

## Verificando la configuración inicial, si quedo todo piola!

```sh
git config --get-regexp user
```

## Inicializando un repositorio de GIT (Creando de GIT)


```sh
git init
```

## Areas del respositorio de GIT

3 Áreas

* Working Directory (WD): Directorio de trabajo donde se an agregando o quitando los archivos durante el desarrollo.
* Staging Area (SA): Área de control de cambios. Área temporal/intermedia
* Local Repo (LR): Una caja donde voy a ir guardando la fotos que vaya sacando.

## Estadoo de los archivos

* untracked: Archivos que está en el WD pero GIT no les está dando seguimiento
* unmodified: Archivo que GIT ya está siguiendo y con respecto al WD, no fueron modificos)
* modified: Archivos que sencuentra en el respositorio (Están siendo seguido por GIT) pero difieren con lo que se encuentra en el area de trabajo WD
* stateg: Archivos que están en el área temporal/intermedia

![git-areas](https://miro.medium.com/v2/resize:fit:500/0*HeEKExh4Z0nlev1m.png)

## ¿Cómo chequeo en que área están los archivo?

```sh
git status
```

## Para confirmar los cambios de un archivo (WD => SA)

```sh
git add <nombre-archivo>
git add README.md
git add README.md css/estilos.css
git add . # Con el punto (.) o el asterisco (*) Agrego todos los archivos que están (UnTRACKED, MODIFIED) al área intermedia o stanging area (SA)
```

## Para hacer commit [sacar foto] (SA => LR)

```sh
git commit -m "<Mensaje explicando que guarde en esa foto>"
git commit -m "Agrego el README.md"
``` 

## Para ver las fotos (commits) que están dentro del repositorio local (Local REPO)

```sh
git log
git log --oneline
```

## Si quiero ver los cambios entre el WD y LR
NOTA: Si se me bloquea la consola. Tengo que presionar la tecla q (quit)

```sh
git diff
```