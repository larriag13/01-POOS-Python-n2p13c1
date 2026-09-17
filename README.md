# 01-POOS-Python-n2p13c1
## Luis Arriagada

A continuación se detalla el flujo de comandos para configurar y actualizar el repositorio del proyecto:

### 1. Clonar el repositorio
```bash
git clone url .
```
**Explicación:** Descarga una copia exacta del repositorio remoto especificado en la `url`. El punto (`.`) al final es muy importante: le indica a Git que los archivos deben descargarse directamente en la carpeta actual, en lugar de crear una nueva subcarpeta con el nombre del repositorio.

### 2. Configurar credenciales de usuario
```bash
git config --global user.name "nombre_usuario_github"
git config --global user.email "correo_github"
```
**Explicación:** Establece el nombre y el correo electrónico que quedarán registrados como autor en el historial de cambios. El parámetro `--global` hace que esta configuración se aplique a todos los proyectos de Git en el equipo. (Nota: Es recomendable que el correo coincida con el utilizado en la cuenta de GitHub).

### 3. Preparar los cambios (Staging)
```bash
git add .
```
**Explicación:** Añade todos los archivos nuevos, modificados o eliminados en el directorio actual al área de preparación (*staging area*). Es el paso previo a confirmar los cambios, indicándole a Git exactamente qué archivos formarán parte de la próxima actualización.

### 4. Registrar los cambios (Commit)
```bash
git commit -m "avance clase paciente"
```
**Explicación:** Guarda permanentemente los archivos preparados en el historial local del repositorio. El parámetro `-m` permite adjuntar un mensaje directo ("avance clase paciente"), el cual es fundamental para documentar de forma clara qué es lo que se hizo o avanzó en ese punto del código.

### 5. Enviar los cambios al servidor remoto (Push)
```bash
git push origin main
```
**Explicación:** Sube todos los commits (cambios registrados) locales a la rama `main` del servidor remoto (identificado por defecto como `origin`). Esto actualiza el repositorio en la nube con los últimos avances para que estén respaldados y disponibles.