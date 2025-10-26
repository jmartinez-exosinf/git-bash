# 🔄 Mini Tutorial: Renombrar una Rama Local en Git

Este tutorial te muestra cómo cambiar el nombre de una rama local en Git utilizando el comando `git branch -m`.

---

## 🧠 ¿Cuándo usarlo?

Renombrar una rama puede ser útil cuando:

- El nombre original no describe bien su propósito.
- Quieres seguir una convención de nombres más clara.
- Cometiste un error al nombrarla inicialmente.

---

## 🛠️ Comando para renombrar una rama

### ✅ Si estás en la rama que deseas renombrar:

```bash
git branch -m nuevo-nombre
```

### 🔁 Si estás en otra rama y quieres renombrar una diferente:
git branch -m nombre-antiguo nuevo-nombre

Ejemplo:
git branch -m hotfix/login-error fix/login-validation

## ⚠️ Recomendaciones

Asegúrate de no tener conflictos antes de renombrar.
Si la rama ya fue publicada en un repositorio remoto, deberás eliminar la antigua y subir la nueva manualmente.
