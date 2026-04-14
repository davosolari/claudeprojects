# Resumen Ejecutivo — Análisis AS-IS
## Sistema de Gestión de Compromisos RCA — CODELCO

| Campo | Valor |
|-------|-------|
| **Proyecto** | Gestión de Compromisos RCA |
| **Empresa** | CODELCO — Corporación Nacional del Cobre de Chile |
| **Fecha de generación** | 2026-04-14 |
| **Versión** | v001 |
| **Elaborado por** | Agente AS-IS (tecpetrol-rca-asis-analyst adaptado a CODELCO) |
| **Fuentes analizadas** | VACS-SGA-I-005 Rev.01 · VACS-SGA-P-010 Rev.02 |
| **Nivel de confianza** | Alto (proceso) · Bajo (tecnología) · Alto (organización) |

---

## 1. Objetivo del Documento

Presentar un resumen ejecutivo del estado actual (AS-IS) del Sistema de Gestión de Compromisos de Permisos Ambientales (RCA) de CODELCO, basado exclusivamente en los documentos disponibles en la carpeta /input del proyecto.

---

## 2. Descripción General del Sistema

CODELCO opera un **Sistema de Cumplimiento Ambiental** corporativo que gestiona los compromisos, condiciones y exigencias derivados de sus **Instrumentos de Gestión Ambiental (IGA)**, principalmente:

- Resoluciones de Calificación Ambiental (RCA)
- Consultas de Pertinencia (CdP)
- Revisiones Excepcionales de RCA (artículo 25 quinquies)
- Planes de Prevención y Descontaminación Atmosférica (PPDA)
- Normas de Emisión y Calidad
- Resoluciones de la SMA y SEA

El sistema abarca **toda la Corporación**: Divisiones mineras, Vicepresidencia de Proyectos (VP) y Casa Matriz (CM).

---

## 3. Hallazgos Principales

### 3.1 Proceso de Gestión (Bien Documentado)

El proceso AS-IS está estructurado en **4 etapas secuenciales**:

| Etapa | Nombre | Actores Principales |
|-------|--------|---------------------|
| 1 | Identificación y Levantamiento de Compromisos | DCGPP, División, CM |
| 2 | Verificación del Cumplimiento | División, VP, CM |
| 3 | Gestión de Incumplimientos | División, VP, CM, DCGAO, GMA |
| 4 | Control y Seguimiento | DCGAO |

### 3.2 Sistema Tecnológico (Parcialmente Documentado)

Existe una **Plataforma Corporativa de Cumplimiento Ambiental** que centraliza la carga, seguimiento y validación de compromisos. Sin embargo, su nombre comercial, proveedor, arquitectura técnica y capacidades específicas **no están documentados** en los archivos disponibles. [NO CONFIRMADO]

### 3.3 Estructura Organizacional (Bien Documentada)

Se identificaron **8 roles organizacionales** con responsabilidades diferenciadas. La DCGAO actúa como eje central de control y validación. Existe separación explícita entre quien carga verificadores y quien los valida.

### 3.4 Instrumentos de Control de Cumplimiento

- **Estados de cumplimiento:** Cumple (C) / No Cumple (NC) / No Aplica (NA) / No Verificable (NV)
- **Tipos de cumplimiento:** Puntual / Esporádico / Periódico
- **Priorización:** Escala de 5 niveles (I al V, de menor a mayor prioridad)
- **ICC (Índice de Circunstancia Calificante):** 4 niveles — Bajo / Medio / Alto / Muy Alto
- **Planes de Acción (PDA):** Obligatorios para estado NC, con plazos diferenciados según ICC

---

## 4. Fortalezas Observadas

- Proceso completamente documentado con flujo secuencial claro
- Separación de roles entre carga y validación de verificadores (independencia operacional)
- Sistema de priorización definido (ICC + escala de 5 niveles)
- Plazos explícitos para elaboración de matrices (60 días) y planes de acción (15-60 días según ICC)
- Reportes semestrales mínimos establecidos por procedimiento

---

## 5. Brechas y Riesgos Observados

| ID | Brecha / Riesgo | Fuente | Criticidad |
|----|-----------------|--------|------------|
| B-01 | Plataforma Corporativa no especificada técnicamente | DOC-001/002 | Alta |
| B-02 | Anexos A, B, C y D del Instructivo no disponibles en /input | DOC-001 | Alta |
| B-03 | Sin documentación de RCAs o proyectos específicos de CODELCO | /input | Alta |
| B-04 | Proceso de identificación de compromisos depende de criterio experto no estandarizado | DOC-001 §3.1.2 | Media |
| B-05 | Dependencia de correo electrónico como mecanismo de validación formal | DOC-002 §3.1.2 | Media |
| B-06 | Sin definición clara del proceso de marcha blanca (hasta 31-12-2025) | DOC-001 §5 | Baja |

---

## 6. Nivel de Cobertura AS-IS

| Dimensión | Cobertura | Observación |
|-----------|-----------|-------------|
| Proceso operativo | Alta | Flujo completo documentado en DOC-001 y DOC-002 |
| Roles y responsabilidades | Alta | 8 roles identificados con funciones explícitas |
| Tecnología / Plataforma | Baja | Solo referenciada, no especificada |
| Datos y flujos de información | Muy baja | No hay documentación de arquitectura de datos |
| Proyectos RCA específicos | Nula | No hay RCAs concretas en /input |

---

## 7. Recomendaciones para Completar el AS-IS

1. Obtener documentación técnica de la Plataforma Corporativa de Cumplimiento Ambiental
2. Incorporar los Anexos A, B, C y D del Instructivo VACS-SGA-I-005
3. Agregar al menos 2-3 RCAs de proyectos reales de CODELCO para mapear compromisos concretos
4. Realizar entrevistas con DCGAO y DMAT para validar el proceso real vs. documentado
5. Verificar el estado de implementación post-marcha blanca (posterior a 31-12-2025)
