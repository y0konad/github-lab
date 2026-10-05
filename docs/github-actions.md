# Fundamentos de GitHub Actions

Estructura para automatizar pruebas, linters y despliegues continuos.

## Jerarquía de un Workflow
1. `name`: Identificador legible en la interfaz de GitHub.
2. `on`: Eventos disparadores (`push`, `pull_request`, `workflow_dispatch`).
3. `jobs`: Tareas que corren en paralelo por defecto (aisladas en máquinas virtuales).
4. `steps`: Secuencia ordenada de comandos o acciones (`uses:` o `run:`).

## Buenas Prácticas
- Pinning de acciones a SHA completo para garantizar inmutabilidad y seguridad.
- Utilizar `actions/cache` para acelerar instalaciones de dependencias (npm, pnpm, cargo).
- Limitar los permisos del token (`permissions: contents: read`) según el principio de mínimo privilegio.
