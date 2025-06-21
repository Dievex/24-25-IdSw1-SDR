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

## Convenciones de Nomenclatura

Los archivos siguen la convención:
- `[accion]_[entidad].puml`
- Donde `accion` puede ser: crear, editar, eliminar, listar, hacer, ver
- Y `entidad` puede ser: postulante, capacitacion, test, sesion, estadisticas, progreso, resultados

## Cómo Visualizar los Diagramas

Para visualizar estos diagramas PlantUML:

1. **Online**: Usar [PlantUML Online Server](http://www.plantuml.com/plantuml/uml/)
2. **VS Code**: Instalar la extensión "PlantUML"
3. **IntelliJ IDEA**: Instalar el plugin "PlantUML integration"
4. **Línea de comandos**: Instalar PlantUML y usar `java -jar plantuml.jar archivo.puml`

## Relación con Otros Diagramas

Estos diagramas detallados complementan:
- Los diagramas de casos de uso generales (carpeta `../diagramas_casos_de_uso/`)
- Los diagramas de contexto (carpeta `../diagramas_de_contexto/`)
- Los actores del sistema (carpeta `../actores/`)

## Notas de Implementación

- Todos los diagramas están en formato PlantUML (.puml)
- Siguen las convenciones UML estándar
- Incluyen validaciones y manejo de errores
- Consideran diferentes roles de usuario (Administrador, Seleccionador, Postulante, Becario)

---

*Estos diagramas forman parte del análisis y diseño del sistema de gestión de postulantes y capacitaciones.*