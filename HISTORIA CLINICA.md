- # Proyecto_1_Corte
# Diseño y Aplicación de un Modelo de Ciclo de Vida del Software (SDLC)

**Programa:** Ingeniería de Sistemas  
**Asignatura:** Procesos De Software 
**Caso Base:** Sector Salud (Sistemas de Historias Clinicas)

---

## 1. Introducción
El **Ciclo de Vida del Software (SDLC)** El Ciclo de Vida del Software (SDLC) comprende el conjunto de procesos mediante los cuales se concibe, desarrolla,
implementa y mantiene un sistema de información.Existen múltiples enfoques como Cascada, Incremental, Prototipado, Iterativo, Modelo en V, Espiral, Unified Process,
metodologías ágiles como Scrum y XP, además de marcos normativos como IEEE 1074.

En el contexto de la salud, donde la integridad de los datos y la disponibilidad del sistema son críticas,
la elección del modelo no es solo una decisión técnica, sino una **decisión mas estratégica** que impacta directamente
en la seguridad del paciente y el cumplimiento normativo de los sistemas integrados.

---

## 2. Análisis Comparativo de Modelos

### 2.1. Modelo en Cascada (Waterfall)
* **Descripción:** Enfoque lineal y secuencial donde cada fase debe completarse antes de iniciar la siguiente.
* **Ventajas:** Estructura trasnparente y sencilla y documentación muy completa.
* **Debilidades:** Escasa adaptabilidad de la estructura frente a nuevas exigencias.
* **Proyectos adecuados:** Sistemas con requisitos críticos, fijos y bien comprendidos.
## IMAGEN ( Guia )
<img width="290" height="174" alt="image" src="https://github.com/user-attachments/assets/9f8aaf9a-cce7-4bb4-aa66-a72bbed70894" />

### 2.2. Modelo Incremental
* **Descripción:** El software se divide en partes funcionales llamadas "incrementos".
* **Ventajas:** Entrega temprana de valor y reducción del impacto de fallos modulares.
* **Debilidades:** Requiere una arquitectura inicial muy sólida.
* **Proyectos adecuados:** Sistemas modulares donde el *time-to-market* es vital.
## IMAGEN ( Guia )
<img width="800" height="600" alt="image" src="https://github.com/user-attachments/assets/24caf6a4-2f65-4bc1-b352-02b7fa4206fb" />

### 2.3. Modelo de Prototipado
* **Descripción:** Construcción de versiones preliminares para validar requisitos con el usuario.
* **Ventajas:** Reduce la brecha de comunicación y asegura el cumplimiento de expectativas.
* **Debilidades:** Riesgo de omitir estándares de calidad por la rapidez.
* **Proyectos adecuados:** Sistemas con interfaces complejas o requisitos vagos.
## IMAGEN ( Guia )
<img width="640" height="480" alt="image" src="https://github.com/user-attachments/assets/bdc001fe-2be9-4928-bc34-ecb5e09d4168" />

### 2.4. Modelo Iterativo
* **Descripción:** El desarrollo se organiza en ciclos repetitivos donde el producto se refina y expande.
* **Ventajas:** Gestión de riesgos temprana y alta adaptabilidad.
* **Debilidades:** Complejidad en la gestión de la configuración.
* **Proyectos adecuados:** Sistemas complejos con alta incertidumbre técnica.
## IMAGEN ( Guia )
<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/3488ba9b-8745-4a92-9c5a-8af43c1a2b07" />


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
4.  **Tamaño y Estructura del Equipo**
Para ejecutar este modelo iterativo con éxito y cubrir las **3.500 horas/trabajadorque** estimadas, se ha conformado un equipo multidisciplinario de **6 especialistas**:

| Rol | Cantidad | Función en el Ciclo Iterativo |
| :--- | :---: | :--- |
| **Arquitecto de Software** | 1 | Define la estructura base y asegura la seguridad de los datos. |
| **Desarrollador Full-Stack (Sr)** | 1 | Lidera la implementación técnica de los módulos críticos. |
| **Desarrollador Full-Stack (Mid)** | 1 | Ejecuta tareas de codificación y soporte en integraciones de APIs. |
| **Analista de QA / Tester** | 1 | Realiza pruebas de regresión y validación clínica en cada ciclo. |
| **Ingeniero DevOps / Seguridad** | 1 | Garantiza el despliegue continuo y la integridad de los datos. |
| **Product Owner (Enlace Médico)** | 1 | Prioriza los requisitos del backlog para la siguiente iteración. |

