# 🔄 Cambiar de Rama en Git

Este tutorial te muestra cómo cambiar de rama en tu repositorio Git utilizando el comando moderno `git switch`.

---

## 🧠 ¿Qué es `git switch`?

`git switch` es un comando introducido en Git 2.23 para facilitar el cambio entre ramas. Es más intuitivo que el clásico `git checkout`.

## 🚀 Cambiar de rama
Para cambiar a una rama existente, usa:
```git
git switch nombre-de-la-rama
```

Ejemplo:
```git
git switch Desarrollo
```

En caso de tener cambios pendientes por subir te aparecerá el siguiente mensaje:
```git
jmartinez@ESIDELL04 MINGW64 /c/git/icm-tools-9 (F2-PorcentajeVenta)
$ git switch F2-CategoriaMontosMetas
error: Your local changes to the following files would be overwritten by checkout:
        ICMTools/Controllers/PorcentajeVentaController.vb
Please commit your changes or stash them before you switch branches.
Aborting
```

> Última Revisión: Lunes, 03 de Noviembre de 2025
