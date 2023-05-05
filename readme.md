#Clase 15

## Configuracion inicial

```sh
git config --global user.name "Andres Teselman"
git config --global user.email "ateselman@gmail.com"
```
Se verifica con $
git config --get-regexp user

## Crear un repositorio (inicializar un repo)
```sh
git init
```
## Areas del repositorio de GIT

3 areas

Working directory (WD) -- es la carpeta donde tego mi index, css, etc donde estan los archivos durante el desarrollo--
Staging Area (SA) -- Area de control de cambios. Area temporal donde se saca "fotos". Area intermedia--
Local Repo (LR) -- caja donde voy a ir teniendo todas las fotos que vaya sacando--


## El estado de los archivos

* untracked: Git los reconoce pero no le esta dando seguimiento.
* unmodified: Son archivos que Git ya esta siguiendo y con respecto al working directory no fueron modificados.
* modified: son archivos que se encuentran en el repo (estan siendo seguidos por Git), pero difieren con lo que se encuentra actualmente en el working Directory.
* staged: Archivos con estan en el Area temporal/intermedia

## Saber estado actual de los archivos
```sh
git status
```
## Como indicar que un archivo pueda ser commiteado (llevarlo a Staging Area)

git add index.html (git add + el nombre del archivo)
git add readme.md CSS/Estilos.css
git add . (agrega todos los archivos que estan untracked, modified)

## Para sacar una foto (commitear)
 git commit -m "Agrego index.html" (el mensaje "" es una desc concisa de lo que mande a sacar foto)

## Ver las fotos que ya guarde/Commitee
```sh
git log
o
git log --oneline
```
