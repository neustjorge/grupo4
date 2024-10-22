# Git Branch

## Índice

- [Git Branch](#git-branch)
  - [Índice](#índice)
  - [¿Qué es una rama en Git?](#qué-es-una-rama-en-git)
  - [Comandos Básicos de Git Branch](#comandos-básicos-de-git-branch)
    - [1. Crear una nueva rama](#1-crear-una-nueva-rama)
    - [2. Ver todas las ramas](#2-ver-todas-las-ramas)
    - [3. Cambiar de rama](#3-cambiar-de-rama)
    - [4. Eliminar una rama](#4-eliminar-una-rama)
    - [5. Fusionar una rama](#5-fusionar-una-rama)
    - [Cambiar de rama](#cambiar-de-rama)
    - [Y Fusionar](#y-fusionar)
    - [6. Renombrar una rama](#6-renombrar-una-rama)
    - [6.1 Renombrar desde otra rama](#61-renombrar-desde-otra-rama)
    - [7 Ver el último commit de cada rama](#7-ver-el-último-commit-de-cada-rama)
    - [8 Mostrar ramas que ya han sido fusionadas](#8-mostrar-ramas-que-ya-han-sido-fusionadas)
    - [9 Mostrar ramas no fusionadas](#9-mostrar-ramas-no-fusionadas)
- [Trabajando con ramas remotas](#trabajando-con-ramas-remotas)
    - [1. Ver ramas remotas](#1-ver-ramas-remotas)
    - [2. Traer una rama remota](#2-traer-una-rama-remota)
    - [3. Eliminar una rama remota](#3-eliminar-una-rama-remota)
    - [4. Forzar la actualización de una rama remota](#4-forzar-la-actualización-de-una-rama-remota)

---

## ¿Qué es una rama en Git?

Una rama en Git es simplemente un puntero a un commit específico en el historial de un repositorio. La rama principal en Git se llama `main` (antes conocida como `master`), pero puedes crear otras ramas para desarrollar nuevas características, corregir errores o experimentar sin afectar la rama principal.  


## Comandos Básicos de Git Branch

A continuación se describen algunos de los comandos más comunes relacionados con las ramas en Git.  


### 1. Crear una nueva rama

Para crear una nueva rama, puedes usar el siguiente comando:

```bash
git branch <nombre-de-la-rama>
```

### 2. Ver todas las ramas

```bash
git branch
```


### 3. Cambiar de rama

```bash
git checkout <nuevo-nombre>
```


### 4. Eliminar una rama

```bash
git branch -d <nombre-de-la-rama> 
```


### 5. Fusionar una rama

### Cambiar de rama

```bash
git checkout main
```


### Y Fusionar

```bash
git merge <nombre-de-la-rama>
```


### 6. Renombrar una rama

```bash
git branch -m <nuevo-nombre>
```

### 6.1 Renombrar desde otra rama

```bash
git branch -m <nombre-antiguo> <nuevo-nombre>
```

### 7 Ver el último commit de cada rama

```bash
git branch -v
```

### 8 Mostrar ramas que ya han sido fusionadas

```bash
git branch --merged
```

### 9 Mostrar ramas no fusionadas

```bash
git branch --no-merged
```

# Trabajando con ramas remotas

### 1. Ver ramas remotas

```bash
git branch -r
```

### 2. Traer una rama remota

```bash
git checkout -t origin/<nombre-de-la-rama>
```

### 3. Eliminar una rama remota

```bash
git push origin --delete <nombre-de-la-rama>
```

### 4. Forzar la actualización de una rama remota

```bash
git push --force origin <nombre-de-la-rama>
```
