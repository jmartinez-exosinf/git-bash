# 🌿 Mini Tutorial: Crear una Nueva Rama en Git

Este tutorial te guía paso a paso para crear una nueva rama en tu repositorio utilizando Git Bash.

---

## 🔄 1. Primero verifica que no tengas cambios pendientes por subir

Antes de crear una nueva rama, asegúrate de revisar si tienes cambios pendientes.

```git
git status
```

## 🔄 2. Cambiar a la rama base (`Desarrollo`)

Antes de crear una nueva rama, asegúrate de estar en la rama desde la cual deseas partir. En este caso, la rama `Desarrollo`.

```git
git switch Desarrollo
```

🌱 2. Crear una nueva rama
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
