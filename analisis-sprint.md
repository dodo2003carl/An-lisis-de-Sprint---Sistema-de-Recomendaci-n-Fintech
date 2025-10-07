# ANÁLISIS DE SPRINT
## Homework #1: Proyecto de Recomendación

**Metodologías Ágiles en Data Science**

---

## 📋 Información del Estudiante

- **Estudiante:** DODY SALIM DUEÑAS REMACHE
- **LinkedIn:** [Ver Perfil](https://www.linkedin.com/in/dody-due%C3%b1as-079164296/)
- **Contacto:** +593 982744895
- **Asignatura:** Ciencia de Datos
- **Fecha de Entrega:** 16 de Julio de 2025

---

## 📖 Consigna

Estás trabajando como Data Scientist en una fintech y recibes un mensaje de la líder de producto sobre un proyecto en curso. El equipo está desarrollando un modelo de recomendación de productos financieros personalizados, pero surgieron algunos problemas durante el sprint actual.

**Tu tarea:** Analizar la situación, identificar errores de enfoque, aplicar conocimientos de metodologías ágiles y proponer un plan de acción iterativo.

### 📩 Situación

---

**De:** Sofia <sofia.pm@fintechlocal.com>  
**Para:** Equipo de Datos <datos@fintechlocal.com>  
**Fecha:** 04 de julio de 2025, 15:30  
**Asunto:** Revisión urgente – Proyecto de recomendación

---

> **Hola equipo,**
>
> Estamos teniendo algunas dificultades con el proyecto del sistema de recomendación de productos. Les comparto un resumen de la situación:
>
> - El modelo fue entrenado hace dos semanas, pero los datos de entrenamiento venían de un pipeline que aún no está finalizado, por lo que no estaban del todo limpios ni completos.
>
> - En la daily de hoy, varios integrantes comentaron que no tienen claridad sobre qué se espera como entregable para este sprint.
>
> - El tablero Kanban está desactualizado y hay tareas que no reflejan lo que realmente se está haciendo.
>
> - Nos dimos cuenta de que no incluimos métricas de validación del modelo en el sprint actual, y eso va a retrasar la evaluación de resultados.
>
> - En paralelo, el equipo de front ya está trabajando en el diseño del módulo donde se van a mostrar las recomendaciones, pero todavía no saben cómo va a venir la salida del modelo.
>
> ¿Podemos revisar el enfoque del sprint actual y proponer cómo reordenarnos para avanzar mejor?
>
> Gracias, –  
> *Sofia (PM)*  
> *FintechLocal*

---

---

## ❓ Pregunta 1

**Identifica al menos tres fallas en la forma en que se está llevando a cabo este sprint.**

### 🚨 Respuesta: Fallas Identificadas en el Sprint

#### 1. Fallo en la Calidad y Preparación de los Datos

**Evidencia:** 
> "El modelo fue entrenado hace dos semanas, pero los datos de entrenamiento venían de un pipeline que aún no está finalizado, por lo que no estaban del todo limpios ni completos."

**Análisis:** Error fundamental. Se inició una tarea crítica sin asegurar el principal insumo. Implica una falta de "Definition of Ready" y compromete la fiabilidad de cualquier resultado del modelo.

#### 2. Falta de Transparencia y Desactualización del Proceso

**Evidencia:** 
> "El tablero Kanban está desactualizado y hay tareas que no reflejan lo que realmente se está haciendo. En la daily de hoy, varios integrantes comentaron que no tienen claridad sobre qué se espera como entregable para este sprint."

**Análisis:** Ruptura grave en los principios de agilidad. La falta de claridad y desactualización del tablero impiden evaluar el estado real del sprint.

#### 3. Fallo en la Planificación y Gestión de Dependencias

**Evidencia:** 
> "No incluimos métricas de validación del modelo en el sprint actual. El equipo de front ya está trabajando en el diseño pero todavía no saben cómo va a venir la salida del modelo."

**Análisis:** Planificación deficiente. Faltan pasos críticos del ciclo de desarrollo y no se gestionaron dependencias entre equipos, bloqueando trabajo y garantizando retrasos.

---

## ❓ Pregunta 2

**Indica qué metodología (Scrum, Kanban, híbrida) propondrías usar y por qué.**

### ⚡ Respuesta: Metodología Propuesta

## 🎯 Kanban

Propongo migrar a **Kanban** temporalmente por las siguientes razones clave:

### 1. Manejo del Trabajo en Curso (WIP)

Visualizar el trabajo actual y limitar el WIP forzará al equipo a enfocarse en terminar tareas críticas antes de comenzar otras, mejorando el foco y el throughput.

### 2. Mayor Flexibilidad ante la Incertidumbre

Permite cambios de prioridad fluidos sin esperar al final de un sprint. El trabajo se extrae constantemente (pull system), ideal para equipos de Datos esperando la finalización de pipelines.

### 3. Foco en el Flujo de Valor

Kanban se centra en medir el tiempo de ciclo y eliminar cuellos de botella. Los bloqueos se hacen inmediatamente visibles, forzando al equipo a resolver dependencias.

### ✅ Conclusión

Mientras Scrum es excelente para proyectos con objetivos estables, Kanban ofrece la disciplina de flujo y flexibilidad necesarias para limpiar el desorden, resolver dependencias y entregar valor de forma predecible.

---

## ❓ Pregunta 3

**Propón una nueva secuencia de trabajo para el próximo sprint, incluyendo tareas, entregables clave para el perfil de ciencia de datos y menciona al menos una herramienta colaborativa (por ejemplo, GitHub Projects, Jira, Trello) que apoye la adopción de esa metodología en un equipo distribuido.**

### 🔄 Respuesta: Secuencia de Trabajo Propuesta

| Secuencia | Tarea de Flujo | Descripción y Objetivo |
|-----------|----------------|------------------------|
| **1** | Asegurar la Calidad del Dato | **[PRIORIDAD MÁXIMA]** Finalizar el pipeline ETL y ejecutar rutinas de validación de limpieza para los datos de entrenamiento. |
| **2** | Definir Contrato de Integración | Sesión de pairing (Datos + Frontend) para formalizar la especificación de la API/Payload. Documentar el formato de salida del modelo. |
| **3** | Integrar Métricas de Validación | Implementar métricas de performance (Precision, Recall, F1-Score) dentro del código de entrenamiento y evaluación. |
| **4** | Re-entrenamiento y Evaluación | Re-ejecutar el entrenamiento del modelo usando los datos limpios y el código de evaluación mejorado. |
| **5** | Entrega a Frontend | Proporcionar la salida de prueba del modelo en el formato acordado para que Frontend complete su integración. |
| **6** | Análisis y Documentación Final | Analizar el rendimiento del modelo y generar el informe de resultados. |

### 📦 Entregables Clave (Data Science)

- Pipeline de Datos Finalizado y Código de Limpieza Validado
- Modelo Entrenado y Persistido (pickle o saved model)
- Código de Evaluación con Métricas implementadas
- Especificación Formal del Payload (JSON schema)

### 🛠️ Herramienta Colaborativa: Jira Software

| Ventaja para Kanban | Cómo Resuelve las Fallas Actuales |
|---------------------|-----------------------------------|
| Tablero Kanban con Flujo Personalizado | Permite definir columnas precisas (Bloqueado, Rework, QA) y limitar el WIP, forzando al equipo a enfocarse en terminar tareas. |
| Gestión de Dependencias | Permite vincular tareas entre equipos. Los bloqueos son transparentes para el PM. |
| Transparencia y Actualización | Requiere estados claros. Se convierte en la única fuente de verdad para el Daily Stand-up. |
| Documentación Integrada | Entregables y documentación clave pueden adjuntarse directamente a las tareas. |

---

## ❓ Pregunta 4

**Señala en qué fases del ciclo de vida de los datos (generación, preparación, modelado, evaluación, etc.) están ocurriendo los principales problemas.**

### 🔍 Respuesta: Fases del Ciclo de Vida con Problemas

### Fase 1: Preparación / Limpieza de Datos

**Problema:** Pipeline no finalizado resultando en datos sucios e incompletos.

**Impacto:** Fallo fundamental que compromete la validez del modelo desde su origen. Es la causa raíz del potencial rework.

### Fase 2: Modelado y Evaluación

**Problema:** No se incluyeron métricas de validación en el sprint.

**Impacto:** La fase de Evaluación fue omitida, paralizando la capacidad de determinar si el modelo está listo para producción.

### Fase 3: Despliegue / Integración

**Problema:** Frontend no sabe cómo va a venir la salida del modelo.

**Impacto:** Falta de "Contrato de Servicio" bloquea la integración. Frontend no puede consumir la recomendación sin conocer su formato.

---

## ⭐ Extra Credits

**Propón al menos una práctica de mejora continua que podría implementarse en el equipo para evitar estos errores en el futuro.**

### Respuesta: Práctica de Mejora Continua

## ✅ Definition of Ready (DoR)

Se aplica **antes** de que una tarea pase a "Haciendo":

| Tarea | Criterios Mínimos de LISTO | Falla que Previene |
|-------|----------------------------|-------------------|
| Entrenar Modelo | • Pipeline ETL terminado y validado<br>• Muestra de datos aprobada<br>• Métricas de Validación listas | Datos sucios o incompletos |
| Diseño Frontend | • Contrato de Salida documentado<br>• Acciones ante errores acordadas | Bloqueo por falta de formato |

## ✅ Definition of Done (DoD)

Se aplica **antes** de que una tarea pase a "Terminado":

| Tarea | Criterios Mínimos de HECHO | Falla que Previene |
|-------|----------------------------|-------------------|
| Entrenar y Persistir Modelo | • Métricas ejecutadas y documentadas<br>• Código mergeado a master<br>• Resultados revisados por PM y equipo | Omisión de métricas o resultados no validados |
| Integración con Frontend | • Salida real probada con Frontend<br>• Documentación del payload actualizada | Problemas de integración o falta de claridad |

## 🔄 Retrospectivas Regulares

- **Frecuencia:** Cada dos semanas o al finalizar un ciclo importante
- **Objetivo:** Discutir qué salió mal, por qué, y generar acciones de mejora concretas
- **Resultado:** Cultura de responsabilidad compartida y mejora continua

---

## 🤖 Pregunta Extra: Técnica de ML

**Identifica qué tipo de técnica (ML, DL, recomendación basada en contenido, etc.) sería más adecuada para este caso.**

### Respuesta: Técnica de ML Recomendada

## Filtrado Colaborativo (Collaborative Filtering)

**¿Por qué?**

- Efectividad comprobada como estándar de oro en recomendación
- No requiere datos de contenido ricos, solo matriz de interacciones
- Capacidad de descubrimiento (serendipity)

**Implementación Sugerida:**

- **User-Based CF:** Recomienda productos que a usuarios similares les gustaron
- **Item-Based CF:** Recomienda productos similares a los ya vistos (más escalable)

**Evolución futura:** Migrar a Sistema Híbrido (CF + Contenido) o Deep Learning (Autoencoders, Redes Neuronales Factoriales) para mayor precisión.

---

## 📄 Fin del Documento

*Análisis de Sprint - Metodologías Ágiles en Data Science*