# 📘 Usa ```git log --oneline``` para ver el historial de commits rápidamente
En lugar de usar el comando largo git log, puedes usar:
```git
git log --oneline
```

Este comando muestra el historial de commits en una sola línea por commit, lo que lo hace mucho más fácil de leer.
## Ejemplo de salida:
```git
a1b2c3d Fix bug en login
f4e5g6h Agrega validación de formulario
i7j8k9l Inicializa proyecto
```

## ✅ Beneficios
- Ideal para revisar rápidamente el historial.
- Útil para encontrar el hash de un commit si necesitas hacer un revert, reset o checkout.
- Puedes combinarlo con otros filtros como:

```git
git log --oneline --author="Martinez Lira <jmartinez@exsoinf.com>"
```
