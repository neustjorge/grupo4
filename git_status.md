# Git Status

## Descripción

El comando `git status` muestra el estado del repositorio Git en el que te encuentras, proporcionándote información clave sobre los cambios en tu área de trabajo y el área de preparación. Es uno de los comandos más utilizados en Git y ayuda a mantener el control sobre los cambios que se han realizado.

## Funcionalidad Principal

El comando `git status` realiza las siguientes acciones:
1. **Muestra los archivos en el área de preparación**: Archivos que están listos para ser confirmados (committed).
2. **Muestra los archivos modificados pero no preparados**: Cambios que han sido realizados pero no se han añadido al área de preparación.
3. **Archivos no rastreados**: Archivos nuevos que aún no han sido añadidos al control de versiones.

## Ejemplo de Salida

```bash
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)
        modified:   archivo1.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   archivo2.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        archivo3.txt
```

### Explicación de la Salida

1. **On branch**: Indica en qué rama te encuentras trabajando.
2. **Your branch is up to date**: Muestra si tu rama local está sincronizada con la rama remota.
3. **Changes to be committed**: Son los archivos que ya están en el área de preparación (staged) y listos para ser confirmados en el próximo commit.
4. **Changes not staged for commit**: Archivos modificados pero que no se han añadido al área de preparación.
5. **Untracked files**: Archivos que no están siendo rastreados por Git (nuevos archivos).

## Opciones Útiles

### `git status -s` o `git status --short`
Muestra el estado en un formato más conciso. Los prefijos indican el estado de cada archivo:

- `M`: Modificado (Modified)
- `A`: Añadido (Added)
- `??`: No rastreado (Untracked)

#### Ejemplo:
```bash
M archivo1.txt
?? archivo3.txt
```

### `git status -b`
Muestra información adicional sobre la rama actual, como el nombre de la rama y cuántos commits estás por delante o por detrás de la rama remota.

## Comandos Relacionados

- **`git add <archivo>`**: Añade un archivo modificado o no rastreado al área de preparación.
- **`git commit`**: Crea un commit con los cambios que están en el área de preparación.
- **`git restore <archivo>`**: Revierte los cambios en un archivo que no está preparado (staged).
- **`git reset <archivo>`**: Quita un archivo del área de preparación y lo devuelve al área de trabajo.

## Uso Práctico

El comando `git status` es útil para:
1. **Verificar qué cambios están listos para ser confirmados**.
2. **Controlar qué archivos han sido modificados o son nuevos**.
3. **Organizar tu área de preparación antes de un commit**.
4. **Evitar errores al empujar (push) cambios al repositorio remoto**.

## Buenas Prácticas

Es recomendable ejecutar `git status` con frecuencia mientras trabajas para estar siempre al tanto del estado de tus archivos. Esto te permite gestionar los cambios de manera efectiva y asegurarte de que todo esté en orden antes de hacer un commit.

## Ejemplo de Flujo de Trabajo

1. Modifica un archivo en tu repositorio.
2. Ejecuta `git status` para ver los cambios no preparados.
3. Añade el archivo al área de preparación con `git add <archivo>`.
4. Ejecuta `git status` nuevamente para verificar que el archivo esté listo para ser confirmado.
5. Realiza un commit con `git commit -m "Mensaje del commit"`.