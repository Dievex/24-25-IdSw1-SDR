# Modelo del Dominio

El modelo del dominio representa las entidades principales del sistema Novus y sus relaciones.

## Entidades Principales

- **Usuario**: Clase base para todos los usuarios del sistema
- **NO_BECARIO**: Postulantes que aún no han aprobado los tests
- **BECARIO**: Postulantes que han aprobado los tests y cumplen los requisitos
- **Administrador**: Gestores del sistema (de la aplicación y de la sede)
- **Test**: Pruebas que deben superar los NO_BECARIOS
- **Capacitación**: Recursos formativos disponibles en la plataforma
- **Video**: Material audiovisual para la capacitación
- **Documentación**: Material escrito para la capacitación
- **Estadística**: Datos de progreso y trazabilidad de los usuarios

## Diagramas

- [Diagrama de Clases](diagramas_de_clases/README.md): Muestra la estructura estática del sistema
- [Diagrama de Objetos](diagramas_de_objetos/README.md): Presenta ejemplos concretos de instancias
- [Diagrama de Estados](diagramas_de_estados/README.md): Ilustra los cambios de estado de las entidades