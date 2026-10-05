# Docker Essentials Cheatsheet

Comandos de mantenimiento y diagnóstico de contenedores.

## Ciclo de Vida y Limpieza
- Limpiar contenedores detenidos, redes huérfanas e imágenes no usadas: `docker system prune -f`
- Eliminar volúmenes huérfanos que ocupan espacio en disco: `docker volume prune -f`
- Ver consumo de memoria y CPU por contenedor en vivo: `docker stats`

## Inspección y Debugging
- Ver logs siguiendo el stream en vivo: `docker logs -f --tail 50 <contenedor>`
- Abrir una shell interactiva en contenedor en ejecución: `docker exec -it <contenedor> sh`
- Inspeccionar configuración IP y montajes: `docker inspect <contenedor>`
