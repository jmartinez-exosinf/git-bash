# 🧨 Deshacer Todos los Cambios y Volver al Último Commit en Git

Este tutorial te muestra cómo **descartar todos los cambios locales** y regresar al último commit confirmado en tu repositorio Git utilizando Git Bash.

---

## ⚠️ Advertencia Importante

El siguiente comando **elimina todos los cambios locales** en tu directorio de trabajo, incluyendo archivos modificados y no guardados.  
**No se pueden recuperar fácilmente**, así que asegúrate de que realmente deseas descartar los cambios antes de continuar.

---

## 🔄 Comando para deshacer todos los cambios
```bash
git reset --hard HEAD
```

Este comando:

Revierte todos los archivos modificados al último commit.
Elimina cualquier cambio no guardado (sin add ni commit).


✅ Verificar que se aplicó correctamente
Después de ejecutar el comando, puedes usar:
```bash
git status
```
