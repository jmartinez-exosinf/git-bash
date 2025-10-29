# 🚀 Subir Cambios a un Repositorio Git

Este tutorial te guía paso a paso para subir tus cambios locales a un repositorio remoto utilizando Git Bash.

---

## ✅ 1. Verificar los archivos editados
Utiliza este comando para verificar que aparezcan los archivos que haz editado

```git
git status
```

En rojo aparecerán los archivos pendientes de subir
```git
jmartinez@ESIDELL04 MINGW64 /c/git/icm-tools-9 (F2-PorcentajeVenta)
$ git status
On branch F2-PorcentajeVenta
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   ICMTools/Controllers/PorcentajeVentaController.vb
        modified:   ICMTools/Pages/PorcentajeVenta.aspx
        modified:   ICMTools/js/PorcentajeVenta.js
```

## 📥 1. Agregar archivos al área de staging

Este comando agrega **todos los archivos modificados y nuevos** al área de preparación para el commit:

```git
git add .
```

## ✅ 2. Verificar los archivos preparado
Este comando te permite revisar qué archivos están listos para ser confirmados (commit). Los archivos en verde están en el área de staging

```git
git status
```

## 📝 3. Realizar el commit
Guarda los cambios preparados con un mensaje descriptivo que explique qué se modificó

```git
git commit -m "[Descripción del cambio]"
```

Ejemplo:
```git
git commit -m "Corrige validación de formulario de login"
```

"Mostrar más líneas

## 🌐 4. Subir los cambios al repositorio remoto
Envía los commits locales a la rama correspondiente en el repositorio remoto

```git
git push origin [nombre-de-la-rama]
```

Ejemplo:
```git
git push origin Proyecto
```

### Errores comunes al subir cambios al repositorio remoto
- Repositorio mal escrito o inexistente
```git
error: src refspec [RAMA] does not match any
error: failed to push some refs to 'https://gitlab.tgv.com.ar/aam-soporte/icm-tools-9.git'
```

- Repositorio desactualizado
```git
jmartinez@ESIDELL04 MINGW64 /c/git/icm-tools-9 (F2-VariableEntradaEnfoque)
$ git push origin F2-VariableEntradaEnfoque
To https://gitlab.tgv.com.ar/aam-soporte/icm-tools-9.git
 ! [rejected]        F2-VariableEntradaEnfoque -> F2-VariableEntradaEnfoque (fetch first)
error: failed to push some refs to 'https://gitlab.tgv.com.ar/aam-soporte/icm-tools-9.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
```

En este caso deberás ingresar el comando ```pull```
```git
git pull origin [nombre-de-la-rama]
```

## 🌐 5. Verifica que los cambios se hayan guardado
```git
git status
```

Si todo esta correcto, te debe aparecer algo similar a lo siguiente:
```git
jmartinez@ESIDELL04 MINGW64 /c/git/icm-tools-9 (F2-TiendasGanadoras)
$ git status
On branch F2-TiendasGanadoras
nothing to commit, working tree clean
```
