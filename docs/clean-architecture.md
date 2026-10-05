# Clean Architecture: Separación de Responsabilidades

Guía conceptual para desacoplar lógica de negocio de frameworks y bases de datos.

## Capas Concéntricas
1. **Entidades (Dominio)**: Reglas de negocio universales e invariantes del sistema.
2. **Casos de Uso (Aplicación)**: Orquestación de flujos de trabajo específicos de la aplicación.
3. **Adaptadores de Interfaz**: Controladores, presentadores, repositorios concretos y gateways.
4. **Frameworks y Drivers**: Base de datos, servidor web (Express, Fastify, Axum), librerías UI.

## La Regla de Dependencia
El código de las capas internas **nunca** debe conocer ni importar código de las capas externas. El flujo de control se invierte mediante interfaces e inyección de dependencias.
