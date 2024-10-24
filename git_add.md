
# Comando Git Add

El comando `git add` se utiliza para agregar archivos al área de preparación (staging area) en Git. Este es el primer paso para realizar un commit de los cambios hechos en los archivos.

## Uso Básico

Aquí está la sintaxis básica para agregar un archivo específico:

```bash
git add <nombre_archivo>
```

Donde `<nombre_archivo>` es el archivo o los archivos que deseas agregar al área de preparación.

Si deseas agregar todos los archivos modificados y nuevos en el directorio de trabajo, puedes usar:

```bash
git add .
```

## Ejemplo

Supongamos que has modificado dos archivos, `index.html` y `style.css`, y deseas agregarlos al área de preparación. Aquí está el proceso:

1. **Verificar el estado de tus archivos**:
    ```bash
    git status
    ```

2. **Agregar archivos individualmente**:
    ```bash
    git add index.html
    git add style.css
    ```

3. **O agregar todos los archivos modificados a la vez**:
    ```bash
    git add .
    ```

4. **Confirmar el commit**:
    Después de agregar los archivos al área de preparación, puedes hacer un commit de los cambios:
    ```bash
    git commit -m "Modificados index.html y style.css"
    ```

## Agregar Solo Parte de un Archivo

A veces, es posible que desees agregar solo parte de un archivo en lugar de todo el archivo. Puedes hacer esto usando la opción interactiva `-p`:

```bash
git add -p <nombre_archivo>
```

Esto te permitirá revisar y seleccionar qué partes del archivo deseas agregar al área de preparación.

## Conclusion

El comando `git add` es una herramienta esencial en Git para preparar los cambios que deseas confirmar (commit). Te permite tener control total sobre qué cambios se incluyen en tus commits.
