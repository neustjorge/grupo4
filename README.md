# Commits modificacion 23/10/2024

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

