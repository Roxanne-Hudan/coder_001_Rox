## Uso de Git

dev = prueba 

crear una rama o branch llamada dev, que es una abreviatura de development, es decir, desarollo:

    git branch dev

Cambiar de rama:

    git switch dev
    git checkout dev

Listar ramas para ver que se este bien parado.

    git branch

Hacer los cambios necesarios y enviarlos al staging area.

    git add archivo 

O, si queremos ásar todos los archivos, hacer:

    git add . 

Luego, crear un commit con un mensaje:

    git commit -m "Comentario sobre los cambios Hechos"

Una vez que se terminaron de hacer los commit´s necesarios y se les quiere fusionar a la rama principal, tener cuidado de no dejar archivos con cambios sin commit. 

Pararse en la rama principal:

    git checkout main

Fusionar los commits de la rama dev o prueba en main:

    git merge prueba

Se puede seguir trabjando en prueba

    git checkout prueba

o se le puede borrar 

    git branch -D prueba

Cuando se quiera subir los cambios a la nube, es decir, a GitHub, cambiarse a la rama principal:

    git checkout main

y luego "Empujar" todos los commits nuevos a la rama main en GitHub (Se llama origin/main)

    git push