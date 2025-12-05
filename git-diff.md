# 🔍 ¿Qué hace git diff?
git diff compara diferencias entre archivos en distintas áreas del repositorio:

Área de trabajo (working directory) vs último commit
Staging area vs último commit
Entre commits específicos
Entre ramas


✅ 1. Ver cambios no preparados (working directory vs último commit)
Shellgit diffShow more lines
Muestra los cambios que hiciste en los archivos pero que no están en staging.

✅ 2. Ver cambios preparados (staging vs último commit)
Shellgit diff --cachedShow more lines
Muestra los cambios que ya agregaste con git add y que se incluirán en el próximo commit.

✅ 3. Comparar dos commits
Shellgit diff <commit1> <commit2>Show more lines
Ejemplo:
Shellgit diff abc123 def456Show more lines
Esto muestra las diferencias entre esos dos commits.

✅ 4. Comparar ramas
Shellgit diff main feature-branchShow more lines
Muestra las diferencias entre la rama main y feature-branch.

✅ 5. Ver solo nombres de archivos modificados
Shellgit diff --name-onlyShow more lines

✅ 6. Ver diferencias con formato unificado (resumen)
Shellgit diff --statShow more lines
Ejemplo:
 file1.txt | 2 +-
 file2.txt | 5 +++--


🔥 Tip extra
Si quieres ver diferencias ignorando espacios en blanco:
Shellgit diff -w
