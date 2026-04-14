# Brechas de Información
## Sistema de Gestión de Compromisos RCA — CODELCO

| Campo | Valor |
|-------|-------|
| **Proyecto** | Gestión de Compromisos RCA |
| **Empresa** | CODELCO — Corporación Nacional del Cobre de Chile |
| **Fecha de generación** | 2026-04-14 |
| **Versión** | v001 |
| **Fuentes** | VACS-SGA-I-005 Rev.01 · VACS-SGA-P-010 Rev.02 |

---

## Clasificación de Brechas

- **[BRECHA DE INFORMACIÓN]** — Información que debería existir pero no está disponible en /input
- **[NO CONFIRMADO]** — Información mencionada pero sin evidencia suficiente para confirmarla
- **[AMBIGÜEDAD]** — Información presente pero con interpretación incierta o contradictoria

---

## 1. Brechas Documentales

| ID | Brecha | Tipo | Origen | Impacto AS-IS |
|----|--------|------|--------|---------------|
| B-01 | **Anexo A — Matriz de Carga de Compromisos Ambientales** no disponible en /input | BRECHA DE INFORMACIÓN | DOC-001 §2.4, §3.1.3, §6 | No es posible documentar la estructura de datos exacta de la matriz de compromisos |
| B-02 | **Anexo B — Matriz de Priorización** no disponible en /input | BRECHA DE INFORMACIÓN | DOC-001 §2.4, §3.1.3, §6 | No es posible documentar la metodología de priorización de compromisos |
| B-03 | **Anexo C — Matriz ICC de Incumplimientos** no disponible en /input | BRECHA DE INFORMACIÓN | DOC-001 §2.4, §3.4.8, §6 | No es posible documentar el algoritmo de cálculo del ICC |
| B-04 | **Anexo D — Matriz Planes de Acción** no disponible en /input | BRECHA DE INFORMACIÓN | DOC-001 §2.4, §3.4.9, §6 | No es posible documentar la estructura de los PDAs |
| B-05 | **VACS-SGA-I-001** (Gestión de Cuentas Plataforma) no disponible | BRECHA DE INFORMACIÓN | DOC-001 §2.4, §3.4.2 | No es posible documentar el proceso de gestión de usuarios de la plataforma |
| B-06 | **RCAs o expedientes de proyectos** concretos de CODELCO no disponibles | BRECHA DE INFORMACIÓN | Contexto general | No es posible mapear compromisos reales ni evaluar su complejidad práctica |
| B-07 | **Documentación técnica de la Plataforma Corporativa** no disponible | BRECHA DE INFORMACIÓN | DOC-001 §3.3, DOC-002 §3.1.3 | No es posible documentar la arquitectura tecnológica del sistema |

---

## 2. Información No Confirmada

| ID | Elemento | Tipo | Origen | Observación |
|----|----------|------|--------|-------------|
| NC-01 | **Nombre de la Plataforma Corporativa** de Cumplimiento Ambiental | NO CONFIRMADO | DOC-001 §3.3, DOC-002 §3.1.3 | Solo se menciona como "Plataforma Corporativa vigente" sin identificar nombre, proveedor ni versión |
| NC-02 | **Estado de implementación post-marcha blanca** (después de 31-12-2025) | NO CONFIRMADO | DOC-001 §5 | El plazo de marcha blanca venció. No hay evidencia del estado real de avance de los compromisos de implementación de PAS |
| NC-03 | **Integración entre la Plataforma y otros sistemas** de CODELCO (ERP, SAP, GIS, etc.) | NO CONFIRMADO | Ninguna fuente | No hay mención de integraciones tecnológicas |
| NC-04 | **Número total de RCAs** activas en CODELCO | NO CONFIRMADO | Ninguna fuente | No hay datos cuantitativos del universo de compromisos |
| NC-05 | **Número de compromisos** gestionados actualmente en la plataforma | NO CONFIRMADO | Ninguna fuente | Sin métricas del sistema actual |
| NC-06 | **Porcentaje de cumplimiento actual** del sistema | NO CONFIRMADO | Ninguna fuente | Sin KPIs ni reportes de cumplimiento en /input |
| NC-07 | **Herramienta de validación de verificadores** (¿integrada en plataforma o por correo?) | NO CONFIRMADO | DOC-002 §3.2.3 | El proceso de validación menciona correo electrónico y plataforma — no queda claro cuál es el canal formal primario |
| NC-08 | **Estado real del Convenio de Desempeño Único Divisional 2025** | NO CONFIRMADO | DOC-001 §3.4.10 | No hay documentación del convenio ni de sus compromisos específicos |

---

## 3. Ambigüedades Identificadas

| ID | Ambigüedad | Tipo | Origen | Observación |
|----|-----------|------|--------|-------------|
| A-01 | **¿Qué pasa si la plataforma no tiene el área responsable en su lista desplegable?** | AMBIGÜEDAD | DOC-001 §3.1.3 (Tabla 1) | El instructivo indica solicitar a DCGAO la incorporación, pero no define plazo ni proceso específico |
| A-02 | **¿Quién identifica compromisos en CdPs que no modifican una RCA cuando el proyecto es de una División?** | AMBIGÜEDAD | DOC-001 §3.1.2 | El instructivo distingue entre CM y División para EIAs pero no es explícito para este caso |
| A-03 | **Alcance del término "equivalente a futuro"** en los nombres de áreas | AMBIGÜEDAD | DOC-001 §4, DOC-002 §1.5 | Todos los roles incluyen la cláusula "(o su equivalente a futuro)". No hay mapa de equivalencias para reorganizaciones |
| A-04 | **Criterio para decidir si un compromiso es "NC" por fondo vs. forma** | AMBIGÜEDAD | DOC-002 §3.2.3 | El procedimiento menciona que puede ser NC aunque se reporte en forma y fecha si el "contenido de fondo" está desviado — sin criterio objetivo claro |
| A-05 | **Plataforma corporativa "vigente" vs. plataforma "que la DCGAO defina"** | AMBIGÜEDAD | DOC-002 §3.1.3 | Se usa ambas expresiones indistintamente, sugiriendo posible transición de plataforma [NO CONFIRMADO] |

---

## 4. Preguntas de Validación Prioritarias

Para completar el AS-IS, se deben responder con urgencia:

1. ¿Cuál es el nombre y proveedor de la Plataforma Corporativa de Cumplimiento Ambiental?
2. ¿Cuántas RCAs activas gestiona CODELCO actualmente?
3. ¿Se cumplieron los compromisos de implementación del plan de vigencia (PAS) al 31-12-2025?
4. ¿Existen integraciones entre la Plataforma y otros sistemas corporativos?
5. ¿Cuáles son los KPIs de cumplimiento actuales del sistema?
