# Puntos de Dolor Operacionales
## Sistema de Gestión de Compromisos RCA — CODELCO

| Campo | Valor |
|-------|-------|
| **Proyecto** | Gestión de Compromisos RCA |
| **Empresa** | CODELCO — Corporación Nacional del Cobre de Chile |
| **Fecha de generación** | 2026-04-14 |
| **Versión** | v001 |
| **Fuentes** | VACS-SGA-I-005 Rev.01 · VACS-SGA-P-010 Rev.02 |
| **Nivel de confianza** | Medio — inferido desde lenguaje normativo; requiere validación con actores |

---

> **Nota metodológica:** Los puntos de dolor que siguen son inferidos a partir de la lectura del lenguaje del proceso documentado (cláusulas de excepción, dobles validaciones, plazos escalonados, advertencias). No han sido confirmados directamente por actores del sistema. Se marcan como [INFERENCIA] cuando corresponde.

---

## PD-01 — Dependencia de una Plataforma No Documentada

**Descripción:** Todo el sistema de cumplimiento (carga de compromisos, verificadores, PDAs, estados) depende de una "Plataforma Corporativa de Cumplimiento Ambiental" que no tiene nombre ni especificación técnica en los documentos analizados.

**Evidencia:** DOC-001 §3.3, DOC-002 §3.1.3 — se menciona reiteradamente como "la plataforma vigente" o "la plataforma que la DCGAO defina".

**Riesgo:** Si la plataforma cambia, todo el proceso debe readaptarse. La ausencia de documentación técnica dificulta la auditoría y la continuidad operacional. [INFERENCIA]

---

## PD-02 — Plazos Ajustados para Elaboración de Matrices

**Descripción:** Se dispone de 60 días corridos para elaborar la Matriz de Compromisos desde la notificación del IGA. En RCAs complejas con cientos de compromisos y múltiples documentos de expediente, este plazo puede ser insuficiente.

**Evidencia:** DOC-002 §3.1.2 — *"El plazo para la elaboración de la matriz de compromisos será de hasta 60 días corridos por parte de los responsables del IGA."*

**Riesgo:** Presión de tiempo puede llevar a sistematizaciones incompletas o erróneas que comprometan el cumplimiento posterior. [INFERENCIA]

---

## PD-03 — Fragmentación de Responsabilidades en Etapa 1

**Descripción:** La responsabilidad de elaborar la Matriz de Compromisos varía según el tipo de IGA y el nivel del proyecto (División vs. VP vs. CM), generando múltiples combinaciones de actores. Esto complejiza la coordinación y aumenta el riesgo de errores por confusión de roles.

**Evidencia:** DOC-002 §3.1.2 — 3 escenarios distintos de responsabilidad de elaboración; DOC-001 §4 — 8 roles con matices de responsabilidad.

**Riesgo:** Gaps en la cobertura de compromisos si no está claro quién elabora la matriz en casos límite. [INFERENCIA]

---

## PD-04 — Dependencia del Correo Electrónico como Canal Formal

**Descripción:** Múltiples validaciones críticas del proceso se realizan "mediante correo electrónico" (validación de matrices, notificación de verificadores, aprobación de PDAs). El correo no es un sistema de gestión documental controlado.

**Evidencia:** DOC-002 §3.1.2 — *"Todas estas validaciones deberán respaldarse mediante correo electrónico, con copia a..."*; DOC-001 §3.4.6 — *"el responsable de validación recibirá un correo electrónico indicando que se encuentran disponibles los verificadores."*

**Riesgo:** Pérdida de trazabilidad, falta de trazabilidad auditable, riesgo de correos no leídos o archivados incorrectamente. [INFERENCIA]

---

## PD-05 — Identificación de Compromisos Basada en Criterio Experto

**Descripción:** El proceso de identificación de compromisos desde documentos de expediente (Adendas, ICE, EIA) requiere criterio experto para determinar si hay errores de transcripción, inconsistencias o complementos. No hay criterio objetivo automatizable.

