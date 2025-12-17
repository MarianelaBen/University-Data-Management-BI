# University Data Management & BI Analytics

Este proyecto consiste en la modernización y migración de un sistema de gestión de cursos universitarios, transitando desde un modelo desnormalizado hacia una arquitectura relacional robusta y una capa de Inteligencia de Negocios (BI).

## Alcance del Proyecto
El sistema permite gestionar el ciclo de vida académico: inscripciones de alumnos, cursadas, exámenes finales, pagos de cuotas y encuestas de satisfacción.

## Tecnologías Utilizadas
* **Motor:** Microsoft SQL Server 2022.
* **Lenguaje:** T-SQL (Stored Procedures, Triggers, Views, Functions).

## Arquitectura de Datos
1. **Modelo Transaccional (OLTP):** Diseño normalizado a partir de una tabla maestra, garantizando integridad referencial y eficiencia en la carga de datos.
2. **Modelo de BI (OLAP):** Implementación de un modelo dimensional (Hechos y Dimensiones) para el análisis de indicadores de gestión (KPIs).

## Indicadores de Gestión (BI)
El modelo permite responder consultas críticas como:
* Tasa de rechazo de inscripciones por sede.
* Promedio de notas de finales según rango etario y categoría de curso.
* Índice de satisfacción anual por sede y profesor.
* Análisis de morosidad financiera mensual.

## Proceso de Migración
La migración se realizó íntegramente mediante **Stored Procedures**, procesando datos complejos de una tabla maestra para poblar el nuevo modelo cumpliendo con estándares de normalización.
