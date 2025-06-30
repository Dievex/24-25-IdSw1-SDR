<p align="center">
  <a href="http://github.com/Dievex/24-25-IdSw1-SDR/blob/version-002/README.md">
    🏠 <strong>Inicio</strong>
  </a> •
  <a href="https://github.com/Dievex/24-25-IdSw1-SDR/blob/version-002/modelo_del_dominio/README.md">
    📦 <strong>Modelo del Dominio</strong>
  </a> •
  <a href="https://github.com/Dievex/24-25-IdSw1-SDR/blob/version-002/casos_de_uso/README.md">
    ⚙️ <strong>Casos de Uso</strong>
  </a>
</p>
# Diagrama de Clases

El diagrama de clases muestra la estructura estática del sistema Novus, definiendo las clases, sus atributos, operaciones y las relaciones entre ellas.

## Descripción

Este diagrama representa:

1. **Jerarquía de Usuarios**:
   - La clase base `Usuario` con atributos comunes
   - Especialización en `POSTULANTE`, `BECARIO`,`Administrador` y `Seleccionador`
   - Transición de `POSTULANTE` a `BECARIO` mediante la aprobación de tests

2. **Recursos de Capacitación**:
   - Clase `Capacitación` que agrupa recursos formativos
   - Especialización en `Video` y `Documentación`

3. **Evaluación**:
   - Clase `Test` con sus preguntas y criterios de evaluación
   - Relación con `POSTULANTE` para el proceso de selección

4. **Seguimiento**:
   - Clase `Estadística` para el monitoreo del progreso
   - Relaciones con usuarios y recursos para la trazabilidad

## Diagrama

![Diagrama de Clases](../../documentos/imagenes/modelo_del_dominio/clases/Diagrama_de_Clases_Novus.svg)

