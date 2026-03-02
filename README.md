-    # Proyecto_1_Corte
# Diseño y Aplicación de un Modelo de Ciclo de Vida del Software (SDLC)

**Programa:** Ingeniería de Sistemas  
**Asignatura:** Procesos De Software 
**Caso Base:** Sector Salud (Sistemas de Información Clínica)

---

## 1. Introducción
El **Ciclo de Vida del Software (SDLC)** El Ciclo de Vida del Software (SDLC) comprende el conjunto de procesos mediante los cuales se concibe, desarrolla,
implementa y mantiene un sistema de información.Existen múltiples enfoques como Cascada, Incremental, Prototipado, Iterativo, Modelo en V, Espiral, Unified Process,
metodologías ágiles como Scrum y XP, además de marcos normativos como IEEE 1074.

En el contexto de la salud, donde la integridad de los datos y la disponibilidad del sistema son críticas,
la elección del modelo no es solo una decisión técnica, sino una **decisión mas estratégica** que impacta directamente en la seguridad del paciente y el cumplimiento normativo.

---

## 2. Análisis Comparativo de Modelos

### 2.1. Modelo en Cascada (Waterfall)
* **Descripción:** Enfoque lineal y secuencial donde cada fase debe completarse antes de iniciar la siguiente.
* **Ventajas:** Estructura clara y documentación exhaustiva.
* **Debilidades:** Alta resistencia al cambio y costo de corrección exponencial.
* **Proyectos adecuados:** Sistemas con requisitos críticos, fijos y bien comprendidos.

### 2.2. Modelo Incremental
* **Descripción:** El software se divide en partes funcionales llamadas "incrementos".
* **Ventajas:** Entrega temprana de valor y reducción del impacto de fallos modulares.
* **Debilidades:** Requiere una arquitectura inicial muy sólida.
* **Proyectos adecuados:** Sistemas modulares donde el *time-to-market* es vital.

### 2.3. Modelo de Prototipado
* **Descripción:** Construcción de versiones preliminares para validar requisitos con el usuario.
* **Ventajas:** Reduce la brecha de comunicación y asegura el cumplimiento de expectativas.
* **Debilidades:** Riesgo de omitir estándares de calidad por la rapidez.
* **Proyectos adecuados:** Sistemas con interfaces complejas o requisitos vagos.

### 2.4. Modelo Iterativo
* **Descripción:** El desarrollo se organiza en ciclos repetitivos donde el producto se refina y expande.
* **Ventajas:** Gestión de riesgos temprana y alta adaptabilidad.
* **Debilidades:** Complejidad en la gestión de la configuración.
* **Proyectos adecuados:** Sistemas complejos con alta incertidumbre técnica.

### Matriz Comparativa Técnica

| Criterio | Cascada | Incremental | Prototipado | Iterativo |
| :--- | :--- | :--- | :--- | :--- |
| **Flexibilidad** | Muy Baja | Media | Alta | Muy Alta |
| **Gestión de Riesgos** | Tardía | Moderada | Temprana | Continua |
| **Documentación** | Exhaustiva | Moderada | Baja | Dinámica |
| **Participación Usuario** | Mínima | Regular | Máxima | Alta |
| **Time-to-market** | Largo | Medio | Muy Rápido | Medio |
| **Complejidad** | Baja | Media | Media | Alta |

---

## 3. Selección y Justificación

* **Caso Base:** Sistema de Historia Clínica Electrónica (HCE).
* **Modelo Seleccionado:** **Modelo Iterativo**.

### Justificación Técnica
1.  **Incertidumbre Normativa:** Permite adaptar el sistema a nuevas leyes de protección de datos (GDPR/Locales) sin comprometer la base.
2.  **Gestión de Riesgos Críticos:** Posibilita ciclos de pruebas de seguridad constantes, vitales para datos de salud.
3.  **Contexto Organizacional:** Facilita que el personal médico valide flujos de trabajo  en situaciones reales antes del despliegue final.

---

## 4. Diseño del Modelo Aplicado

### 4.1. Fases e Integración
* **Iteración 0 (Inicio):** Arquitectura de seguridad y gobernanza de datos.
* **Iteración 1 (Identidad):** Registro de pacientes y autenticación segura.
* **Iteración 2 (Gestión Médica):** Evolución clínica, triaje y prescripción.
* **Iteración 3 (Interoperabilidad):** Integración con laboratorios (Estándares HL7/FHIR).

### 4.2. Entregables y Artefactos
* **Planificación:** Especificación de Requisitos de Software (SRS).
* **Diseño:** Documento de Arquitectura (SAD) y Modelo E-R cifrado.
* **Desarrollo:** Código fuente versionado y contenedores (Docker).
* **Calidad:** Reportes de Pentesting y casos de prueba de regresión.

### 4.3. Roles y Responsabilidades
* **Arquitecto de Software:** Líder de infraestructura y seguridad.
* **Analista de QA Médico:** Validación de precisión clínica.
* **Product Owner:** Representante institucional que prioriza el backlog.