**Evidencia:** DOC-001 §3.1.2 — *"se debe determinar si existe un error de transcripción, procediendo luego con la identificación correcta del compromiso."*

**Riesgo:** Variabilidad en la calidad de sistematización entre distintas divisiones o proyectos. Riesgo de subregistro o sobreregistro de compromisos. [INFERENCIA]

---

## PD-06 — Gestión de Compromisos Inconsistentes entre RCA y Expediente

**Descripción:** Cuando hay inconsistencias entre lo señalado en la RCA y su expediente, se debe generar un documento aparte que requiere validación legal (DCGAO/VP Legal). Este proceso no tiene un flujo documentado propio ni plazos definidos.

**Evidencia:** DOC-001 §3.1.2 — *"se deberán identificar en un documento aparte, el cual será emitido por las Divisiones, VP o CM (...) siendo validado por sus respectivas áreas legales."*

**Riesgo:** Las inconsistencias pueden quedar sin resolución formal por tiempo indefinido, creando incertidumbre sobre cuál es el compromiso real exigible. [INFERENCIA]

---

## PD-07 — Complejidad del Proceso de Validación de PDAs

**Descripción:** Los Planes de Acción para incumplimientos Muy Alto y Alto requieren validación encadenada de 4 niveles: Gerencia Responsable → GSAE → Gerente General → GMA. Este proceso puede ser lento y burocrático.

**Evidencia:** DOC-002 §3.3.2 — cuadro de plazos y validaciones: ICC Muy Alto requiere 4 validaciones en 15 días corridos.

**Riesgo:** El plazo de 15 días para elaborar y validar un PDA en 4 niveles jerárquicos es muy ajustado para incumplimientos complejos, especialmente en operaciones mineras con Gerentes Generales con alta carga. [INFERENCIA]

---

## PD-08 — Ausencia de Métricas y KPIs Visibles en la Documentación

**Descripción:** Los documentos no definen indicadores de desempeño del sistema (% de compromisos con Cumple, tasa de incumplimientos, tiempo promedio de validación, etc.), salvo el % de cumplimiento por compromiso a la fecha.

**Evidencia:** DOC-002 §4 — solo menciona reporte semestral sin especificar contenido mínimo de KPIs.

**Riesgo:** Sin KPIs claros, es difícil evaluar el desempeño del sistema de cumplimiento ni tomar decisiones de mejora basadas en datos. [INFERENCIA]

---

## PD-09 — Gestión de Cambios de Usuarios en Plataforma

**Descripción:** Cuando un usuario deja de pertenecer a CODELCO, la baja de su perfil en la Plataforma debe ser solicitada por su área a la DCGAO por correo electrónico. Este proceso manual puede generar demoras con usuarios activos que ya no son responsables.

**Evidencia:** DOC-001 §3.4.2 — *"será responsabilidad de su área indicar a la DCGAO (...) la solicitud de baja a través de correo electrónico."*

**Riesgo:** Usuarios con acceso activo a compromisos y verificadores de personas que ya no trabajan en la organización, con potencial impacto en la integridad del sistema. [INFERENCIA]

---

## Resumen de Puntos de Dolor

| ID | Punto de Dolor | Categoría | Severidad Estimada |
|----|---------------|-----------|-------------------|
| PD-01 | Plataforma no documentada | Tecnología | Alta |
| PD-02 | Plazos ajustados para matrices | Proceso | Media |
| PD-03 | Fragmentación de responsabilidades | Organización | Media |
| PD-04 | Dependencia del correo electrónico | Proceso / Tecnología | Media |
| PD-05 | Identificación por criterio experto | Proceso | Media |
| PD-06 | Inconsistencias RCA vs. expediente sin flujo | Proceso | Media |
| PD-07 | Validación multinivel de PDAs en plazos cortos | Proceso / Organización | Alta |
| PD-08 | Ausencia de KPIs visibles | Gestión | Baja |
| PD-09 | Gestión manual de bajas de usuarios | Proceso | Baja |

> **Severidad estimada basada en impacto potencial en el cumplimiento regulatorio. Requiere validación con actores del sistema.**