---
5. **Presupuesto Base del Proyecto**
El presupuesto se ha calculado para cubrir un ciclo de desarrollo de **6 meses**, garantizando la viabilidad financiera de las iteraciones propuestas:

| Categoría | Concepto | Inversión Estimada (USD) |
| :--- | :--- | :---: |
| **Talento Humano** | Salarios del equipo técnico por 6 meses. | $500.000.000 |
| **Infraestructura** | Servicios Cloud (AWS/Azure) y Bases de Datos. | $48.000.000 |
| **Seguridad y Cumplimiento** | Auditorías, certificados SSL y herramientas MFA. | $34.000.000 |
| **Herramientas** | Licencias de software y entornos de testing. | $14.000 |
| **Reserva de Contingencia** | Margen del 10% para cambios normativos imprevistos. | $50.600.000 |
| **TOTAL ESTIMADO** | | **$655.600.000* |
---

## Anexo: Análisis Financiero y Sustentación del Presupuesto

El presupuesto total de **$655.600.000 COP** para un periodo de 6 meses se desglosa de la siguiente manera:

### 5.1. Desglose del Talento Humano ($500.000.000 COP)
Este proceso cubre a 6 especialistas. En Colombia, el costo empresa incluye el salario básico más una **carga prestacional de aproximadamente el 45%** (Seguridad social, primas, cesantías, intereses de cesantías, vacaciones y parafiscales).

| Perfil Profesional | Costo Mensual (Básico + Prestaciones) | Total (6 Meses) |
| :--- | :--- | :--- |
| **Arquitecto de Software** | $18.000.000 | $108.000.000 |
| **Dev Full-Stack Senior** | $15.000.000 | $90.000.000 |
| **Ingeniero DevOps/Seguridad**| $14.000.000 | $84.000.000 |
| **Product Owner (Especialista)**| $11.000.000 | $66.000.000 |
| **Dev Full-Stack Mid** | $10.000.000 | $60.000.000 |
| **Analista de QA / Tester** | $8.500.000 | $51.000.000 |
| **Subtotal Personal** | | **$459.000.000** |

*Nota: Se redondea a **$500M** para cubrir costos de implementacion y dotaciones a los empleados  (computadoras de alto rendimiento y sistemas requeridos para completatar este proyecto) y gastos operativos.*
---

### 2. Infraestructura y Seguridad ($82.000.000 COP)
* **Servicios Cloud ($48M):** Estimación de **$8.000.000 COP/mes** en AWS/Azure para entornos de producción, pruebas y backups de datos médicos de alta disponibilidad.
* **Seguridad y Licencias ($34M):** Certificados SSL Wildcard, herramientas de análisis de vulnerabilidades (Snyk/SonarQube) y autenticación multifactor (MFA).
---

### 3. Herramientas y Contingencia ($73.600.000 COP)
* **Herramientas ($14M):** Licenciamiento de Jira, GitHub Enterprise y herramientas de diseño.
* **Reserva de Contingencia ($59.6M):** Fondo del 10% destinado a cambios normativos imprevistos por el Ministerio de Salud o actualizaciones de estándares (CIE-10 / HL7).

**Total Proyecto: $655.600.000 COP**

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

## DIAGRAMA
<img width="923" height="521" alt="image" src="https://github.com/user-attachments/assets/a331ecc7-1a2e-4980-8ada-a0ca5b7b38f7" />

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

## 6. VALORES TECNICOS Y PRESUPUESTOS CON REFERENCIAS DE PESO 


### 6.1. Salarios y Mercado Laboral (Referentes TI)
* **Guía Salarial de Hays Colombia:** Considerada el referente anual más importante para salarios en TI. Según reportes recientes (2024-2025), perfiles como el **Arquitecto de Software Senior** promedian entre **$15.000.000 y $22.000.000 COP** mensuales bajo contrato laboral, debido a la alta especialización requerida.
* **Fedesoft (Interacción):** La Federación Colombiana de la Industria del Software valida que la escasez de talento Senior y perfiles **DevOps/Ciberseguridad** impulsa rangos salariales competitivos para retener personal en proyectos de misión crítica.