### 4.4. Artefactos Generados
Durante el ciclo de vida, se producen los siguientes documentos y productos técnicos:
* **Estratégicos:** Acta de Constitución (Project Charter) y Plan de Gestión del Proyecto.
* **Requerimientos:** Especificación de Requisitos de Software (SRS) bajo estándar IEEE 830.
* **Diseño:** Documento de Arquitectura de Software (SAD), Diagramas de Secuencia y Modelo E-R cifrado.
* **Implementación:** Código fuente versionado (Git), Scripts de base de datos y Contenedores (Docker).
* **Cierre:** Manual de Usuario, Manual Técnico y Reporte de Lecciones Aprendidas.

### 4.5. Métricas de Seguimiento (KPIs de Proyecto)
Para medir el avance y la salud del desarrollo:
* **Velocidad del Equipo:** Puntos de historia completados por iteración.
* **Burndown Chart:** Seguimiento del trabajo pendiente vs. tiempo restante.
* **Densidad de Errores:** Número de bugs detectados por cada 1,000 líneas de código (KLOC).
* **Cobertura de Código:** Porcentaje de código verificado por pruebas unitarias (Objetivo: >85%).

## 4.6. Gestión de Riesgos y Aseguramiento de Calidad (QA)

### 4.6.1. Matriz de Riesgos
| Riesgo | Impacto | Probabilidad | Plan de Mitigación |
| :--- | :--- | :--- | :--- |
| **Fuga de Datos (HCE)** | Crítico | Baja | Cifrado AES-256 en reposo y tránsito + Auditoría de logs. |
| **Incompatibilidad HL7** | Alto | Media | Uso de middleware de integración y pruebas de interoperabilidad tempranas. |
| **Resistencia al Cambio** | Medio | Alta | Sesiones de capacitación y diseño centrado en el usuario (UX). |

### 4.6.2. Estrategia de Aseguramiento de Calidad (SQA)
El control de calidad se basa en un enfoque de "Pruebas Tempranas":
* **Pruebas Unitarias e Integración:** Automatizadas en el pipeline de CI/CD.
* **Pruebas de Seguridad (Dast/Sast):** Escaneo de vulnerabilidades en cada despliegue.
* **Validación Clínica:** Pruebas de aceptación (UAT) realizadas por personal médico real.
* **Cumplimiento Normativo:** Auditoría técnica de estándares de salud (ej. HIPAA o normativas locales).

## 4.7. Estrategia de Mantenimiento
Una vez el sistema está en producción, se activan los siguientes niveles de mantenimiento:

1. **Mantenimiento Correctivo:** Resolución inmediata de fallos que afecten la operación clínica (SLA de 2 horas para críticos).
2. **Mantenimiento Evolutivo:** Actualización semestral para añadir nuevas funcionalidades médicas o módulos (ej. Telemedicina).
3. **Mantenimiento Adaptativo:** Ajustes por cambios en leyes de salud o actualizaciones en navegadores/S.O.
4. **Mantenimiento Perfectivo:** Refactorización de código para mejorar el rendimiento de las consultas en la base de datos.

---

## 5. Simulación Ejecutiva

### 5.1. Roadmap y Estimación
* **Mes 1-2:** Infraestructura Cloud y Seguridad (**Hito: Core Estable**).
* **Mes 3-4:** Módulo de consulta externa (**Hito: Beta Interna**).
* **Mes 6:** Lanzamiento oficial e interoperabilidad (**Hito: Go-Live**).
* **Esfuerzo:** ~3.500 horas/hombre con un equipo de 6 especialistas.

### 5.2. Estimación de Alto Nivel
**Equipo de Proyecto (6 personas):**
* 1 Project Manager (PM)
* 1 Arquitecto de Software
* 3 Desarrolladores Full-stack
* 1 Ingeniero de QA

**Métricas de Esfuerzo:**
* **Esfuerzo Total:** 3,456 horas/hombre.
* **Duración:** 6 meses (24 semanas).

**Distribución del Esfuerzo:**
* 📋 **Análisis y Diseño:** 15%
* 💻 **Desarrollo (Codificación):** 50%
* 🧪 **Pruebas y QA:** 25%
* 🚀 **Despliegue y Capacitación:** 10%

### 5.3. Identificación de Hitos 

| Hito | Descripción | Semana |
| :--- | :--- | :--- |
| **Hito 1** | Aprobación del Diseño de Arquitectura y Seguridad | 4 |
| **Hito 2** | Finalización Iteración 1 (Identidad y Registro) | 8 |
| **Hito 3** | Entrega Iteración 2 (Módulo de Consulta Funcional) | 16 |
| **Hito 4** | Pruebas de Estrés y Seguridad (Penetración) superadas | 22 |
| **Hito 5** | Cierre del Proyecto y Go-Live en Clínica Piloto | 24 |

### 5.4. Indicadores Clave (KPIs)
* **Uptime:** Disponibilidad > 99.9%.
* **Eficiencia:** Carga de registros < 2 segundos.
* **Calidad:** < 1 defecto crítico en producción por trimestre.

### 5.4. Riesgos y Mitigación
> [!IMPORTANT]
> **Riesgo Crítico:** Acceso no autorizado a historias clínicas.  
> **Mitigación:** MFA (Autenticación Multifactor) y logs de auditoría inalterables (Blockchain/Hash-chaining).

---

## 6. Conclusión
La aplicación del **Modelo Iterativo** garantiza un equilibrio entre la robustez técnica y la flexibilidad necesaria en el sector salud.
Al priorizar el feedback continuo, se asegura que el producto final sea una herramienta que salve vidas y proteja la privacidad ciudadana.
