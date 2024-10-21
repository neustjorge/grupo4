# Commits - Buenas Prácticas

Este documento tiene como objetivo guiar sobre cómo realizar **commits** de manera efectiva en proyectos de software, utilizando Git como sistema de control de versiones.

## ¿Qué es un Commit?

Un **commit** en Git es un registro de los cambios hechos en el código. Cada commit tiene un identificador único y está acompañado de un mensaje descriptivo que explica los cambios realizados.

## ¿Por qué son importantes los Commits?

Los commits son esenciales para:
- **Mantener un historial claro de cambios**: Permiten rastrear la evolución del proyecto a lo largo del tiempo.
- **Facilitar la colaboración**: Ayudan a otros desarrolladores a entender qué cambios se hicieron y por qué.
- **Recuperar versiones anteriores**: Si algo sale mal, puedes revertir los cambios fácilmente.

## Cómo hacer un Commit

Para realizar un commit en Git, sigue estos pasos:

1. **Añadir los cambios al área de preparación (staging area)**:
   ```bash
   git add <archivo>   # Añade un archivo específico
   git add .           # Añade todos los archivos modificados

   
¡Claro! Aquí tienes un ejemplo de archivo README.md relacionado con la gestión de commits en un repositorio de control de versiones, como Git. Este archivo explica cómo realizar commits efectivos y buenas prácticas.

markdown
Copiar código
# Commits - Buenas Prácticas

Este documento tiene como objetivo guiar sobre cómo realizar **commits** de manera efectiva en proyectos de software, utilizando Git como sistema de control de versiones.

## ¿Qué es un Commit?

Un **commit** en Git es un registro de los cambios hechos en el código. Cada commit tiene un identificador único y está acompañado de un mensaje descriptivo que explica los cambios realizados.

## ¿Por qué son importantes los Commits?

Los commits son esenciales para:
- **Mantener un historial claro de cambios**: Permiten rastrear la evolución del proyecto a lo largo del tiempo.
- **Facilitar la colaboración**: Ayudan a otros desarrolladores a entender qué cambios se hicieron y por qué.
- **Recuperar versiones anteriores**: Si algo sale mal, puedes revertir los cambios fácilmente.

## Cómo hacer un Commit

Para realizar un commit en Git, sigue estos pasos:

1. **Añadir los cambios al área de preparación (staging area)**:
   ```bash
   git add <archivo>   # Añade un archivo específico
   git add .           # Añade todos los archivos modificados
Hacer el commit:

bash
Copiar código
git commit -m "Mensaje descriptivo"
Empujar los cambios al repositorio remoto:

bash
Copiar código
git push origin <rama>
Buenas Prácticas para Commits
1. Realiza commits pequeños y frecuentes
Realiza un commit por cada cambio lógico y pequeño. Esto facilita el seguimiento de cambios y la identificación de errores.
Evita commits grandes con múltiples cambios no relacionados.
2. Escribe mensajes de commit claros y descriptivos
El mensaje del commit debe describir claramente qué cambios se realizaron y por qué.
Usa el siguiente formato recomendado:
yaml
Copiar código
Tipo de cambio: Breve descripción

Detalles adicionales si es necesario.
Ejemplo:
makefile
Copiar código
feat: Añadida nueva funcionalidad de búsqueda avanzada

La funcionalidad de búsqueda ahora permite filtrar por múltiples criterios.
3. Usa el presente para los mensajes de commit
Escribe los mensajes en presente imperativo, como si dieras una orden: "Añadir", "Corregir", "Eliminar". Ejemplo: "Corregir error en la autenticación".
4. Agrupa cambios relacionados
Si trabajas en una nueva característica, asegúrate de que todos los cambios relacionados estén agrupados en un solo commit.
5. Incluye referencias a issues o tareas
Si estás trabajando en una tarea específica, incluye el identificador del issue o la tarea en el mensaje de commit. Ejemplo:
yaml
Copiar código
fix: Resolver bug #123 en la página de inicio
6. Evita los commits "WIP" (Work In Progress)
No hagas commits de trabajo en progreso (WIP). Solo realiza un commit cuando los cambios estén listos para ser compartidos.
Tipos de Commits
Aquí algunos ejemplos de tipos de commit:

feat: Añade una nueva funcionalidad.
fix: Soluciona un bug.
refactor: Refactoriza el código sin cambiar la funcionalidad.
docs: Cambios en la documentación.
style: Cambios que no afectan la lógica del código (espacios, formato).
test: Añade o modifica tests.
chore: Actualización de tareas rutinarias (dependencias, configuraciones).
Revertir un Commit
Si necesitas deshacer un commit, puedes usar el siguiente comando:

bash
Copiar código
git revert <commit_id>
Este comando crea un nuevo commit que revierte los cambios hechos en el commit especificado.

Resumen
Realiza commits pequeños y enfocados.
Escribe mensajes claros y en presente.
Agrupa cambios lógicos en un solo commit.
Evita commits WIP.
Usa tipos de commit estándar para mantener consistencia.
