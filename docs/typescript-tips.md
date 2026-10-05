# Patrones y Utilidades de TypeScript

Recomendaciones para mantener tipado estricto sin caer en sobre-ingeniería.

## Utilidades Estándar Clave
- `Pick<T, K>` y `Omit<T, K>`: Construir variantes acotadas de interfaces complejas.
- `Record<K, T>`: Definir mapas y diccionarios seguros con claves tipadas.
- `ReturnType<T>` y `Parameters<T>`: Extraer firmas de funciones de librerías externas.

## Discriminated Unions (Uniones Discriminadas)
Usar una propiedad literal común (ej. `kind: 'success' | 'error'`) para permitir que TypeScript estreche tipos automáticamente en bloques `switch` o `if`.
