# Diagrama de Objetos

El diagrama de objetos muestra instancias concretas de las clases definidas en el diagrama de clases, ilustrando cómo se relacionan en escenarios específicos del sistema Novus.

## Descripción

Este diagrama representa:

1. **Instancias de Usuarios**:
   - Ejemplos de NO_BECARIOS en diferentes etapas del proceso
   - Ejemplos de BECARIOS que han completado el proceso
   - Administradores de la aplicación y de la sede

2. **Tests y Resultados**:
   - Tests específicos con sus características
   - Resultados de tests para diferentes usuarios
   - Transición de NO_BECARIO a BECARIO tras aprobar tests

3. **Recursos de Capacitación**:
   - Videos específicos con sus atributos
   - Documentos específicos con sus atributos
   - Relación entre usuarios y los recursos que han utilizado

4. **Estadísticas**:
   - Ejemplos de registros estadísticos
   - Trazabilidad de actividades de usuarios específicos

## Diagrama

![Diagrama de Objetos](../../documentos/imagenes/diagrama_objetos.png)

## Ejemplos de Objetos

### Usuarios
- **no_becario1**: {id: "NB001", nombre: "Ana", apellidos: "García", testsRealizados: 2}
- **no_becario2**: {id: "NB002", nombre: "Carlos", apellidos: "López", testsRealizados: 0}
- **becario1**: {id: "B001", nombre: "Elena", apellidos: "Martínez", fechaConversion: "2023-10-15"}
- **admin1**: {id: "A001", nombre: "Miguel", apellidos: "Sánchez", tipo: "aplicación"}

### Tests
- **testProgramacion**: {id: "T001", titulo: "Fundamentos de Programación", puntajeMinimo: 70}
- **testLogica**: {id: "T002", titulo: "Razonamiento Lógico", puntajeMinimo: 65}

### Capacitación
- **videoPython**: {id: "V001", titulo: "Introducción a Python", duracion: "45:30"}
- **docJava**: {id: "D001", titulo: "Manual de Java", formato: "PDF"}

### Estadísticas
- **estadistica1**: {usuario: "NB001", fecha: "2023-10-10", tipoActividad: "Test", resultado: "Aprobado"}
- **estadistica2**: {usuario: "B001", fecha: "2023-10-20", tipoActividad: "Capacitación", resultado: "Completado"}