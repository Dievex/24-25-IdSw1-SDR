# Diagramas de Casos de Uso

Los diagramas de casos de uso muestran las interacciones entre los actores y el sistema Novus, representando las funcionalidades desde la perspectiva del usuario.

## Descripción

Estos diagramas representan:

1. **Gestión de Acceso**:
   - Casos de uso relacionados con la autenticación y el acceso al sistema

2. **Proceso de Selección**:
   - Casos de uso para la realización y evaluación de tests

3. **Capacitación**:
   - Casos de uso para el acceso y seguimiento de material formativo

4. **Administración**:
   - Casos de uso para la gestión del sistema y visualización de estadísticas

## Diagrama General

![Diagrama General de Casos de Uso](../../documentos/imagenes/diagrama_casos_uso_general.png)

## Diagramas Específicos

### Gestión de Acceso
![Diagrama de Casos de Uso - Acceso](../../documentos/imagenes/diagrama_casos_uso_acceso.png)

### Proceso de Selección
![Diagrama de Casos de Uso - Selección](../../documentos/imagenes/diagrama_casos_uso_seleccion.png)

### Capacitación
![Diagrama de Casos de Uso - Capacitación](../../documentos/imagenes/diagrama_casos_uso_capacitacion.png)

### Administración
![Diagrama de Casos de Uso - Administración](../../documentos/imagenes/diagrama_casos_uso_administracion.png)

## Casos de Uso Principales

### CU-01: Iniciar Sesión
- **Actores**: NO_BECARIO, BECARIO, Administrador
- **Descripción**: El usuario accede al sistema con sus credenciales
- **Flujo Principal**:
  1. El usuario introduce sus credenciales
  2. El sistema valida las credenciales
  3. El sistema muestra la interfaz correspondiente al tipo de usuario

### CU-02: Realizar Test
- **Actores**: NO_BECARIO
- **Descripción**: El NO_BECARIO realiza un test de selección
- **Flujo Principal**:
  1. El NO_BECARIO selecciona un test disponible
  2. El sistema muestra las preguntas
  3. El NO_BECARIO responde las preguntas
  4. El sistema evalúa las respuestas
  5. El sistema muestra el resultado

### CU-03: Convertir a BECARIO
- **Actores**: Sistema
- **Descripción**: El sistema convierte a un NO_BECARIO en BECARIO
- **Flujo Principal**:
  1. El sistema verifica que el NO_BECARIO ha aprobado todos los tests requeridos
  2. El sistema actualiza el estado del usuario a BECARIO
  3. El sistema notifica al usuario y a los administradores

### CU-04: Acceder a Capacitación
- **Actores**: NO_BECARIO, BECARIO
- **Descripción**: El usuario accede al material de capacitación
- **Flujo Principal**:
  1. El usuario selecciona un recurso de capacitación
  2. El sistema verifica los permisos del usuario
  3. El sistema muestra el recurso
  4. El sistema registra la actividad

### CU-05: Ver Estadísticas
- **Actores**: Administrador
- **Descripción**: El administrador visualiza estadísticas del sistema
- **Flujo Principal**:
  1. El administrador selecciona el tipo de estadísticas
  2. El sistema procesa los datos
  3. El sistema muestra las estadísticas solicitadas