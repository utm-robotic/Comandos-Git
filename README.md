# Comandos Git
Este documento es una guía para los comandos de Git, abarca desde los comandos de uso diario hasta algunos que son un poco más avanzados para trabajar con GitHub y repositorios remotos, así como también un breve diccionario para saber algunas palabras clave que  se usan.

## Lista de comandos
**Comandos de inicialización**
* `git init`
* `git clone <url>`

**Comandos básicos**
* `git add <archivos>`
* `git commit -m <mensaje>`
## Comandos de inicialización
Existen 2 comandos para iniciar un repositorio de Git, es decir, solo se ejecutarán una vez por repositorio. El primer comando es `git init` el cual inicia un repositorio local vacío.
**Ejemplo:**
```bash
git init
```
El segundo comando para iniciar un repositorio es `git clone`, este comando descarga un repositorio remoto hacia tu máquina virtual trayendo todo su historial de versiones consigo.
**Sintaxis:**
```bash
git clone <url>
```
**Ejemplo:**
```bash
git clone git@github.com:utm-robotic/Comandos-Git.git
```
## Comandos básicos
Estos comandos son de básicos de git y son los que más estarás usando en tu día a día con tu repositorio.

* El primer comando es `git add`, este comando agrega los archivos seleccionados a la zona de preparación para la nueva versión o commit del repositorio.
**Sintaxis:**
```bash
git add <archivos>
```
**Ejemplo:**
```bash
git add archivo.txt                       # Ejemplo 1 (Agregar un solo archivo)
git add archivo.txt about.html index.php  # Ejemplo 2 (Agregar multiples archivos)
git add .                                 # Ejemplo 3 (El punto agrega todos los archivos dentro del repositorio)
```
* El segundo comando es `git commit`, el cual crea y guarda una nueva versión del repositorio desde los archivos que se fueron a la zona de preparación con el comando `git add`. Este debe tener el parámetro `-m` siempre, que significa *message* o mensaje, posterior a un mensaje descriptivo de los cambios realizados en el repositorio.
**Sintaxis:**

```bash
git commit -m <mensaje>
```
**Ejemplo:**
```bash
git commit -m "Esto fue lo que cambió..."
```
