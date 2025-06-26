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

# Casos de Uso

## Actores del Sistema

Los actores son entidades externas que interactúan con el sistema Novus. Pueden ser personas, otros sistemas o dispositivos.

### Descripción

Este documento define los actores principales del sistema Novus y sus características:

### Diagrama

![Diagrama de Actores](../../documentos/imagenes/actores/Actores.svg)

#### Explicación del Diagrama

El diagrama muestra los cuatro actores principales que interactúan con el Sistema Novus:

1. **POSTULANTE**: Postulantes en proceso de selección  
2. **BECARIO**: Postulantes ya seleccionados  
3. **Administrador de Aplicación**: Gestores técnicos del sistema  
4. **Seleccionador**: Supervisores del programa que recomienda estudiantes para el programa PROFER  

Cada actor tiene un rol específico y diferentes niveles de acceso al sistema, como se detalla a continuación.

### Actores Principales

#### POSTULANTE
- **Descripción**: Postulantes que aún no han aprobado los tests de selección
- **Responsabilidades**:
  - Acceder a la plataforma con credenciales proporcionadas por la sede
  - Realizar tests de selección
  - Acceder a material básico de capacitación
  - Ver su propio progreso

#### BECARIO
- **Descripción**: Postulantes que han aprobado los tests y cumplen los requisitos
- **Responsabilidades**:
  - Acceder a material avanzado de capacitación
  - Ver su propio progreso

#### Administrador de Aplicación
- **Descripción**: Personal encargado de la gestión técnica de la plataforma
- **Responsabilidades**:
  - Gestionar usuarios
  - Subir material de capacitación
  - Crear y modificar tests
  - Ver estadísticas de todos los usuarios

#### Seleccionador
- **Descripción**: Personal de FUNIBER que recomienda estudiantes para el programa PROFER
- **Responsabilidades**:
  - Ver estadísticas de todos los usuarios
  - Tomar decisiones basadas en los resultados
  - Supervisar el proceso de selección y capacitación

---

# Diagramas de Casos de Uso

Esta carpeta contiene los diagramas de casos de uso del sistema, organizados por funcionalidades principales. Todos los diagramas están implementados en PlantUML (.puml) y representan las interacciones entre los diferentes actores del sistema y las funcionalidades disponibles.

## Actores del Sistema

Los siguientes actores participan en los casos de uso:

- **Usuario**: Actor base del cual heredan los demás actores
- **Administrador**: Gestiona el sistema completo (usuarios, capacitaciones, tests)
- **Seleccionador**: Consulta información y ve los postulantes
- **Postulante**: Realiza tests y capacitaciones
- **Becario**: Realiza capacitaciones y consulta su progreso

## Diagramas Disponibles

### 1. Gestión de Sesiones
**Archivo**: `manejo_sesion.puml`  
**Descripción**: Define los casos de uso relacionados con la autenticación y manejo de sesiones de usuario.

**Casos de uso incluidos**:
- Iniciar Sesión
- Cerrar Sesión

**Actores involucrados**: Todos los actores del sistema (Usuario base)

![Gestión de Sesiones](../../documentos/imagenes/casos_de_uso/diagrams_casos_de_uso/manejo_sesion.svg)

---

### 2. CRUD de Postulantes
**Archivo**: `crud_postulante.puml`  
**Descripción**: Gestión completa de postulantes en el sistema.

**Casos de uso incluidos**:
- Crear Postulante
- Listar Postulante
- Editar Postulante
- Eliminar Postulante

**Actores involucrados**:
- **Administrador**: Acceso completo (CRUD)
- **Seleccionador**: Solo consulta (Listar)

![CRUD de Postulantes](../../documentos/imagenes/casos_de_uso/diagrams_casos_de_uso/crud_postulante.svg)

---

### 3. CRUD de Capacitaciones
**Archivo**: `crud_capacitacion.puml`  
**Descripción**: Administración de capacitaciones disponibles en el sistema.

**Casos de uso incluidos**:
- Crear Capacitación
- Listar Capacitación
- Editar Capacitación
- Eliminar Capacitación

**Actores involucrados**:
- **Administrador**: Acceso completo (CRUD)
- **Becario**: Solo consulta (Listar)
- **Postulante**: Solo consulta (Listar)

![CRUD de Capacitaciones](../../documentos/imagenes/casos_de_uso/diagrams_casos_de_uso/crud_capacitacion.svg)

---

### 4. CRUD de Tests
**Archivo**: `crud_test.puml`  
**Descripción**: Gestión de tests y evaluaciones del sistema.

**Casos de uso incluidos**:
- Crear Test
- Listar Test
- Editar Test
- Eliminar Test

**Actores involucrados**:
- **Administrador**: Acceso completo (CRUD)
- **Postulante**: Solo consulta (Listar)

![CRUD de Test](../../documentos/imagenes/casos_de_uso/diagrams_casos_de_uso/crud_test.svg)

---

### 5. Gestión de Capacitaciones
**Archivo**: `gestion_capacitacion.puml`  
**Descripción**: Funcionalidades para realizar y seguir el progreso de capacitaciones.

**Casos de uso incluidos**:
- Hacer Capacitación
- Ver Progreso

**Actores involucrados**:
- **Postulante** y **Becario**

![Gestión de capacitaciones](../../documentos/imagenes/casos_de_uso/diagrams_casos_de_uso/gestion_capacitacion.svg)

---

### 6. Gestión de Tests
**Archivo**: `gestion_test.puml`  
**Descripción**: Funcionalidades para realizar tests y consultar resultados.

**Casos de uso incluidos**:
- Hacer Test
- Ver Resultado

**Actores involucrados**:
- **Postulante**

![Gestión Test](../../documentos/imagenes/casos_de_uso/diagrams_casos_de_uso/gestion_test.svg)

