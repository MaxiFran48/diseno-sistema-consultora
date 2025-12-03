# Sistema de Gestión para Consultora de Profesionales

## Descripción General
Repositorio de documentación para el diseño de la arquitectura de software de un sistema de gestión para una consultora. El proyecto abarca el análisis de requerimientos, el modelado del dominio y el diseño detallado de los flujos de negocio y la estructura de datos.

## Contexto del Problema (Caso de Negocio)
El sistema fue diseñado para una consultora de profesionales que necesitaba una solución integral para gestionar sus operaciones. La problemática principal incluía:

*   **Gestión de Acuerdos Comerciales:** Registrar los compromisos con clientes, especificando proyectos, tipos de servicio y horas mensuales mínimas contratadas.
*   **Administración de Consultores:** Manejar una nómina de profesionales independientes, sus especialidades y su disponibilidad.
*   **Asignación de Tareas:** Asignar servicios solicitados por los clientes al consultor más adecuado, controlando la carga horaria.
*   **Facturación Automatizada:** Generar facturas mensuales de forma automática, incluyendo cargos fijos por horas no consumidas y multas, integrándose con sistemas de recaudación externos (ARCA).

## Alcance de la Solución
Se diseñó la arquitectura completa abarcando los siguientes artefactos:

### 1. Modelado de Datos
*   **Modelo Entidad-Relación (MER):** Se diseñó la estructura de la base de datos relacional, normalizada hasta 3FN, para dar soporte a toda la operativa.

### 2. Ingeniería de Software (Proceso Unificado y UML)
*   **Diagrama de Clases:** Modela la estructura estática del sistema, incluyendo entidades como `Cliente`, `Consultor`, `Convenio`, `Servicio` y `Factura`.
*   **Flujos de Sucesos (Casos de Uso):** Se detallaron los flujos para los casos de uso críticos del sistema, entre ellos:
    *   `CU1 - Solicitar servicio`
    *   `CU2 - Aceptar convenio`
    *   `CU4 - Iniciar proceso de facturación`
    *   `CU13 - Gestionar proceso de facturación`
*   **Diagramas de Transición de Estados (DTE):** Se modeló el ciclo de vida de las entidades clave para controlar su comportamiento a lo largo del tiempo:
    *   `DTE - Convenio`
    *   `DTE - Servicio`
    *   `DTE - Proceso de Facturación`

## Tecnologías y Herramientas
*   **Modelado:** Draw.io
*   **Base de Datos (Diseño):** Orientado a motores de bases de datos relacionales (ej. PostgreSQL, MySQL).
*   **Metodología:** Proceso Unificado de Desarrollo de Software.

---
*Proyecto académico realizado para la cátedra "Diseño de Sistemas" de la UTN-FRM.*
*Equipo: Máximo Fran, Guillermina Fiore, Agustín Aguilera, Santiago Castro, Camila Bastian, Elena Moyano, Francisco Velasco, Juan Zalazar, Julián Sagues, Julián Berón, Bautista Martin, Franco Giusti, Juan Pablo Acre, Emiliano Pacin, Martín Berni y Gonzalo Gerónimo*
