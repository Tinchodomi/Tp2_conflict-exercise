# Tp2_conflict-exercise
Tp2_actividad3

ESTE ES UN CAMBIO EN LA BRANCH MAIN

3) Realizar la siguiente actividad:
Paso 1: Crear un repositorio en GitHub
• Ve a GitHub e inicia sesión en tu cuenta.
• Haz clic en el botón "New" o "Create repository" para crear un nuevo
repositorio.
• Asigna un nombre al repositorio, por ejemplo, conflict-exercise.
• Opcionalmente, añade una descripción.
• Marca la opción "Initialize this repository with a README".
• Haz clic en "Create repository".
Paso 2: Clonar el repositorio a tu máquina local
• Copia la URL del repositorio (usualmente algo como
https://github.com/tuusuario/conflict-exercise.git).
• Abre la terminal o línea de comandos en tu máquina.
• Clona el repositorio usando el comando:
git clone https://github.com/tuusuario/conflict-exercise.git
• Entra en el directorio del repositorio:
cd conflict-exercise
Paso 3: Crear una nueva rama y editar un archivo
• Crea una nueva rama llamada feature-branch:
git checkout -b feature-branch
• Abre el archivo README.md en un editor de texto y añade una línea nueva,
por ejemplo:
Este es un cambio en la feature branch.
• Guarda los cambios y haz un commit:
git add README.md
git commit -m "Added a line in feature-branch"
Paso 4: Volver a la rama principal y editar el mismo archivo
• Cambia de vuelta a la rama principal (main):
git checkout main
• Edita el archivo README.md de nuevo, añadiendo una línea diferente:
Este es un cambio en la main branch.
• Guarda los cambios y haz un commit:
git add README.md
git commit -m "Added a line in main branch"
Paso 5: Hacer un merge y generar un conflicto
• Intenta hacer un merge de la feature-branch en la rama main:
git merge feature-branch
• Se generará un conflicto porque ambos cambios afectan la misma línea del
archivo README.md.
Paso 6: Resolver el conflicto
• Abre el archivo README.md en tu editor de texto. Verás algo similar a esto:
<<<<<<< HEAD
Este es un cambio en la main branch.
=======
Este es un cambio en la feature branch.
>>>>>>> feature-branch
• Decide cómo resolver el conflicto. Puedes mantener ambos cambios, elegir
uno de ellos, o fusionar los contenidos de alguna manera.
• Edita el archivo para resolver el conflicto y guarda los cambios(Se debe borrar
lo marcado en verde en el archivo donde estes solucionando el conflicto. Y se
debe borrar la parte del texto que no se quiera dejar).
• Añade el archivo resuelto y completa el merge:
git add README.md
git commit -m "Resolved merge conflict"
Paso 7: Subir los cambios a GitHub
• Sube los cambios de la rama main al repositorio remoto en GitHub:
git push origin main
>>>>>>> • También sube la feature-branch si deseas:
git push origin feature-branch
Paso 8: Verificar en GitHub
• Ve a tu repositorio en GitHub y revisa el archivo README.md para confirmar
que los cambios se han subido correctamente.
• Puedes revisar el historial de commits para ver el conflicto y su resolución.
