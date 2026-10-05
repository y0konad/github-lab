# Atajos y Productividad en Bash

Técnicas esenciales para agilizar el trabajo en la terminal de Linux.

## Navegación y Atajos Readline
- `Ctrl + R`: Búsqueda interactiva en el historial de comandos.
- `Ctrl + A` / `Ctrl + E`: Ir al inicio / final de la línea actual.
- `Ctrl + U` / `Ctrl + K`: Borrar desde el cursor al inicio / final de línea.
- `Alt + .`: Pegar el último argumento del comando anterior.

## Pipes y Redirecciones
- Redirigir stdout y stderr a un log: `comando > out.log 2>&1`
- Silenciar salida de error: `comando 2>/dev/null`
- Redirección con buffer en tiempo real: `tail -f app.log | grep --line-buffered "ERROR"`
