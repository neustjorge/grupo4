# Comando Push
## El comando `git push` te permite subir los commits desde tu rama (branch) local en tu repositorio git local al repositorio remoto.

Para poder subir a tu repositorio remoto, te debes asegurar de  **hacer commit a todos tus cambios al repositorio local.**

La sintaxis de ese comando es la siguiente:

```bash
git push <nombre del repositorio> <nombre de la rama>
```

Existen diferentes opciones que puedes pasar a este comando, puedes aprender más acerca de estos en la documentación de Git o ejecuta `git push --help`.

### **Subir a un repositorio remoto y rama específica.**

En orden para subir tu código, primero debes clonar un repositorio a tu máquina local.

```bash
# Una vez clonado el repositorio, estarás trabajando dentro de la rama por defecto (Por defecto es `main`)
git clone https://github.com/<git-usuario>/<nombre-repo> && cd <nombre-repo>
# Haz cambios y agrega tus archivos (repite el comando `git add` por cada archivo, o utiliza `git add .` para agregarlos todos)
git add <nombre-archivo>
# Ahora haz el commit de tu código
git commit -m "Agregué cambios a mi repo!"
# Sube los cambios en la rama 'main' a github
git push origin main
```

### **Subir a un repositorio remoto específico y todas las ramas que contiene.**

Si quieres subir todos tus cambios al repositorio remoto con todo y sus ramas, puedes utilizar:

```bash
git push --all <NOMBRE-REMOTO>
```

el cual:

-   `--all`  es la bandera que señala que quieres subir todas las ramas al repositorio remoto.
-   `NOMBRE-REMOTO`  es el nombre del repositorio remoto al cual las quieres subir.

**Subir a una rama específica con el parámetro** _force_

Si quieres ignorar los cambios locales hechos al repositorio Git en Github(Lo cual hacen la mayoría de desarrolladores para dar una solución rápida al servidor de desarrollo) luego puedes usar el comando —force para subir ignorando esos cambios.

`    
En la cual:

- `NOMBRE-REMOTO`  es el nombre del repositorio remoto al cual quieres subir los cambios.- `RAMA-REMOTA`  es el nombre de la rama remota a la cual quieres subir los cambios.  
  

###**Subir ignorando el hook pre-push de Git** 

Por defecto  `git push`  disparará el interruptor  `--verify`. Esto significa que git ejecutará cualquier script pre-push(antes de subirlo) del lado del cliente, que haya sido configurado. Si el script pre-push falla, también fallará el git push. ( Hooks Pre-Push son buenos para hacer cosas como, revisar si los mensajes al hacer commit están dentro del estándar de la empresa, ejecutar tests unitarios, etc...). Ocasionalmente podrías querer ignorar este comportamiento por defecto, por ejemplo: en el escenario donde quisieras subir tus cambios a una rama en particular para que otro colaborador la descargue, pero los cambios en tu trabajo en progreso rompen los tests unitarios. Para ignorar el hook, simplemente inserta tu comando push y añade la bandera `--no-verify`

` ` ` bash git push --no-verify ` ` `                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            
