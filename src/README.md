# Release v1.0 - ExamenCOD

Este documento describe los pasos detallados para realizar la **release v1.0** del proyecto **ExamenCOD**.

## Pasos para crear la release

### 1. Realiza un fork del proyecto

Antes de empezar a trabajar en el proyecto, debes hacer un **fork** del repositorio original para que puedas trabajar de manera independiente.

1. Ve al repositorio [ExamenCOD](https://github.com/damiancastelao/ExamenCOD).
2. Haz clic en el botón **"Fork"** en la esquina superior derecha de la página.
3. Esto creará una copia del repositorio en tu cuenta personal de GitHub.

#### Justificación:
El **fork** es necesario para tener una copia del repositorio donde podrás hacer cambios sin afectar al proyecto original.

---

### 2. Clona el repositorio a tu máquina local

Una vez que hayas hecho el **fork**, debes clonar el repositorio a tu máquina local para trabajar en él.

1. Copia la URL del repositorio de tu cuenta de GitHub.
2. Abre tu terminal y ejecuta los siguientes comandos:

   ```bash
   git clone https://github.com/TU_USUARIO/ExamenCOD.git
   cd ExamenCOD

## 3. Revisa las ramas existentes 
git branch -a

## Crear y trabajar en la rama readme
git checkout -b readme

## Crea un archivo llamado README.md en la raíz del proyecto y agrega el contenido que estás leyendo ahora.
git add README.md
git commit -m "Agregado README con pasos para la release v1.0"

## Luego de agregar el contenido, agrega y confirma los cambios:
git push origin readme

## Verifica el código de la rama interface
git checkout interface

## Revisa el historial de commits con el siguiente comando:
git log

## Si el último commit no es necesario o contiene código que no debe ser incluido, puedes revertirlo utilizando el commit-id:
git revert <commit-id>

## Fusiona las ramas en main
git checkout main
git merge datos
git merge interface

## Después de la fusión, confirma los cambios y empuja a main
git push origin main

## Etiqueta el commit como v1.0
git tag -a v1.0 -m "Release v1.0"
git push origin v1.0

## Crear la release en GitHub. 
Ahora que tienes la etiqueta v1.0, puedes crear la release en GitHub.
Ve a la página de tu repositorio en GitHub.
Haz clic en la pestaña "Releases". Si no la ves, puedes acceder a la URL directamente: https://github.com/TU_USUARIO/ExamenCOD/releases.
Haz clic en "Draft a new release".
En el campo "Tag version", selecciona la etiqueta v1.0.
Agrega un título para la release, como "Release v1.0".
Agrega una descripción sobre los cambios realizados en esta release.
Haz clic en "Publish release" para publicar la release. 
