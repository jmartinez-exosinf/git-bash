# 🧪 Actualización de Rama

Este tutorial te guía paso a paso para validar, subir y sincronizar cambios en una rama de desarrollo utilizando Git Bash.

---

## 🔍 1. Lo primero es validar si existen cambios pendientes por subir

Este comando muestra los archivos modificados, nuevos o eliminados que aún no están preparados para el commit.

```git
git status
```

Si no tienes cambios pendientes por subir te debe aparecer algo como esto:
```git
jmartinez@ESIDELL04 MINGW64 /c/git/icm-tools-9 (F2-PorcentajeVenta)
$ git status
On branch F2-PorcentajeVenta
nothing to commit, working tree clean
```
De ser así, ve al Paso 3.

Caso contrario, te aparecerá algo como esto:
```git
jmartinez@ESIDELL04 MINGW64 /c/git/icm-tools-9 (F2-TiendasGanadoras)
$ git status
On branch F2-TiendasGanadoras
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   ICMTools/Controllers/TiendasGanadorasController.vb
        modified:   ICMTools/Pages/TiendasGanadoras.aspx
        modified:   ICMTools/Pages/TiendasGanadoras.aspx.designer.vb
        modified:   ICMTools/js/TiendasGanadoras.js

no changes added to commit (use "git add" and/or "git commit -a")
```

En caso de tener cambios pendientes por subir, ve al siguiente enlace:
[Subir Cambios](https://github.com/jmartinez-exosinf/git-bash/blob/main/subir-cambios.md)


## 🔄 2. Sincronizar con el repositorio remoto
Obtiene los últimos cambios del repositorio remoto sin aplicarlos directamente.

```git
git fetch origin Desarrollo
```

📤 Actualizar rama de desarrollo
Descarga y aplica los últimos cambios de la rama Desarrollo desde el repositorio remoto

```git
git pull origin Desarrollo
```

### En caso de aparecer la pantalla de unix
Presiona ESC y posteriormente teclea ```:wq```

Si todo esta correcto te debe aparecer algo como lo siguiente:
```git
jmartinez@ESIDELL04 MINGW64 /c/git/icm-tools-9 (F2-PorcentajeVenta)
$ git pull origin Desarrollo
From https://gitlab.tgv.com.ar/aam-soporte/icm-tools-9
 * branch            Desarrollo -> FETCH_HEAD
Already up to date.
```

Finalmente escribe ```git status``` para confirmar que todo este correcto

## 4. En caso de existir conflictos

### A. En caso de existir conflictos aparecerá algo como esto:
```git
CONFLICT (content): Merge conflict in ICMTools/Controllers/PorcentajeVentaController.vb
```

### B. Corrige los conflictos en Visual Studio
