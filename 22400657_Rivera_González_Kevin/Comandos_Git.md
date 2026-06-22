1. git init: Inicializa un nuevo repositorio Git local en la carpeta actual. Convierte un directorio común en un repositorio listo para rastrear cambios.
Ejemplo:
git init
2. git clone: Descarga una copia exacta de un repositorio remoto (por ejemplo, desde GitHub) a tu máquina local.
Ejemplo:
git clone [https://github.com/usuario/mi-proyecto.git](https://www.google.com/search?q=https://github.com/usuario/mi-proyecto.git)
3. git status: Muestra el estado actual del directorio de trabajo. Te permite ver qué archivos han sido modificados, cuáles están listos para guardarse y cuáles no están siendo rastreados.
Ejemplo:
git status
4. git add: Añade los archivos modificados o nuevos al área de preparación (staging area) para incluirlos en el próximo commit.
Ejemplo para un archivo específico:
git add index.html
Ejemplo para añadir todos los archivos modificados:
git add .
5. git commit: Guarda permanentemente los cambios que están en el área de preparación en el historial del repositorio. Siempre se acompaña de un mensaje descriptivo.
Ejemplo:
git commit -m "Agregar la barra de navegacion principal"
6. git branch: Permite listar, crear o eliminar ramas. Si se ejecuta sin argumentos, muestra las ramas locales y resalta la rama actual.
Ejemplo para listar ramas:
git branch
Ejemplo para crear una nueva rama:
git branch nueva-funcion
7. git checkout: Permite cambiar de una rama a otra o restaurar archivos del historial de trabajo.
Ejemplo para cambiar de rama:
git checkout nueva-funcion
8. git switch: Es un comando moderno diseñado específicamente para cambiar de rama de una forma más segura y clara que 'git checkout'.
Ejemplo para cambiar de rama:
git switch main
Ejemplo para crear y cambiar a una nueva rama a la vez:
git switch -c mejora-interfaz
9. git merge: Une el historial de una rama distinta a la rama actual en la que te encuentras. Es ideal para integrar funciones terminadas.
Ejemplo (estando en la rama main):
git merge nueva-funcion
10. git remote add origin: Conecta tu repositorio Git local con un repositorio remoto vacío en GitHub por primera vez, asignándole el alias "origin".
Ejemplo:
git remote add origin [https://github.com/usuario/mi-proyecto.git](https://www.google.com/search?q=https://github.com/usuario/mi-proyecto.git)
11. git push: Envía los commits locales de tu rama actual a la rama correspondiente en el repositorio remoto (GitHub).
Ejemplo para el primer envío estableciendo la rama remota por defecto:
git push -u origin main
Ejemplo para envíos posteriores:
git push
12. git pull: Descarga e integra los últimos cambios del repositorio remoto en tu rama local actual. Es una combinación de los comandos 'fetch' y 'merge'.
Ejemplo:
git pull origin main
13. git fetch: Descarga el historial y las referencias del repositorio remoto (nuevas ramas o commits de tus compañeros) sin modificar ni mezclar nada en tus archivos de trabajo locales.
Ejemplo:
git fetch origin
14. git log: Muestra el historial completo de commits realizados en la rama actual, detallando el autor, la fecha, el identificador único (hash) y el mensaje de cada cambio.
Ejemplo:
git log
Ejemplo para ver el historial resumido en una línea por commit:
git log --oneline
15. git diff: Muestra las diferencias exactas de código entre los archivos modificados en tu directorio de trabajo y la última versión guardada.
Ejemplo:
git diff
16. git reset: Elimina cambios del área de preparación (unstage) o revierte el historial de commits a un punto anterior. El parámetro --hard borra los cambios por completo.
Ejemplo para quitar un archivo del área de preparación sin borrar su contenido:
git reset index.html
17. git stash: Guarda temporalmente tus cambios modificados que aún no están listos para un commit y limpia tu directorio de trabajo. Ideal para cambiar de rama rápido sin perder el progreso.
Ejemplo para guardar los cambios en pausa:
git stash
Ejemplo para recuperar esos cambios guardados más tarde:
git stash pop
18. git rm: Elimina archivos del repositorio (y del disco local de forma opcional) y los añade al área de preparación para el próximo commit.
Ejemplo:
git rm archivo-viejo.txt
19. git remote -v: Muestra la lista de los servidores remotos conectados a tu repositorio local junto con sus URLs de lectura (fetch) y escritura (push).
Ejemplo:
git remote -v
20. git revert: Crea un nuevo commit que deshace exactamente los cambios de un commit anterior. Es la forma segura de corregir errores en ramas públicas porque no altera el historial existente.
Ejemplo (usando el código identificador del commit a revertir):
git revert 7a12b3c
