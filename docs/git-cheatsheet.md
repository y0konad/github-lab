# Guía Rápida de Git para el Día a Día

Apuntes prácticos para resolver situaciones cotidianas en terminal sin fricción.

## Manejo de Cambios y Ramas
- Crear y saltar a una rama nueva: `git checkout -b feature/nombre`
- Descartar cambios sin commitear en un archivo: `git restore archivo.ext`
- Guardar cambios temporalmente en el cajón: `git stash push -m "en progreso"`
- Recuperar el último stash: `git stash pop`

## Historial y Limpieza
- Ver historial compacto en árbol: `git log --oneline --graph --decorate -n 15`
- Modificar el último commit (sin cambiar historial público): `git commit --amend --no-edit`
- Deshacer el último commit preservando el código en el editor: `git reset --soft HEAD~1`
