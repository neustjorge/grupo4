Comando git push
El comando git push se utiliza en Git para cargar los cambios locales a un repositorio remoto. Es el paso final en el flujo de trabajo de Git cuando has confirmado los cambios localmente y ahora deseas compartirlos con otros colaboradores en un servidor remoto.

Uso básico
git push <nombre-remoto> <nombre-rama>

**Ejemplos:**

1.  Empujar (push) los cambios de la rama `main` al repositorio remoto `origin`:
git push origin main

2. Empujar todos los commits locales a la rama predeterminada en el servidor remoto:
git push

## Uso avanzado
### Empujar una nueva rama

Cuando creas una nueva rama localmente y deseas compartirla en el repositorio remoto:
git push -u <nombre-remoto> <nombre-nueva-rama>
Esto no solo envía la nueva rama al repositorio remoto, sino que también la establece como la rama por defecto para futuros `git push`.

**Ejemplo:**
-   Empujar la nueva rama `feature/login` al remoto `origin`:
git push -u origin feature/login

### Empujar todos los cambios a todas las ramas
-   Para enviar todas las ramas locales que tengan cambios pendientes al repositorio remoto:
git push --all <nombre-remoto>

**Ejemplo:**
-   Enviar todas las ramas locales a `origin`
git push --all origin

### Eliminar una rama remota
Si deseas eliminar una rama en el servidor remoto:
git push <nombre-remoto> --delete <nombre-rama>

**Ejemplo:**
-   Eliminar la rama `feature/login` del repositorio remoto
git push origin --delete feature/login

### Forzar el envío (cuidado)
Si es necesario sobrescribir cambios en el repositorio remoto (lo cual debe hacerse con precaución), puedes forzar el push:
git push --force