---

### 6.2. Carga Prestacional (Marco Legal Colombiano)
De acuerdo con el **Código Sustantivo del Trabajo (CST)**, el costo real de un empleado para la organización incluye rubros obligatorios que elevan el gasto entre un **42% y 53%** sobre el salario base:

| Concepto | Porcentaje (Aprox.) |
| :--- | :---: |
| **Salud (Aporte Empleador)** | 8.5% |
| **Pensión (Aporte Empleador)** | 12.0% |
| **Parafiscales (Caja de Compensación)** | 4.0% |
| **Prestaciones (Primas, Cesantías, Intereses)** | 21.8% |
| **Seguridad (ARL y otros)** | Variable |



---

### 6.3. Costos de Infraestructura y Estándares de Salud
* **Calculadora de Precios AWS/Azure:** El cumplimiento de la **Ley 1581 de 2012** (Protección de Datos Personales) exige entornos con redundancia, cifrado en reposo y tránsito, y firewalls de aplicación. Esto justifica una inversión mensual de **~$2,000 USD** para un sistema de salud escalable y seguro.
* **Resolución 866 de 2021 (MinSalud):** Esta norma exige el uso de estándares de interoperabilidad como **HL7 FHIR**. La implementación de estos protocolos requiere personal con certificaciones específicas y herramientas de validación de datos que incrementan el costo operativo frente a un software genérico.

---

### 6.4. Gestión de Riesgos y Contingencia
* **PMBOK (Project Management Body of Knowledge):** Los estándares internacionales de gestión de proyectos sugieren que en sectores de alta incertidumbre regulatoria (salud o banca), es obligatorio asignar una **reserva de contingencia de entre el 10% y el 15%** del presupuesto total. 
* Este fondo asegura la continuidad del proyecto ante cambios inesperados en la normativa de salud pública o actualizaciones tecnológicas críticas.

## 7. Conclusión
La aplicación del **Modelo Iterativo** garantiza un equilibrio entre lo robusto ,técnico y la flexibilidad necesaria en el sector salud.
Al priorizar el feedback continuo, se asegura que el producto final sea una herramienta que salve vidas y proteja la privacidad ciudadana.



## 8. Bibliografía y Fuentes de Respaldo
Para la presentacion de este proyecto y sus presupuestos a nivel nacional(COLOMBIA) se ha investigado las siguientes fuetes oficiales y consulatas a industrias:

### 8.1. Marco Legal y Prestacional (Colombia)
* **Congreso de la República de Colombia.** (1950). *Código Sustantivo del Trabajo*. Adopción de cargas prestacionales y seguridad social para contratos laborales.
* **Congreso de la República de Colombia.** (2012). *Ley 1581 de 2012: Protección de Datos Personales*. Marco regulatorio para el manejo de historias clínicas y datos sensibles.
* **Ministerio de Salud y Protección Social.** (2021). *Resolución 866 de 2021*. Requisitos de interoperabilidad y estándares de datos para la Historia Clínica Electrónica.

### 8.2. Estándares de Ingeniería y Salarios
* **Hays Colombia.** (2025). *Guía Salarial 2025: Tendencias y Salarios en Tecnología*. Reporte de rangos salariales para Arquitectos de Software y Desarrolladores Senior en el mercado local.
* **Fedesoft (Federación Colombiana de la Industria del Software).** (2024). *Informe de Caracterización del Sector TI*. Estadísticas sobre costos operativos y demanda de perfiles especializados.
* **Project Management Institute (PMI).** (2021). *A Guide to the Project Management Body of Knowledge (PMBOK Guide)* (7ma ed.). Estándares para la gestión de riesgos y reservas de contingencia en proyectos complejos.

### 8.3. Infraestructura y Tecnología
* **Amazon Web Services (AWS).** (2026). *Cloud Pricing Calculator*. Estimación de costos para servicios de alta disponibilidad y bases de datos cifradas bajo cumplimiento HIPAA/GDPR.
* **HL7 International.** (2025). *HL7 FHIR (Fast Healthcare Interoperability Resources) Standard*. Guía técnica para el intercambio de información de salud.
