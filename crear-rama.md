# 🌿 Mini Tutorial: Crear una Nueva Rama en Git

Este tutorial te guía paso a paso para crear una nueva rama en tu repositorio utilizando Git Bash.

---

## 🔄 1. Cambiar a la rama base (`Desarrollo`)

Antes de crear una nueva rama, asegúrate de estar en la rama desde la cual deseas partir. En este caso, la rama `Desarrollo`.


git switch Desarrollo

🌱 2. Crear una nueva rama
Este comando crea una nueva rama y te cambia automáticamente a ella.

git checkout -b [nombre-de-la-rama]

Reemplaza [nombre-de-la-rama] por el nombre que desees darle a tu nueva rama, por ejemplo:

git checkout -b feature/login

✅ Confirmar que estás en la nueva rama (opcional)
Puedes verificar que estás en la nueva rama con

git branch

La rama actual aparecerá marcada con un asterisco *.
