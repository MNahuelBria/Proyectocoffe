# Clase 06 - Git Intro

## Configuración inicial.

```sh
git config --global user.name "Maximiliano Principe"
git config --global user.email "mlapeducacionit@gmail.com"
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