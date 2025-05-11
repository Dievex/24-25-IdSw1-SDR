# Diagrama de Estados

El diagrama de estados muestra los diferentes estados por los que pasan las entidades del sistema Novus y las transiciones entre estos estados.

## Descripción

Este diagrama representa:

1. **Estados de un Postulante**:
   - Transición de NO_BECARIO a BECARIO
   - Estados intermedios durante el proceso de selección

2. **Estados de un Test**:
   - Pendiente → En Progreso → Completado → Evaluado
   - Condiciones para las transiciones entre estados

3. **Estados de Capacitación**:
   - Disponible → En Progreso → Completada
   - Seguimiento del avance en la capacitación

## Diagrama

![Diagrama de Estados](../../documentos/imagenes/diagrama_estados.png)

## Estados Principales

### Estados de Postulante
- **Registrado**: Estado inicial de un NO_BECARIO
- **En Evaluación**: Realizando tests
- **Evaluado**: Tests completados, pendiente de resultados
- **BECARIO**: Aprobado y convertido en BECARIO
- **Rechazado**: No cumple los requisitos

### Estados de Test
- **Pendiente**: Test disponible pero no iniciado
- **En Progreso**: Test siendo realizado
- **Completado**: Test finalizado
- **Evaluado**: Resultados procesados

### Estados de Capacitación
- **Disponible**: Material publicado
- **En Progreso**: Usuario accediendo al material
- **Completada**: Usuario ha finalizado el material