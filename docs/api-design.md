# Principios de Diseño de APIs REST

Lineamientos para crear interfaces HTTP predecibles y consistentes.

## Códigos de Estado Semánticos
- `200 OK`: Respuesta exitosa con cuerpo.
- `201 Created`: Recurso creado exitosamente (usar cabecera `Location` cuando aplique).
- `204 No Content`: Operación exitosa sin cuerpo de retorno (común en DELETE o actualizaciones silenciosas).
- `400 Bad Request`: Error de validación en la petición del cliente.
- `401 Unauthorized` vs `403 Forbidden`: Falta autenticación vs falta permiso.
- `404 Not Found`: Recurso inexistente.

## Idempotencia
- Métodos seguros e idempotentes: `GET`, `HEAD`, `OPTIONS`.
- Métodos idempotentes con mutación: `PUT`, `DELETE`.
- Método no idempotente por defecto: `POST`.
