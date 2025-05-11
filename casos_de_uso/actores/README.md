# Actores del Sistema

Los actores son entidades externas que interactúan con el sistema Novus. Pueden ser personas, otros sistemas o dispositivos.

## Descripción

Este documento define los actores principales del sistema Novus y sus características:

## Diagrama

![Diagrama de Actores](../../documentos/imagenes/diagrama_actores.png)

## Actores Principales

### NO_BECARIO
- **Descripción**: Postulantes que aún no han aprobado los tests de selección
- **Responsabilidades**:
  - Acceder a la plataforma con credenciales proporcionadas por la sede
  - Realizar tests de selección
  - Acceder a material básico de capacitación
  - Ver su propio progreso

### BECARIO
- **Descripción**: Postulantes que han aprobado los tests y cumplen los requisitos
- **Responsabilidades**:
  - Acceder a material avanzado de capacitación
  - Ver su propio progreso
  - Participar en actividades exclusivas para becarios

### Administrador de Aplicación
- **Descripción**: Personal encargado de la gestión técnica de la plataforma
- **Responsabilidades**:
  - Gestionar usuarios
  - Subir material de capacitación
  - Crear y modificar tests
  - Ver estadísticas de todos los usuarios
  - Configurar parámetros del sistema

### Administrador de Sede
- **Descripción**: Personal de la Universidad encargado del programa PROFER
- **Responsabilidades**:
  - Proporcionar acceso a los postulantes
  - Ver estadísticas de todos los usuarios
  - Tomar decisiones basadas en los resultados
  - Supervisar el proceso de selección y capacitación