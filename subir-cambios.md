# 🚀 Subir Cambios a un Repositorio Git

Este tutorial te guía paso a paso para subir tus cambios locales a un repositorio remoto utilizando Git Bash.

---

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

## 🌐 5. Verifica que los cambios se hayan guardado
```git
git status
```
