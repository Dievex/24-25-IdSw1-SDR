# Diagrama de Clases

El diagrama de clases muestra la estructura estática del sistema Novus, definiendo las clases, sus atributos, operaciones y las relaciones entre ellas.

## Descripción

Este diagrama representa:

1. **Jerarquía de Usuarios**:
   - La clase base `Usuario` con atributos comunes
   - Especialización en `NO_BECARIO`, `BECARIO` y `Administrador`
   - Transición de `NO_BECARIO` a `BECARIO` mediante la aprobación de tests

2. **Recursos de Capacitación**:
   - Clase `Capacitación` que agrupa recursos formativos
   - Especialización en `Video` y `Documentación`

3. **Evaluación**:
   - Clase `Test` con sus preguntas y criterios de evaluación
   - Relación con `NO_BECARIO` para el proceso de selección

4. **Seguimiento**:
   - Clase `Estadística` para el monitoreo del progreso
   - Relaciones con usuarios y recursos para la trazabilidad

## Diagrama

![Diagrama de Clases](../../documentos/imagenes/diagrama_clases.png)

## Clases Principales

### Usuario
- **Atributos**: id, nombre, apellidos, email, contraseña
- **Operaciones**: iniciarSesion(), cerrarSesion()

### NO_BECARIO
- **Atributos**: fechaRegistro, testsRealizados
- **Operaciones**: realizarTest(), verCapacitacion()

### BECARIO
- **Atributos**: fechaConversion, nivelAcceso
- **Operaciones**: accederCapacitacionAvanzada()

### Administrador
- **Atributos**: tipo (aplicación/sede), permisos
- **Operaciones**: gestionarUsuarios(), verEstadisticas(), subirMaterial()

### Test
- **Atributos**: id, titulo, descripcion, preguntas, puntajeMinimo
- **Operaciones**: evaluar(), generarResultado()

### Capacitación
- **Atributos**: id, titulo, descripcion, fechaPublicacion
- **Operaciones**: mostrarContenido()

### Video
- **Atributos**: duracion, formato, url
- **Operaciones**: reproducir()

### Documentación
- **Atributos**: formato, tamaño, url
- **Operaciones**: descargar()

### Estadística
- **Atributos**: usuario, fecha, tipoActividad, resultado
- **Operaciones**: generarInforme(), filtrarDatos()