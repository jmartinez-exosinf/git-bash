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

## 📥 2. Si tienes cambios pendientes por subir

### A. Agrega todos los archivos modificados al área de preparación para el commit

```git
git add .
```

### B. Validar cambios preparados (opcional)
Verifica que los archivos aparezcan en verde, lo que indica que están listos para el commit

```git
git status
```

### 📝 C. Realizar commit
Guarda los cambios preparados con un mensaje descriptivo.

```git
git commit -m "[Descripción del cambio]"
```

🚀 5. Subir cambios al repositorio remoto (opcional)
Envía los commits locales a la rama correspondiente en el repositorio remoto.

```git
git push origin [nombre-de-la-rama]
```

## 🔄 3. Sincronizar con el repositorio remoto
Obtiene los últimos cambios del repositorio remoto sin aplicarlos directamente.

```git
git fetch origin Desarrollo
```

📤 Actualizar rama de desarrollo
Descarga y aplica los últimos cambios de la rama Desarrollo desde el repositorio remoto

```git
git pull origin Desarrollo
```

En caso de aparecer la pantalla de unix, presiona ESC y posteriormente teclea ```:wq```

## 4. En caso de existir conflictos

### A. En caso de existir conflictos aparecerá algo como esto:
```git
CONFLICT (content): Merge conflict in ICMTools/Controllers/PorcentajeVentaController.vb
```

### B. Corrige los conflictos en Visual Studio
