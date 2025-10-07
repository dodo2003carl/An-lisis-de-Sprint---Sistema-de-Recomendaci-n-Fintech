# 📊 Análisis de Sprint - Sistema de Recomendación Fintech

## 🎯 Descripción del Proyecto

Este repositorio contiene el análisis completo de un sprint problemático en un proyecto de Data Science para una fintech, enfocado en el desarrollo de un **sistema de recomendación de productos financieros personalizados**.

El trabajo incluye:
- Identificación de fallas críticas en la gestión del sprint
- Propuesta de metodología ágil (Kanban vs Scrum)
- Plan de acción iterativo para resolver problemas
- Análisis del ciclo de vida de los datos
- Prácticas de mejora continua (DoR/DoD)

## 📁 Estructura del Repositorio

```
sprint-analysis-fintech/
│
├── README.md                                    # Este archivo - Descripción general del proyecto
│
├── analisis-sprint.md                           # 📄 Análisis completo en formato Markdown
│                                                # Incluye todas las respuestas y propuestas
│
├── styled_homework_pdf.html                     # 🎨 Versión HTML estilizada del análisis
│                                                # Lista para imprimir/exportar a PDF
│
└── assets/                                      # 📂 Recursos visuales
    └── email-situacion.png                      # 📧 Captura del email de la PM```

## 🚨 Contexto del Problema

El equipo de Data Science enfrentó múltiples problemas durante un sprint:

1. **Datos sucios e incompletos**: Modelo entrenado con pipeline no finalizado
2. **Falta de transparencia**: Tablero Kanban desactualizado
3. **Métricas omitidas**: Sin validación del modelo en el sprint
4. **Dependencias mal gestionadas**: Frontend sin información sobre la salida del modelo
5. **Falta de claridad**: Equipo sin conocer los entregables esperados

## 🔍 Análisis Realizado

### 1. Identificación de Fallas
- ✅ Fallo en la calidad y preparación de datos
- ✅ Falta de transparencia y desactualización del proceso
- ✅ Fallo en la planificación y gestión de dependencias

### 2. Propuesta de Metodología
**Kanban** como solución temporal para:
- Visualizar y limitar el Work In Progress (WIP)
- Mayor flexibilidad ante la incertidumbre
- Foco en el flujo de valor y eliminación de cuellos de botella

### 3. Secuencia de Trabajo Propuesta

| Fase | Tarea | Prioridad |
|------|-------|-----------|
| 1 | Asegurar calidad del dato | 🔴 CRÍTICA |
| 2 | Definir contrato de integración | 🟡 ALTA |
| 3 | Integrar métricas de validación | 🟡 ALTA |
| 4 | Re-entrenamiento y evaluación | 🟢 MEDIA |
| 5 | Entrega a Frontend | 🟢 MEDIA |
| 6 | Análisis y documentación final | 🟢 MEDIA |

### 4. Fases del Ciclo de Vida Afectadas
- **Preparación/Limpieza**: Pipeline incompleto
- **Modelado/Evaluación**: Métricas omitidas
- **Despliegue/Integración**: Falta de contrato de servicio

## 🛠️ Herramientas Recomendadas

- **Jira Software**: Gestión de flujo Kanban con WIP limits
- **GitHub Projects**: Alternativa para equipos pequeños
- **Confluence/Notion**: Documentación colaborativa
- **MLflow**: Tracking de experimentos y métricas

## 📦 Entregables Clave

- [x] Pipeline de datos validado
- [x] Modelo persistido (pickle/saved_model)
- [x] Código de evaluación con métricas
- [x] Especificación formal del payload (JSON schema)
- [x] Documentación técnica

## ✨ Prácticas de Mejora Continua

### Definition of Ready (DoR)
Criterios antes de mover una tarea a "En Progreso":
- Pipeline ETL terminado y validado
- Datos de muestra aprobados
- Métricas de validación definidas
- Contrato de salida documentado

### Definition of Done (DoD)
Criterios antes de marcar una tarea como "Terminada":
- Métricas ejecutadas y documentadas
- Código mergeado a master
- Resultados revisados por PM
- Integración probada con otros equipos

### Retrospectivas Regulares
- Frecuencia: Quincenal o fin de ciclo
- Objetivo: Identificar mejoras y acciones concretas
- Resultado: Cultura de mejora continua

## 🤖 Técnica de ML Recomendada

**Filtrado Colaborativo (Collaborative Filtering)**

**Ventajas:**
- Estándar de oro en sistemas de recomendación
- No requiere datos de contenido ricos
- Capacidad de descubrimiento (serendipity)

**Implementación:**
- User-Based CF: Recomienda productos según usuarios similares
- Item-Based CF: Recomienda productos similares (más escalable)

**Evolución futura:**
- Sistema Híbrido (CF + Content-Based)
- Deep Learning (Autoencoders, Neural Collaborative Filtering)

## 👨‍💻 Autor

**Dody Salim Dueñas Remache**

- 📧 Email: [Contacto disponible]
- 💼 LinkedIn: [linkedin.com/in/dody-dueñas-079164296](https://www.linkedin.com/in/dody-dueñas-079164296/)
- 📱 Teléfono: +593 982744895

## 📚 Contexto Académico

- **Asignatura:** Metodologías Ágiles en Data Science
- **Institución:** [Tu Universidad/Institución]
- **Fecha:** Julio 2025
- **Tipo:** Homework #1 - Análisis de Sprint

## 📄 Licencia

Este proyecto es parte de un trabajo académico.

---

## 🚀 Cómo Usar Este Repositorio

1. **Revisar el análisis completo**: Lee `analisis-sprint.md`
2. **Estudiar la metodología**: Consulta `docs/metodologia-propuesta.md`
3. **Aplicar las prácticas**: Implementa DoR/DoD en tu equipo
4. **Adaptar a tu contexto**: Personaliza las recomendaciones según tu proyecto

---

## 📌 Keywords

`#DataScience` `#AgileMethodologies` `#Kanban` `#Scrum` `#MachineLearning` `#RecommendationSystems` `#SprintAnalysis` `#Fintech` `#MLOps` `#ProjectManagement`

---

> **Nota**: Este análisis demuestra la aplicación práctica de metodologías ágiles en proyectos de ciencia de datos, identificando problemas reales y proponiendo soluciones concretas y accionables.

⭐ Si este análisis te resultó útil, ¡dale una estrella al repositorio!
