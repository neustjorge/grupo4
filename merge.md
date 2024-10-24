El comando git merge se utiliza para unir dos o más ramas de trabajo en Git. Su función principal es integrar los cambios de una rama (source branch) en la rama actual (target branch). Es una herramienta esencial en el flujo de trabajo de Git, permitiendo combinar esfuerzos de desarrollo paralelos y colaborativos.

1. Funcionamiento
Preparación: Antes de realizar un merge, es recomendable asegurarse de estar en la rama de destino, generalmente mediante el comando git checkout:
git checkout main

2. Ejecución del merge:
git merge <nombre-rama>

Este comando intenta fusionar los cambios de la rama <nombre-rama> en la rama actual.

Tipos de merge:

Fast-forward: Si la rama de destino no ha avanzado y la rama fuente es un descendiente directo, Git simplemente "moverá" el puntero de la rama de destino hacia adelante, sin crear un nuevo commit de merge.
Merge con commit: Si las ramas han avanzado de forma independiente, Git intentará combinar los cambios y creará un commit de merge para reflejar la unión.
Merge con conflictos: Si los mismos archivos fueron modificados en ambas ramas de forma incompatible, Git reportará un conflicto que debe ser resuelto manualmente antes de completar el merge.
Resolución de conflictos: Si se produce un conflicto, Git marcará los archivos involucrados. El desarrollador debe resolver manualmente los conflictos, editando los archivos y luego marcarlos como resueltos:
git add <archivo-resuelto>

Después, completar el merge:
git commit
Finalización: Al finalizar, la historia de la rama mostrará la unión de los cambios en un punto de convergencia (en el caso de un merge con commit), o simplemente avanzará si fue un fast-forward.

Buenas Prácticas
Antes de fusionar, es buena idea asegurarse de que la rama de destino esté actualizada ejecutando git fetch y luego un git pull.
Realizar merges regularmente para evitar grandes conflictos de integración.
Usar ramas descriptivas y commits claros para facilitar el entendimiento del código al hacer merges.
