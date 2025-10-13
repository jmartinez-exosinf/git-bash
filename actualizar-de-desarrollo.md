# 🧪 Mini Tutorial: Actualización de Rama de Desarrollo en Git

Este tutorial te guía paso a paso para validar, subir y sincronizar cambios en una rama de desarrollo utilizando Git Bash.

---

## 🔍 1. Validar estatus de cambios

Este comando muestra los archivos modificados, nuevos o eliminados que aún no están preparados para el commit.

git status

statusMostrar más líneas

📥 2. Subir cambios al área de staging
Agrega todos los archivos modificados al área de preparación para el commit.

git add .

✅ 3. Validar cambios preparados (opcional)
Verifica que los archivos aparezcan en verde, lo que indica que están listos para el commit

git status

📝 4. Realizar commit
Guarda los cambios preparados con un mensaje descriptivo.

git commit -m "[Descripción del cambio]"

🚀 5. Subir cambios al repositorio remoto (opcional)
Envía los commits locales a la rama correspondiente en el repositorio remoto.

git push origin [nombre-de-la-rama]

🔄 6. Sincronizar con el repositorio remoto
Obtiene los últimos cambios del repositorio remoto sin aplicarlos directamente.

git fetch

Mostrar más líneas

📤 7. Actualizar rama de desarrollo
Descarga y aplica los últimos cambios de la rama Desarrollo desde el repositorio remoto

git pull origin Desarrollo