---

### 7. Consulta de Estadísticas
**Archivo**: `consultar_estadisticas.puml`  
**Descripción**: Funcionalidades para consultar estadísticas del sistema.

**Casos de uso incluidos**:
- Ver Estadísticas

**Actores involucrados**:
- **Administrador**
- **Seleccionador**

![Consulta Estadisticas](../../documentos/imagenes/casos_de_uso/diagrams_casos_de_uso/consultar_estadisticas.svg)

---

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

#### Iniciar Sesión  
![Iniciar Sesión](documentos/imagenes/casos_de_uso/diagramas_casos_de_uso_detallados/iniciar_sesion.svg)

#### Cerrar Sesión  
![Cerrar Sesión](documentos/imagenes/casos_de_uso/diagramas_casos_de_uso_detallados/cerrar_sesion.svg)

### Gestión de Postulantes

#### Crear Postulante  
![Crear Postulante](documentos/imagenes/casos_de_uso/diagramas_casos_de_uso_detallados/crear_postulante.svg)

#### Editar Postulante  
![Editar Postulante](documentos/imagenes/casos_de_uso/diagramas_casos_de_uso_detallados/editar_postulante.svg)

#### Eliminar Postulante  
![Eliminar Postulante](documentos/imagenes/casos_de_uso/diagramas_casos_de_uso_detallados/eliminar_postulante.svg)

#### Listar Postulante  
![Listar Postulante](documentos/imagenes/casos_de_uso/diagramas_casos_de_uso_detallados/listar_postulante.svg)

### Gestión de Capacitaciones

#### Crear Capacitación  
![Crear Capacitación](documentos/imagenes/casos_de_uso/diagramas_casos_de_uso_detallados/crear_capacitacion.svg)

#### Editar Capacitación  
![Editar Capacitación](documentos/imagenes/casos_de_uso/diagramas_casos_de_uso_detallados/editar_capacitacion.svg)

#### Eliminar Capacitación  
![Eliminar Capacitación](documentos/imagenes/casos_de_uso/diagramas_casos_de_uso_detallados/eliminar_capacitacion.svg)

#### Listar Capacitación  
![Listar Capacitación](documentos/imagenes/casos_de_uso/diagramas_casos_de_uso_detallados/listar_capacitacion.svg)

#### Hacer Capacitación  
![Hacer Capacitación](documentos/imagenes/casos_de_uso/diagramas_casos_de_uso_detallados/hacer_capacitacion.svg)

### Gestión de Tests

#### Crear Test  
![Crear Test](documentos/imagenes/casos_de_uso/diagramas_casos_de_uso_detallados/crear_test.svg)

#### Editar Test  
![Editar Test](documentos/imagenes/casos_de_uso/diagramas_casos_de_uso_detallados/editar_test.svg)

#### Eliminar Test  
![Eliminar Test](documentos/imagenes/casos_de_uso/diagramas_casos_de_uso_detallados/eliminar_test.svg)

#### Listar Test  
![Listar Test](documentos/imagenes/casos_de_uso/diagramas_casos_de_uso_detallados/listar_test.svg)

#### Hacer Test  
![Hacer Test](documentos/imagenes/casos_de_uso/diagramas_casos_de_uso_detallados/hacer_test.svg)

### Consulta y Reportes

#### Ver Estadísticas  
![Ver Estadísticas](documentos/imagenes/casos_de_uso/diagramas_casos_de_uso_detallados/ver_estadisticas.svg)

#### Ver Progreso  
![Ver Progreso](documentos/imagenes/casos_de_uso/diagramas_casos_de_uso_detallados/ver_progreso.svg)

#### Ver Resultados  
![Ver Resultados](documentos/imagenes/casos_de_uso/diagramas_casos_de_uso_detallados/ver_resultados.svg)

---

# Diagramas de contexto

### Seleccionador

|![Diagrama de Contexto](/documentos/imagenes/casos_de_uso/diagramas_contexto/diagrama_contexto_seleccionador.svg)|[Código](/casos_de_uso/diagramas_de_contexto/diagrama_contexto_seleccionador.puml)|
|---|---|

### Administrador

#### Diagrama General
|![Diagrama de Contexto](/documentos/imagenes/casos_de_uso/diagramas_contexto/diagrama_contexto_administrador.svg)|[Código](/casos_de_uso/diagramas_de_contexto/diagrama_contexto_administrador.puml)|
|---|---|

#### Gestión de Usuarios
|![Diagrama de Contexto Usuarios](/documentos/imagenes/casos_de_uso/diagramas_contexto/diagrama_contexto_administrador_usuarios.svg)|[Código](/casos_de_uso/diagramas_de_contexto/diagrama_contexto_administrador_usuarios.puml)|
|---|---|

#### Gestión de Tests
|![Diagrama de Contexto Tests](/documentos/imagenes/casos_de_uso/diagramas_contexto/diagrama_contexto_administrador_tests.svg)|[Código](/casos_de_uso/diagramas_de_contexto/diagrama_contexto_administrador_tests.puml)|
|---|---|

#### Gestión de Capacitaciones y Estadísticas
|![Diagrama de Contexto Capacitaciones](/documentos/imagenes/casos_de_uso/diagramas_contexto/diagrama_contexto_administrador_capacitaciones.svg)|[Código](/casos_de_uso/diagramas_de_contexto/diagrama_contexto_administrador_capacitaciones.puml)|
|---|---|

### Usuario

|![Diagrama de Contexto](/documentos/imagenes/casos_de_uso/diagramas_contexto/diagrama_contexto_postulante.svg)|[Código](/casos_de_uso/diagramas_de_contexto/diagrama_contexto_postulante.puml)|
|---|---|
