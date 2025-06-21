# Diagramas de Casos de Uso Detallados

Esta carpeta contiene los diagramas de casos de uso detallados del sistema, implementados en PlantUML. Cada diagrama representa un caso de uso específico con sus flujos principales, alternativos y de excepción.

## Descripción

Los diagramas de casos de uso detallados proporcionan una vista granular de cada funcionalidad del sistema, mostrando:
- Actores involucrados
- Precondiciones y postcondiciones
- Flujo principal de eventos
- Flujos alternativos
- Manejo de excepciones

## Estructura de Archivos

### Gestión de Sesión
- `iniciar_sesion.puml` - Proceso de autenticación de usuarios
- `cerrar_sesion.puml` - Proceso de cierre de sesión

### Gestión de Postulantes
- `crear_postulante.puml` - Registro de nuevos postulantes
- `editar_postulante.puml` - Modificación de datos de postulantes
- `eliminar_postulante.puml` - Eliminación de postulantes del sistema
- `listar_postulante.puml` - Visualización de lista de postulantes

### Gestión de Capacitaciones
- `crear_capacitacion.puml` - Creación de nuevas capacitaciones
- `editar_capacitacion.puml` - Modificación de capacitaciones existentes
- `eliminar_capacitacion.puml` - Eliminación de capacitaciones
- `listar_capacitacion.puml` - Visualización de capacitaciones disponibles
- `hacer_capacitacion.puml` - Proceso de realización de capacitaciones

### Gestión de Tests
- `crear_test.puml` - Creación de nuevos tests de evaluación
- `editar_test.puml` - Modificación de tests existentes
- `eliminar_test.puml` - Eliminación de tests
- `listar_test.puml` - Visualización de tests disponibles
- `hacer_test.puml` - Proceso de realización de tests

### Consulta y Reportes
- `ver_estadisticas.puml` - Visualización de estadísticas del sistema
- `ver_progreso.puml` - Consulta del progreso de postulantes
- `ver_resultados.puml` - Visualización de resultados de evaluaciones
