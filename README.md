Tarea 1: introducción a Git

## Descripción
Este programa en Java imprime el mensaje "Hola Git". El objetivo de esta tarea es practicar el uso de Git y GitHub.

## Instrucciones de uso
Para ejecutar el programa, utiliza el siguiente comando:

Crea la carpeta y navega a ella:

bash
Copiar código
mkdir ProyectoEjemploGit
cd ProyectoEjemploGit
Inicializa el repositorio:

bash
Copiar código
git init
Crea el archivo HolaMundo.java:

java
Copiar código
// HolaMundo.java
public class HolaMundo {
    public static void main(String[] args) {
        System.out.println("Hola Mundo");
    }
}
Añade y realiza el primer commit:

bash
Copiar código
git add HolaMundo.java
git commit -m "Se agregó el programa de Hola Mundo en Java"
Paso 2: Segundo commit
Crea el archivo debug.log:

bash
Copiar código
touch debug.log
Crea el archivo .gitignore:

bash
Copiar código
echo "*.log" > .gitignore
Añade y realiza el segundo commit:

bash
Copiar código
git add .gitignore
git commit -m "Se agregó el archivo .gitignore"
Verifica que debug.log es ignorado:

bash
Copiar código
git status
En la salida, debug.log no debería aparecer.

Paso 3: Tercer commit
Actualiza HolaMundo.java:

java
Copiar código
// HolaMundo.java
public class HolaMundo {
    public static void main(String[] args) {
        System.out.println("Hola Git");
    }
}
Añade y realiza el tercer commit:

bash
Copiar código
git add HolaMundo.java
git commit -m "Se actualizó el mensaje en HolaMundo.java"
Paso 4: Subir los cambios a un repositorio remoto
Crea un repositorio público en GitHub.

Ve a GitHub y crea un nuevo repositorio, por ejemplo, "ProyectoEjemploGit".
Conecta el repositorio local al remoto:

bash
Copiar código
git remote add origin https://github.com/tu_usuario/ProyectoEjemploGit.git
Sube los cambios al repositorio remoto:

bash
Copiar código
git push -u origin master
Verifica en GitHub que los archivos se han subido correctamente (asegúrate de que debug.log no esté presente).

Paso 5: Crear un archivo README.md
Crea el archivo README.md:

bash
Copiar código
touch README.md
Escribe el contenido usando Markdown:

markdown
Copiar código
# Proyecto Ejemplo Git

## Descripción
Este programa en Java imprime el mensaje "Hola Git". El objetivo de esta tarea es practicar el uso de Git y GitHub.

## Instrucciones de uso
Para ejecutar el programa, utiliza el siguiente comando:
javac HolaMundo.java java HolaMundo

markdown
Copiar código

## Comandos utilizados
- `git init`
- `git add <archivo>`
- `git commit -m "<mensaje>"`
- `git remote add origin <url>`
- `git push -u origin master`
- `git status`

## Notas sobre el archivo .gitignore
Se creó para ignorar los archivos con extensión `.log`, específicamente `debug.log`, que no son necesarios en el repositorio.

Al ejecutar el programa, se debe mostrar el mensaje "Hola Git". Para verificar que `debug.log` no se subió, revisa la lista de archivos en el repositorio en GitHub.
Añade y realiza el commit del README.md:

bash
Copiar código
git add README.md
git commit -m "Se agregó el archivo README.md"
git push origin master
