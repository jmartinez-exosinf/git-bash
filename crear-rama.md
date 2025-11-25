# 🌿 Crear una Nueva Rama en Git

Este tutorial te guía paso a paso para crear una nueva rama en tu repositorio utilizando Git Bash.

---

## 🔄 1. Primero verifica que no tengas cambios pendientes por subir

Antes de crear una nueva rama, asegúrate de revisar si tienes cambios pendientes.

```git
git status
```

Si no tienes cambios pendientes por subir te debe aparecer algo como esto:
```git
jmartinez@ESIDELL04 MINGW64 /c/git/icm-tools-9 (TiendasGanadoras)
$ git status
On branch TiendasGanadoras
nothing to commit, working tree clean
```

## 🔄 2. Cambiar a la rama base (`Desarrollo`)

Antes de crear una nueva rama, asegúrate de estar en la rama desde la cual deseas partir. En este caso, la rama `Desarrollo`.
```git
git switch Desarrollo
```

Si todo se ejecuta correctamente te debe aparecer algo como esto:
```git
jmartinez@ESIDELL04 MINGW64 /c/git/icm-tools-9 (F2-TiendasGanadoras)
$ git switch Desarrollo
Switched to branch 'Desarrollo'
Your branch is up to date with 'origin/Desarrollo'.
```
De ser así, ve al paso 3.

En caso contrario, si te aparece algo como esto, significa que tienes cambios pendientes por actualizar en tu rama de Desarrollo local:
```git
jmartinez@ESIDELL04 MINGW64 /c/git/icm-tools-9 (TiendasGanadoras)
$ git switch Desarrollo
Switched to branch 'Desarrollo'
Your branch is behind 'origin/Desarrollo' by 10 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)
```

Para actualizar ejecutá los siguientes comandos:
```git
git fetch origin Desarrollo
git pull origin Desarrollo
```

## 🌱 3. Crear una nueva rama
Este comando crea una nueva rama y te cambia automáticamente a ella.

```git
git checkout -b [nombre-de-la-rama]
```

✅ Confirmar que estás en la nueva rama (opcional)
Puedes verificar que estás en la nueva rama con

```git
git branch
```

La rama actual aparecerá marcada con un asterisco *.

> Última Revisión: Ma, 25/Nov/25
